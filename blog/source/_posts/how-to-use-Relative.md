---
title: Tutorial - Relative Layout 사용법
date: 2018-06-27 10:00:00
tags: 
- Android
- Layout
- Cracker9
categories:
- Tutorial
author: Cracker9
---
<span style="color:#4d4d4d">안녕하세요. 크래커나인 입니다.
오늘은 Relaitve Layout을 사용하여 코드를 생성해보도록 하겠습니다.
***
### 1. Relative Layout 소개
<span style="color:#4d4d4d">Relative는 부모 혹은 다른 자식 View와의 상대적 위치를 이용해 화면을 구성하는 방법입니다.
더 정확한 Relative Layout에 대한 설명은 이곳을 참고해주세요.
[참고 사이트](https://developer.android.com/guide/topics/ui/layout/relative)


<span style="color:#4d4d4d">기준이 되는 View A와 다른 View B가 있다면
![Relative01](/img/HowToUseRelative/01.jpg?raw=true)
#  

<span style="color:#4d4d4d">아래와 같은 경우는 ‘B가 A의 왼쪽에 배치한다’ 입니다. 코드는 android:layout_toLeftOf=A 를 작성합니다.
![Relative02](/img/HowToUseRelative/02.jpg?raw=true)
#  

<span style="color:#4d4d4d">다음은 ‘B가 A의 위에 배치한다’ 입니다. 코드는 android:layout_above=A를 작성합니다.
![Relative03](/img/HowToUseRelative/03.jpg?raw=true)
#  

<span style="color:#4d4d4d">아래와 같은 경우는 B를 A와 왼쪽 변을 맞추는 것입니다. 코드는 android:layout_alignLeft=A 를 작성합니다
![Relative04](/img/HowToUseRelative/04.jpg?raw=true)
#  

<span style="color:#4d4d4d">만일 View A가 View B를 포함하는 부모이고,
B를 부모와 왼쪽 변을 맞추면 코드는 android:layout_alignParentLeft=True 를 작성합니다.
![Relative05](/img/HowToUseRelative/05.jpg?raw=true)
#  

<span style="color:#4d4d4d">B를 부모의 수직,수평 중앙에 맞추면 코드는 android:layout_centerParent=True 를 작성합니다.
![Relative06](/img/HowToUseRelative/06.jpg?raw=true)
#  

<span style="color:#4d4d4d">Relative는 부모 Layout과 자식 view 혹은 자식 view들간의 관계가 필요합니다.
Cracker9 툴은 이를 코드로 작성하지 않고 마우스로 연결하여 쉽게 관계를 맺을 수 있습니다.

### 2. Cracker9에서 관계맺기 방법
<span style="color:#4d4d4d">**STEP 01.** Relative로 코드를 구성할 View 선택 후 Design Panel로 옮겨줍니다.
![Relative07](/img/HowToUseRelative/07.gif?raw=true)
#  

<span style="color:#4d4d4d">**STEP 02.** 오른쪽 Setting Panel에서 Layout을 Relative로 설정합니다.
![Relative08](/img/HowToUseRelative/07.jpg?raw=true)
#  

<span style="color:#4d4d4d">**STEP 03.** 부모 안에 포함된 자식 View을 선택하세요.관계를 맺을 수 있는 아이템을 선택하면 위와 같이 보여지며,
![Relative09](/img/HowToUseRelative/08.jpg?raw=true)
#  

<span style="color:#4d4d4d">연결 상태는 다음과 같습니다.
![Relative10](/img/HowToUseRelative/09.jpg?raw=true)
#  

<span style="color:#4d4d4d">**STEP 04.** View 선택 후 View의 왼쪽을 부모와 연결합니다.
![Relative11](/img/HowToUseRelative/10.jpg?raw=true)
#  

<span style="color:#4d4d4d">**STEP 05.** View 선택 후 View의 상단을 부모 상단과 연결합니다.
![Relative12](/img/HowToUseRelative/11.jpg?raw=true)
#  

<span style="color:#4d4d4d">**STEP 06.** 두번째 View 선택 후 View의 왼쪽을 첫번째 View의 오른쪽과 연결합니다.
![Relative13](/img/HowToUseRelative/12.jpg?raw=true)
#  

<span style="color:#4d4d4d">**STEP 07.** 두번째 View 선택 후 View의 상단을 부모의 상단과 연결합니다.
![Relative14](/img/HowToUseRelative/13.jpg?raw=true)
#  

<span style="color:#4d4d4d">**STEP 08.** 세번째 아이템 선택 후 아이템의 왼쪽을 두번째 아이템의 왼쪽과 연결합니다.
![Relative15](/img/HowToUseRelative/14.jpg?raw=true)
#  

<span style="color:#4d4d4d">**STEP 09.** 세번째 아이템 선택 후 아이템의 상단을 두번째 아이템의 하단과 연결합니다.
![Relative16](/img/HowToUseRelative/15.jpg?raw=true)
#  

<span style="color:#4d4d4d">**STEP 10.** 더 정확한 이해를 돕기 위해 영상을 첨부했습니다.
[![Relative20](/img/HowToUseRelative/v03.jpg?raw=true)](https://youtu.be/2JvLv_PYAxU)  
#  

<span style="color:#4d4d4d">**STEP 11.** View끼리 서로 연결된 결과는 각각 View를 선택해도 확인할 수 있지만, 더 자세한 사항은 오른쪽 Setting Panel > Relation에서도 확인 할 수 있습니다.
![Relative17](/img/HowToUseRelative/17.jpg?raw=true)
#  

<span style="color:#4d4d4d">**STEP 12.** Setting Panel 아래의 Generate Code 버튼을 선택해주세요.
![Relative18](/img/HowToUseRelative/18.jpg?raw=true)
#  

<span style="color:#4d4d4d">**STEP 13.** Code Result Panel이 나오면 코드가 제대로 나왔는지 확인해주세요.
![Relative19](/img/HowToUseRelative/19.jpg?raw=true)
#  


<span style="color:#4d4d4d">그럼, 그 외에 문의사항은 [hello@cracker9.io](helloo@cracker9.io) 로 메일주세요!
크래커나인는 디자이너와 개발자들이 Creative에 집중할 수 있도록 돕겠습니다.

Cracker9 이 없다면 ▶ [클릭](http://cracker9.io/#skip-downloads)
Cracker9 으로 Relative Layout 을 구성 해 보고 싶다면  ▶ [클릭](https://release.cracker9.io/code-snippet/artboards/402afe59-88df-4933-b22b-885b3fb11531/)

_____

* Homepage_ http://cracker9.io
* Blog_ https://blog.cracker9.io
* Facebook_ https://www.facebook.com/cracker9.io

_____
