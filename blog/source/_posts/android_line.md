---
title: 구분선 그리기의 모든 것
date: 2018-03-16
tags: 
- Android
- Line
categories:
- Develop
author: 윤명준
---



![대표이미지](http://cracker9.github.io/img/Android_Line/title.png)



안드로이드 뷰를 구성하다보면 다양한 해상도와 화면 크기인 기기에 대한 이해가 종종 필요하다. 나도 윈도우 프로그래밍만 하던 개발자인지라, 일단 여러 해상도,  화면 크기, 단위에 대한 고려 없이 개발을 진행하곤 했다. 
그러다 보니 지정한 디바이스에서 맞게끔 개발을 했는데, 다른 디바이스에서 사용하면 화면 비율이 이상하거나 디자이너 요청 사항처럼 예쁘게 나오지 않는 경우가 많았다. 

따라서 디자이너 요청 대로 화면을 구현하기 위해서는  안드로이드 디바이스에서의 해상도, 화면크기, DPI (화면 밀도)를 이해 해야 한다. 그래야 정확하게 구현 할 수 있다.



## 해상도, 화면크기.. 그리고 DPI
아래는 인터넷에서 “갤럭시 S8 스펙” 하고 검색해서 찾은 삼성 갤럭시 S8 의 디스플레이 스펙이다. 

5.77인치 QHD super AMOLED / 570ppi 

여기서 5.77인치는 화면의 크기 QHD 는 해상도이다.  각 해상도의 픽셀 수는 아래와 같다.


|이름  | 해상도|
|:---:|:---:|
|nHD | 640×360|
|qHD | 960×540|
|HD | 1280×720|
|HD+ | 1600×900|
|FHD | 1920×1080|
|Full-HD+ | 2220×1080|
|QHD | 2560×1440|
|QHD+ | 3200×1800|
|UHD | 3840×2160|
|UHD+ | 5120×2880|
|QUHD | 7680×4320|


PPI 는 무엇일까? Pixel per Inch, 즉 인치 당 들어가는 Pixel 의 수이다. 

그럼 안드로이드에서 사용하는 DPI 는 무엇일까? DPI 는 Dot per Inch, 인치 당 들어가는 점의 수이다. DPI 와 PPI 는 1:1 이므로 크게 신경 쓰지 말자.

그렇다면 갤럭시 S8 을 기준으로 하는 안드로이드 앱을 만들려고 할 때 DPI 는 어떻게 될까?  화면의 크기로 1인치에 몇개나 Pixel 이 들어가는지 계산 해 보자. 그리고 해당 숫자에 알맞은 dpi 를 찾아 보자.

dpi | 1인치당 최대 도트 수
--|--
ldpi (저밀도) | ~120dpi
mdpi (중간 밀도) | ~160dpi
hdpi (고밀도) | ~240dpi
xhdpi (초고밀도) | ~320dpi
xxhdpi (초초고밀도) | ~480dpi
xxxhdpi (초초초고밀도) |  ~640dpi


디스플레이의 면적과 해상도를 가지고 1인치에 들어 있는 dot 수를 계산하면 갤럭시 S8은 기준 dpi 가 xxhdpi 인 걸 알 수 있다.

사실 이 부분은 안드로이드 스튜디오에서 Virtual Device 를 생성할 때,  Screen Size 와 Resolution 을 입력하면 자동으로 계산 해 주는 부분이긴 하다. 



## 다양한 선 그리는 방법들

구분선을 그리는 방법은 사실 개발자 마음이다. 

View 로 그리든.. Drawable 로 하든.. 하지만 일반적으로 사용하는 방법은 몇 가지로 좁혀진다.



### 일반적인 구분선 그리기

####  (1)  View 로 그리기

가장 일반적인 방법이다. 

~~~ html
<View
   android:layout_width="match_parent"
   android:layout_height="2dp"
   android:background="#FFFF0000"/>
~~~


#### (2) LinearLayout 의 divider 로 지정
Linear Layout 내부에 있는 동일한 색상에 동일한 길이인 여러 개의 뷰 간의 구분선을 그려줘야 할 때 한꺼번에 그릴 수 있다는 것이 장점이다. 

#### (3) LinearLayout 의 ButtonStyle 로 지정



### 특수한 구분선 그리기


#### 그라데이션이 들어간 선 그리기

우리는 구분선을 그리기 위해 Rectangle 을 사용할 것이다. 중심(빨간색)에서 점점 양쪽(검정색)으로 퍼져 나가는 그라데이션을 그릴 것이다. 일단 Drawable 폴더에 gradient.xml 을 생성한다.

gradient.xml
~~~ html
<?xml version="1.0" encoding="utf-8"?>
<shape
   xmlns:android="http://schemas.android.com/apk/res/android"
   android:shape="rectangle">
   <gradient
       android:angle="0"
       android:startColor="#000000"
       android:endColor="#000000"
       android:centerColor="#FFFF0000" />
</shape>
~~~

그리고 그린 구분선을 activity_main.xml 에서 View 로 사용한다.

~~~ html
<?xml version="1.0" encoding="utf-8"?>
<android.support.constraint.ConstraintLayout
   xmlns:android="http://schemas.android.com/apk/res/android"
   xmlns:app="http://schemas.android.com/apk/res-auto"
   xmlns:tools="http://schemas.android.com/tools"
   android:id="@+id/LinearLayout01"
   android:orientation="vertical"
   android:layout_width="match_parent"
   android:layout_height="match_parent">

   <TextView
       android:id="@+id/textView2"
       android:layout_width="wrap_content"
       android:layout_height="wrap_content"
       android:layout_marginLeft="24dp"
       android:layout_marginTop="16dp"
       android:text="Title"
       app:layout_constraintLeft_toLeftOf="parent"
       app:layout_constraintTop_toTopOf="parent" />

   <View
       android:id="@+id/view3"
       android:layout_width="0dp"
       android:layout_height="1dp"
       android:layout_marginTop="8dp"
       android:background="@drawable/gradient"
       app:layout_constraintHorizontal_bias="0.0"
       app:layout_constraintLeft_toLeftOf="parent"
       app:layout_constraintRight_toRightOf="parent"
       app:layout_constraintTop_toBottomOf="@+id/textView2"></View>

   <TextView
       android:id="@+id/textView3"
       android:layout_width="wrap_content"
       android:layout_height="wrap_content"
       android:layout_marginLeft="24dp"
       android:layout_marginTop="8dp"
       android:text="Name"
       app:layout_constraintLeft_toLeftOf="parent"
       app:layout_constraintTop_toBottomOf="@+id/view3" />

   <View
       android:id="@+id/view4"
       android:layout_width="0dp"
       android:layout_height="1px"
       android:layout_marginTop="8dp"
       android:background="@drawable/gradient"
       app:layout_constraintHorizontal_bias="0.0"
       app:layout_constraintLeft_toLeftOf="parent"
       app:layout_constraintRight_toRightOf="parent"
       app:layout_constraintTop_toBottomOf="@+id/textView3"></View>


</android.support.constraint.ConstraintLayout>
~~~



여기서 주의할 점은 첫번째 뷰와 두번째 뷰의 layout_height 이다. 첫번째는 1dp, 두번째는 1px 로 했다. 어떤 차이가 생기는지 확인 해 보자.![img0](http://cracker9.github.io/img/Android_Line/img0.png)



실제 그려지는데 많은 차이가 있는 것을 알 수 있다. 

이런 부분에 대해서  디자이너에게 알려줄 필요가 있다. 



## 실전 활용의 예



실무에 적용 해보자.  아래의 예제들은 내가 실전에서 겪었던 사례들이다.



#### 레이아웃과 레이아웃 사이에 구분선이 들어가는 예	

![img1](http://cracker9.github.io/img/Android_Line/img1.png)



#### Linear Layout 으로 묶고 버튼과 버튼 사이의 divider 를 넣은 예



![img2](http://cracker9.github.io/img/Android_Line/img2.png)



## 1px 과 1dp 어떤 것이 정답일까?



다양한 해상도를 지원해야 하는 앱(요새는 다 그래야 하지 않나?)에서는 dp 를 사용하는게 적합 해 보인다. px 로 하게 되면 해상도가 높은 디바이스에서는 구분선이 안보이는 경우도 있을 수 있다. px 로 하는게 적합한 상황도 있다.1dp 보다 더 얇은 구분선을 그리고 싶을 때!앱 개발 할 때 많은 도움이 되었으면 하는 바람이다.

