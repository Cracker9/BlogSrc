---
title: 디자이너에게 요청하지 않고 안드로이드 아이콘을 만들기
date: 2018-04-05
tags: 
- Android
- ICON
categories:
- Develop
author: Cracker9
---

디자이너가 앱에 필요한 아이콘을 그때그때 직접 만들어준다면 문제가 없지만, 불가피하게 디자이너 없이 만들어야 하는 경우도 있을 것이다.
그런 이들을 위해 Android Studio에는 Image Asset Studio라는 기능이 포함되어 있다. 또한 웹에서 이와 관련된 툴도 존재한다.
과연 이 툴을 사용하여 아이콘을 어떻게 만들 수 있는지 알아보았다.

우선 그 전에 아이콘 소스들이 필요하므로 다운받았다.

* Material 아이콘 : https://material.io/icons/
* Nounproject : https://thenounproject.com/

## Android studio의 Image Asset studio

아이콘을 다운 받았으면 실제로 어떻게 안드로이드의 다양한 해상도에 맞춰서 제작하면 된다.우선 안드로이드 스튜디오 툴안에 있는 Image Asset Studio로 만들어보도록 하자.

처음에는 어플의 간판 같은 존재, 런처 아이콘을 만들어 보았다.

1)안드로이드 스튜디오의 리소스 폴더를 오른쪽 마우스 클릭한다.

2)image asset 메뉴를 선택한다.
![1](https://github.com/sohee9/test_Doc/blob/master/Image%20Asset%20studio_%E1%84%85%E1%85%A5%E1%86%AB%E1%84%8E%E1%85%A5%E1%84%8B%E1%85%A1%E1%84%8B%E1%85%B5%E1%84%8F%E1%85%A9%E1%86%AB1.png?raw=true)

3)Item type 에서 luncher icon 선택한다.

4)아이콘 이름, 이미지, 색상, 정돈, 여백 등 세팅한다.
![2](https://github.com/sohee9/test_Doc/blob/master/Image%20Asset%20studio_%E1%84%85%E1%85%A5%E1%86%AB%E1%84%8E%E1%85%A5%E1%84%8B%E1%85%A1%E1%84%8B%E1%85%B5%E1%84%8F%E1%85%A9%E1%86%AB2.png?raw=true)

5)내가 세팅한 값에 따라서 미리보기를 할 수 있으니 참고해가며 조정하면 된다.
![3](https://github.com/sohee9/test_Doc/blob/master/Image%20Asset%20studio_%E1%84%85%E1%85%A5%E1%86%AB%E1%84%8E%E1%85%A5%E1%84%8B%E1%85%A1%E1%84%8B%E1%85%B5%E1%84%8F%E1%85%A9%E1%86%AB3.png?raw=true)

6)예상 결과물 확인한다.
![4](https://github.com/sohee9/test_Doc/blob/master/Image%20Asset%20studio_%E1%84%85%E1%85%A5%E1%86%AB%E1%84%8E%E1%85%A5%E1%84%8B%E1%85%A1%E1%84%8B%E1%85%B5%E1%84%8F%E1%85%A9%E1%86%AB4.png?raw=true)

7)실제 폴더에 들어가 있는지 확인한다.
![5](https://github.com/sohee9/test_Doc/blob/master/Image%20Asset%20studio_%E1%84%85%E1%85%A5%E1%86%AB%E1%84%8E%E1%85%A5%E1%84%8B%E1%85%A1%E1%84%8B%E1%85%B5%E1%84%8F%E1%85%A9%E1%86%AB5.png?raw=true)

이미지 Asset외에 Vector 아이콘을 만들 수 있는데, 안드로이드 스튜디오에서 제공하는 Material 아이콘이나 가지고있는 SVG 아이콘으로 만들 수 있다.

<Material 아이콘을 만드는 과정>

1)안드로이드 스튜디오의 리소스 폴더를 오른쪽 마우스 클릭한다.
2)Vector asset 메뉴를 선택한다.
![1](https://github.com/sohee9/test_Doc/blob/master/Image%20Asset%20studio_%E1%84%87%E1%85%A6%E1%86%A8%E1%84%90%E1%85%A5%E1%84%8B%E1%85%A1%E1%84%8B%E1%85%B5%E1%84%8F%E1%85%A9%E1%86%AB1.png?raw=true)

3)Asset Type에서 Material icon 선택
![2](https://github.com/sohee9/test_Doc/blob/master/Image%20Asset%20studio_%E1%84%87%E1%85%A6%E1%86%A8%E1%84%90%E1%85%A5%E1%84%8B%E1%85%A1%E1%84%8B%E1%85%B5%E1%84%8F%E1%85%A9%E1%86%AB3.png?raw=true)

4)icon 버튼을 선택하여 안드로이드 스튜디오에서 제공하는 아이콘을 선택한다.
![3](https://github.com/sohee9/test_Doc/blob/master/Image%20Asset%20studio_%E1%84%87%E1%85%A6%E1%86%A8%E1%84%90%E1%85%A5%E1%84%8B%E1%85%A1%E1%84%8B%E1%85%B5%E1%84%8F%E1%85%A9%E1%86%AB2.png?raw=true)

5)리소스 파일 경로를 확인하고 Finish!
![4](https://github.com/sohee9/test_Doc/blob/master/Image%20Asset%20studio_%E1%84%87%E1%85%A6%E1%86%A8%E1%84%90%E1%85%A5%E1%84%8B%E1%85%A1%E1%84%8B%E1%85%B5%E1%84%8F%E1%85%A9%E1%86%AB4.png?raw=true)


<SVG파일로 아이콘을 만드는 과정>

1)Asset Type에서 Local file 선택
2)Path에서 내가 가진 SVG파일 경로를 찾아 선택
![5](https://github.com/sohee9/test_Doc/blob/master/Image%20Asset%20studio_%E1%84%87%E1%85%A6%E1%86%A8%E1%84%90%E1%85%A5%E1%84%8B%E1%85%A1%E1%84%8B%E1%85%B5%E1%84%8F%E1%85%A9%E1%86%AB5.png?raw=true)

3)리소스 파일 경로를 확인하고 Finish!
![6](https://github.com/sohee9/test_Doc/blob/master/Image%20Asset%20studio_%E1%84%87%E1%85%A6%E1%86%A8%E1%84%90%E1%85%A5%E1%84%8B%E1%85%A1%E1%84%8B%E1%85%B5%E1%84%8F%E1%85%A9%E1%86%AB6.png?raw=true)

## Roman Nurik Android Asset studio

https://romannurik.github.io/AndroidAssetStudio/index.html
이번에는 웹에서도 아이콘을 만들 수 있는 툴을 사용해보자.
웹사이트 메인에 가면 상당히 다양한 종류의 아이콘을 만들 수 있는데, 나인패치도 만들 수 있다.
필자는 일반 아이콘을 만들어보았다.

![1](https://github.com/sohee9/test_Doc/blob/master/Android%20Asset%20studio_%E1%84%8B%E1%85%A1%E1%84%8B%E1%85%B5%E1%84%8F%E1%85%A9%E1%86%AB1.png?raw=true)

1)Source 부분에서 Image를 선택하고 이미지 파일을 선택한다.
![2](https://github.com/sohee9/test_Doc/blob/master/Android%20Asset%20studio_%E1%84%8B%E1%85%A1%E1%84%8B%E1%85%B5%E1%84%8F%E1%85%A9%E1%86%AB2.png?raw=true)

2)Padding, Asset size, Color등을 세팅한다.
![3](https://raw.githubusercontent.com/sohee9/test_Doc/bf452f8e628cf0f85ffaa1336505733167866d7a/Android%20Asset%20studio_%E1%84%8B%E1%85%A1%E1%84%8B%E1%85%B5%E1%84%8F%E1%85%A9%E1%86%AB3.png)

3)미리보기에서 'SEE ALL'을 선택하면 다양한 해상도에 맞춰진 아이콘을 확인 할 수 있다.
![4](https://raw.githubusercontent.com/sohee9/test_Doc/bf452f8e628cf0f85ffaa1336505733167866d7a/Android%20Asset%20studio_%E1%84%8B%E1%85%A1%E1%84%8B%E1%85%B5%E1%84%8F%E1%85%A9%E1%86%AB4.png)

4)맨 오른쪽 내려받기 아이콘을 클릭 후 저장된 경로로 들어가 확인한다.
![5](https://github.com/sohee9/test_Doc/blob/master/Android%20Asset%20studio_%E1%84%8B%E1%85%A1%E1%84%8B%E1%85%B5%E1%84%8F%E1%85%A9%E1%86%AB5.png?raw=true)


_____
  <a href="http://www.cracker9.io?utm_medium=cpc&utm_source=blog_origin&utm_campaign=0.11.x&utm_content=Android_Icon_Design" onclick="gtag('event', 'button click', {'event_category': 'Homepage','event_label': 'Android Icon Design'});">![cracker9](/img/Logo/Cracker9_Symbollogo.png?raw=true)</a>
_____