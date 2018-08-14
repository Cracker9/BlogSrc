---
title: Tutorial - Android view Center & Constraint Layout Bias 사용법
date: 2018-06-28 14:00:00
tags: 
- Android
- Layout
- Cracker9
categories:
- Tutorial
author: Cracker9
---
<span style="color:#4d4d4d">안녕하세요. 크래커나인 입니다.
Cracker9 사용은 익숙해지셨나요? 오늘은 Center와 Bias기능을 사용하여 코드를 생성하는 방법에 대해 알려드리도록 하겠습니다.

<span style="color:#4d4d4d">안드로이드 스튜디오에는 Centerㅍ속성을 코드로 작성할 수 있는데요.
Cracker9에서는 어떻게 Center 코드를 생성할수 있는지 그리고 어떤 상황에서 Bias 기능을 사용하는지 알아보도록 하겠습니다.
***
### 1. Linear Layout에서 Center
<span style="color:#4d4d4d">**STEP 01.** View Panel에서 아이템을 사용하여 Design Panel로 아이템을 끌어옵니다.
<span style="color:#4d4d4d">**STEP 02.** 부모 아이템을 선택 후 오른쪽 Setting Panel에서 Layout 값을 Linear Layout으로 설정합니다. Horizontal , Vertical 어떤 것이든 상관 없습니다.
![Center_01](/img/HowToUseCenterbias/01.jpg?raw=true)
#  

<span style="color:#4d4d4d">**STEP 03.** 지난번 Linear Layout 사용법에 대해 설명했을 때 Gravity와 Linear_Layout Gravity에 대한 얘기를 했었습니다. [Linear Layout 사용법 보러가기](https://cracker9.github.io/2018/06/27/How-to-use-Linear/)
<span style="color:#4d4d4d">**STEP 04.** 부모를 선택하시면 오른쪽 Setting Panel에서 Gravity의 메뉴를 선택하시면 Center, Center Horizontal, Center Vertical을 설정할 수 있습니다.
![Center_02](/img/HowToUseCenterbias/02.jpg?raw=true)
#  

![Center_03](/img/HowToUseCenterbias/03.jpg?raw=true)
#  

<span style="color:#4d4d4d">Center 입력시 부모 안에 포함된 View들이 수평+수직 가운데에 놓이게 되며
<span style="color:#4d4d4d">Center Horizontal 입력시 부모안에 포함된 View들이 수평 가운데에 놓이게 되며
<span style="color:#4d4d4d">Center Vertical 입력시 부모안에 포함된 View들이 수직 가운데에 놓이게 됩니다.
#  

<span style="color:#4d4d4d">**STEP 05.** 그리고 Linear Layout안에 있는 자식 아이템 선택 시 오른쪽 Setting Panel에서 Linear Layout_Gravity 메뉴를 선택하시면 되는데요. Linear Layout부모 방향이 Horizontal일 경우는 자식 아이템은 수직 방향으로만 설정할 수 있기 때문에 Center Vertical을, 부모 방향이 Vertical일 경우는 자식 이템은 수평 방향으로만 설정할 수 있기 때문에 Center Horiztontal을 선택할 수 있습니다.
![Center_04](/img/HowToUseCenterbias/04.jpg?raw=true)
#  

![Center_05](/img/HowToUseCenterbias/05.jpg?raw=true)
#  

### 2. Relative Layout에서 Center
<span style="color:#4d4d4d">**STEP 01.** View Panel에서 아이템을 사용하여 Design Panel로 아이템을 끌어옵니다.
<span style="color:#4d4d4d">**STEP 02.** 부모 아이템을 선택 후 Layout 값을 Relative로 변경합니다.
<span style="color:#4d4d4d">**STEP 03.** 부모 안에 포함되어 있는 자식 아이템을 선택해주세요.
<span style="color:#4d4d4d">**STEP 04.** 상단 Tool bar에서 Center 버튼을 선택해주세요. 이 때 Center Horizontal . Center Vertical 을 선택할 수 있는데, Center Horizontal을 선택해주세요.
![Center_06](/img/HowToUseCenterbias/06.jpg?raw=true)
#  

<span style="color:#4d4d4d">**STEP 05.** 그러면 좌/우 연결점들이 연결할 수 없는 상태로 변경되는데 이는 Center Horizontal로 연결되었기 때문입니다.
![Center_07](/img/HowToUseCenterbias/07.jpg?raw=true)
#  

<span style="color:#4d4d4d">**STEP 06.** 만약 Center Vertical을 입력하면 선택한 자식 아이템이 수직 방향 한 가운데로 이동하게 되며 상/하 연결점들이 연결할 수 없는 상태로 변경됩니다.
![Center_08](/img/HowToUseCenterbias/08.jpg?raw=true)
#  

### 3. Constraint Layout에서 Center
<span style="color:#4d4d4d">**STEP 01.** 부모 아이템을 선택 후 Layout 값을 Constraint로 변경합니다.
<span style="color:#4d4d4d">**STEP 02.** 부모안에 포함된 자식 아이템을 선택후 좌/우 연결점을 부모의 좌/우에 연결합니다.
![Center_09](/img/HowToUseCenterbias/09.gif?raw=true)
#  

<span style="color:#4d4d4d">**STEP 03.** 그러면 자동으로 Center가 입력됩니다. Constraint는 아이템을 선택하고 연결점을 연결해야만 Tool bar의 Center 버튼이 활성화 되는데요, 만약 좌/우로 연결했으면 Center_Horizontal로 상/하로 연결했으면 Center_Vertical로 설정됩니다. 그리고 Constraint도 Relative와 마찬가지로 Center 입력 시 자동으로 아이템의 위치가 이동하게 됩니다.
<span style="color:#4d4d4d">**STEP 04.** 나머지 텍스트 아이템도 Center로 연결합니다.
![Center_10](/img/HowToUseCenterbias/10.jpg?raw=true)
#  

### 4. Constraint Layout에서 Bias
<span style="color:#4d4d4d">**STEP 01.** Bias는 Constraint Layout에서만 사용할 수 있는 기능입니다. Constraint에서 하나의 아이템을 선택 하여 연결점을 좌/우로 연결했을 때 자동으로 Center로 설정됩니다. 하지만 만약 Center로 입력할 의도가 아니였다면 Bias로 바꾸어줘야 합니다.
![Center_11](/img/HowToUseCenterbias/11.gif?raw=true)
#  

<span style="color:#4d4d4d">**STEP 02.** 상단 Tool bar에서 Center 버튼 옆에 Bias 버튼을 눌러주세요.
![Center_12](/img/HowToUseCenterbias/12.jpg?raw=true)
#  

<span style="color:#4d4d4d">Bias도 Center와 마찬가지로 좌/우로 연결했을 때, Bias_Horizontal만 활성화되고 상/하로 연결했을 때 Bias_Vertical이 활성화 됩니다.
#  

<span style="color:#4d4d4d">**STEP 03.** Center로 설정되었던 아이템이 원래 제자리로 이동되면서 Bias 값이 설정됩니다.
![Center_13](/img/HowToUseCenterbias/13.gif?raw=true)
#  

<span style="color:#4d4d4d">**STEP 04.** Setting Panel 아래의 Generate Code 버튼을 선택해주세요.
![Center_14](/img/HowToUseCenterbias/14.jpg?raw=true)
#  

<span style="color:#4d4d4d">**STEP 05.** Code Result Panel이 나오면 코드가 제대로 나왔는지 확인해주세요.
![Center_15](/img/HowToUseCenterbias/15.jpg?raw=true)
#  

<span style="color:#4d4d4d">위의 과정을 담은 영상을 첨부하니 참고해주세요.
[![Center_16](/img/HowToUseCenterbias/v07.jpg?raw=true)](https://youtu.be/-9CXQIND5zw)

<span style="color:#4d4d4d">그럼, 그 외에 문의사항은 [hello@cracker9.io](helloo@cracker9.io) 로 메일주세요!
크래커나인는 디자이너와 개발자들이 Creative에 집중할 수 있도록 돕겠습니다.

***

   ▶ Homepage: http://cracker9.io
   ▶ Blog: https://blog.cracker9.io
   ▶ Twitter: https://twitter.com/HelloCracker9
   ▶ Facebook: https://www.facebook.com/cracker9.io

***