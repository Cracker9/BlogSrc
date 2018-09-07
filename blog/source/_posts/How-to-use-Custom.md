---
title: Tutorial - Custom Layout 사용법
date: 2018-06-28 11:00:00
tags: 
- Android
- Layout
- Cracker9
categories:
- Tutorial
author: Cracker9
---
<span style="color:#4d4d4d">안녕하세요. 크래커나인 입니다.
Custom Layout은 디자이너가 만들어 주지 못한 영역을 개발자가 임의의 영역을 직접 그려 레이아웃을 구성 할 수 있도록 만든 기능입니다. 사용하는 방법은 매우 간편해서 쉽게 사용할 수 있습니다.

<span style="color:#4d4d4d">먼저 Custom Layout이 필요한 경우를 알아볼까요?
![Custom_01](/img/HowToUseCustom/01.jpg?raw=true)
#  

<span style="color:#4d4d4d">예를 들어 리스트로 되어 있는 디자인일 때 각각 하나의 리스트를 감싸주는 영역이 필요한데요. 이 때 디자이너가 미리 그 영역까지 그리지 않은 경우가 종종 있습니다. 그래서 이러한 경우 개발자가 직접 디자이너에게 요청하거나 직접 해당하는 영역을 그려야 합니다.

<span style="color:#4d4d4d">이 외에도 영역이 필요할 경우 디자이너에게 요청하는 등의 커뮤니케이션이 발생하는데, Cracker9은 별도의 디자인 추가 작업 없이 개발자가 영역을 지정하는 Custom Layout 기능이 있습니다.

<span style="color:#4d4d4d">자, 그럼 Custom Layout 으로 직접 영역을 만들어보도록 하겠습니다.
Custom Layout으로 영역을 생성하는 방법은 2가지가 있는데, 하나는 선택한 View들의 전체 크기로 만드는 방법과 또 다른 하나는 View를 선택하지 않고 만드는 방법입니다.
***
### 1. 선택한 View들의 전체 크기로 Custom Layout 생성
<span style="color:#4d4d4d">**STEP 01.** View Panel에서 View를 선택한 후 Design Panel로 끌어옵니다.
![Custom_01](/img/HowToUseCustom/03.gif?raw=true)
#  

<span style="color:#4d4d4d">**STEP 02.** Custom Layout이 감싸야하는 View들을 선택해주세요.
![Custom_02](/img/HowToUseCustom/04.jpg?raw=true)
#  

<span style="color:#4d4d4d">**STEP 03.** 상단 툴바에 보시면 Custom Layout을 만들어주는 버튼을 클릭합니다.
![Custom_03](/img/HowToUseCustom/02.jpg?raw=true)
#  

<span style="color:#4d4d4d">**STEP 04.** 내가 선택한 View를 감싸는 영역이 만들어지고 그 아래에 원본 스크린이 보이는데 그 영역을 참고하여 원하는 크기만큼 조절해줍니다.
![Custom_04](/img/HowToUseCustom/06.gif?raw=true)
#  

<span style="color:#4d4d4d">**STEP 05.** Save 버튼을 눌러주세요.

<span style="color:#4d4d4d">**STEP 06.** 필요한 영역이 생성되었습니다.
![Custom_05](/img/HowToUseCustom/07.jpg?raw=true)
#  

<span style="color:#4d4d4d">**STEP 07.** Generate Code로 코드를 생성한 후 해당되는 코드를 확인하면 됩니다. Cracker9에서 제공하는 샘플을 이용하여 Custom Layout을 생성하였을 경우의 코드는 아래와 같습니다.
![Custom_06](/img/HowToUseCustom/08.jpg?raw=true)
#  

### 2. View를 선택하지 않고 Custom Layout 생성

<span style="color:#4d4d4d">**STEP 01.** Design Panel로 View를 끌어왔다면, View를 선택하지 않고 Custom Layout 버튼을 눌러주세요. View를 선택한 상태로 Custom Layout을 선택하면 그 크기만큼의 영역이 생성되기 때문에 선택되지 않아야 합니다.
![Custom_07](/img/HowToUseCustom/09.jpg?raw=true)
#  

<span style="color:#4d4d4d">**STEP 02.** 마우스가 + 모양으로 바뀌면, 아래에 깔려진 원본 스크린을 참고하여 원하는 크기만큼 드래그 하여 영역을 그려줍니다.
![Custom_08](/img/HowToUseCustom/10.jpg?raw=true)
#  

<span style="color:#4d4d4d">**STEP 03.** 원하는 크기로 영역을 그려졌다면 Save 버튼을 눌러 저장해주세요.

<span style="color:#4d4d4d">**STEP 04.** 완성된 모습은 위의 방법과 동일하며 코드 내용도 동일합니다.
#  

<span style="color:#4d4d4d">View를 선택하지 않고, Custom Layout을 사용하면 보다 자유롭게 직접 그려서 영역을 생성 할 수 있다는 장점이 있습니다. 어느 쪽이든 편한 방법으로 사용하면 됩니다.
#  

<span style="color:#4d4d4d">위의 과정을 담은 영상을 첨부하니 참고해주세요.
[![Custom_09](/img/HowToUseCustom/v06.jpg?raw=true)](https://youtu.be/s0UQzVVRk_c)

<span style="color:#4d4d4d">그럼, 그 외에 문의사항은 [hello@cracker9.io](helloo@cracker9.io) 로 메일주세요!
크래커나인는 디자이너와 개발자들이 Creative에 집중할 수 있도록 돕겠습니다.

Cracker9 이 없다면 ▶ [클릭](http://cracker9.io/#skip-downloads)
Cracker9 으로 Custom Layout 를 만들어 보고 싶다면  ▶ [클릭](https://release.cracker9.io/code-snippet/artboards/090e6013-111a-4993-aec8-d9972d981a89/)

***

   ▶ Homepage: http://cracker9.io
   ▶ Blog: https://blog.cracker9.io
   ▶ Twitter: https://twitter.com/HelloCracker9
   ▶ Facebook: https://www.facebook.com/cracker9.io

***