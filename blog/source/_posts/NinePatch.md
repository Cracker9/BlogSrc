---
title: 앤트맨으로 나인패치(9Patch) 이해하기
date: 2018-10-24 12:30
tags: 
- Android
- Ninepatch
- 9patch
- 나인패치
- 앤트맨
- Antman
- 안드로이드
- AssetStudio
categories:
- Design
author: 구소희
---


# **시작**

![](/img/NinePatch/01_antman-395e3e34-6e72-4842-bd3c-568b3e453e6b.gif)

영화 ‘캡틴 아메리카: 시빌워’를 본 사람이라면 작은 ‘앤트맨’의 존재감이 누구보다 컸다고 말할 수 있습니다. 앤트맨은 가장 중요한 전투 신에서 자유자재로 신체 크기를 바꾸며 맹활약을 한 히어로인데요.

안드로이드(Android)에도 이런 앤트맨처럼 크기를 자유자재로 바꾸되, 해상도를 그대로 보존하여 앱을 구현하는데 큰 도움을 주는 이미지 저장방식이 있습니다. 바로 나인패치(9patch)입니다. 포스팅을 통해 나인패치를 이해해보고자 합니다.

# **나인패치 이해하기**

## **#사이즈는 바뀌지만 내용은 그대로**

영화 속 앤트맨은 핌입자를 통해 분자보다 더 작은 양자 사이즈만큼 작아졌다가, 비행기보다 더 큰 사이즈로 변하는 히어로인데요. 핌 입자를 사용시 질량에는 변화가 없어 작아진 크기에서도 정상 어른의 펀치와 같은 위력을 줍니다.

나인패치 역시 앤트맨과 같은 특징을 가지고 있는데요. 우리가 사용하고 있는 핸드폰의 해상도는 제각각 입니다. 하지만 이미지를 그 해상도에 전부 맞춰서 제작하기에는 무리가 있죠. 그렇기 때문에 디바이스에 표현되는 아이콘이나 버튼 등에 확대 되는 영역을 지정해줍니다. 그러면 큰 해상도에 이미지를 적용 하여도 픽셀이 깨지지 않고 확대된 이미지를 사용 할 수 있습니다.

좀 더 정확하게 설명하자면, 이미지를 9분할 하여 확대되는 영역과 아닌 영역을 구분하여 저장하는 방식이며 이미지 확장자는. 9.png가 됩니다. 아래의 그림에서 살펴보면 빨간색 화살표 영역은 늘어나고 흰색 영역은 늘어나지 않게 됩니다.

![](/img/NinePatch/02_9patch-55efbd57-de8c-4753-8eb3-7b6a71850cd9.png)

나인패치로 지정해는 과정이 필요한 이유는 모바일은 한정된 용량을 가지고 있기 때문에 용량을 줄여서 하나의 이미지로 다양하게 사용할 수 있도록 하기 위해서 입니다.

# **나인패치 만들어보기**

## **#만드는 방법**

나인패치를 만드는 방법에는 여러가지가 있습니다.

1. 포토샵으로 만들고, 확장자를 name.9.png으로 저장
2. 안드로이드 sdk 도구를 다운로드하여 만든다.

    [https://developer.android.com/studio/?hl=ko](https://developer.android.com/studio/?hl=ko) 

3. Android Asset Studio 활용

    [http://romannurik.github.io/AndroidAssetStudio/nine-patches.html](http://romannurik.github.io/AndroidAssetStudio/nine-patches.html)

그중에서 툴 설치도 필요 없고 쉽게 만들 수 있는 3번의 방법을 활용하여 간략하게 나마 만들어보겠습니다.

## **#우리는 그저 감사하게 사용할 뿐**

세상은 넓고 금손이 많은 것 같아요. 위 3번의 주소를 타고 들어가시면 아래와 같은 화면이 보여집니다.

![](/img/NinePatch/03_9patch-5132579c-419a-4bbe-aa9b-08c09ade8d43.png)

나인패치를 만들 수 있는 웹 툴인데, 저 사이트에는 나인패치 뿐만 아니라 안드로이드 디자인을 위한 다양한 툴을 제공하니 한번 참고해보시면 좋을 것 같습니다. 언제 이런걸 만들 생각을 하셨는지 한번 더 자괴감과 감사함을 느끼며 샘플 버튼 이미지를 불러옵니다.

![](/img/NinePatch/04_9patch-5e7ded51-016c-43b4-af1c-3fcf93f73541.png)

왼쪽 패널을 보면 이미지의 리소스 해상도를 지정하는 부분과 Drawable 이름을 편집할 수 있는 기능이 있습니다. 이름을 변경하게 되면 zip파일로 다운 받았을 때 변경된 이름으로 다운로드 됩니다.

![](/img/NinePatch/05_9patch-56d881a4-42f9-4a00-a624-13a98d2e7de8.png)

자 그럼 불러온 이미지가 가운데 화면에 보여집니다. Stretch Regions는 늘어나게 되는 부분을 설정하는 것입니다. 화면에 보이는 얇은 검은 선으로 Stretch Regions을 지정하면 됩니다.

![](/img/NinePatch/06_9patch-63ba0afd-b1bd-41a0-8007-96338b7fac6b.png)

위와 같이 설정하게 되면 해상도에 따라 붉은색 부분이 늘어나게 됩니다.

![](/img/NinePatch/07_9patch-06e545e8-53a4-431d-83e8-fe44e911baaa.png)

Contetns Padding은 안에 들어가는 텍스트가 들어가는 여백을 설정해줍니다.

![](/img/NinePatch/08_9patch-86dd65f6-42e0-47e8-ba86-76bf7bc6ad06.png)

오른쪽 패널에서 Preview로 텍스트가 들어가는 것을 확인하면서 설정 할 수 있습니다.

With content를 체크해주셔야 텍스트가 보여집니다.

![](/img/NinePatch/09_9patch-75e9b7fc-3acd-4661-8bf0-eeee73c0097f.png)

완성되면 Assets 탭에서 zip파일을 다운로드 받아주세요.

![](/img/NinePatch/10_9patch-8e90079e-5aca-48f2-91f0-fd414c148d06.png)

다운로드가 완료되면 drawable name.9.zip으로 다운로드 되고 zip파일을 압축해제 하면 해상도 별로 나인패치 파일이 생성됩니다.

부족하지만 나인패치에 대해 알아가는 시간이 되었기를 바라며, 이번 글은 여기서 마무리 하겠습니다.

***

   ▶ Homepage: http://cracker9.io
   ▶ Blog: https://blog.cracker9.io
   ▶ Twitter: https://twitter.com/HelloCracker9
   ▶ Facebook: https://www.facebook.com/cracker9.io

***