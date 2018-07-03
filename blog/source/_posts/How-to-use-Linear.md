---
title: Tutorial - Linear Layout 사용법
date: 2018-06-26 10:21:10
tags:
- Android
- Cracker9
categories:
- Cracker9 Story
author: 구소희
---
<span style="color:#4d4d4d">안녕하세요. 크래커나인 입니다.
이번에는 Cracker9 App으로 Linear Layout 코드를 생성해보도록 하겠습니다.
***
### 1. Cracker9에서 사용
<span style="color:#4d4d4d">**STEP 01.** 레이아웃을 구성해야하는 View들을 왼쪽에 있는 View Panel에서 선택합니다. 이 때 Shift를 누르고 선택을 원하는 영역을 드래그 하거나 Ctrl (혹은 Command)를 누르고 View를 하나씩 선택해주세요.
![Linear01](/img/HowToUseLinear/01.jpg?raw=true)
#  

<span style="color:#4d4d4d">**STEP 02.** 선택된 View를 오른쪽에 있는 Design Panel로 끌어옵니다.
![Linear02](/img/HowToUseLinear/02.gif?raw=true)
#  

<span style="color:#4d4d4d">**STEP 03.** 오른쪽 사이드에 있는 Setting Panel에서 View를 감싸는 최상위의 Layout을 Linear Horizontal로 설정합니다. Cracker9에서 기본으로 설정되는 Layout은 Constraint이기 때문입니다.
![Linear03](/img/HowToUseLinear/03.jpg?raw=true)

<span style="color:#4d4d4d">Linear Layout이 자식 View를 나열하는 방향은 Horizontal과 Vertical 2가지로 나뉘는데요.
Cracker9의 Linear Layout은 2가지 중 1가지를 선택할 수 있습니다. Tutorial의 샘플은 자식 view들이 수평적으로 정렬되기 때문에 Linear Horizontal로 설정해주세요.
#  

<span style="color:#4d4d4d">**STEP 04.** Gravity는 현재의 View 안에 있는 내용들을 어디에 놓을 것인지를 지정하는 속성이고, layout_gravity는 부모 View 안에서 자식의 View를 어디에 놓을 것인지를 지정하는 속성입니다.
그래서 Cracker9에서는 부모 View를 선택하면 ‘android:gravity’ 속성을 설정할 수 있고, 자식 View를 선택하면 ‘android:layout_gravity’ 속성을 설정 할 수 있습니다.
#  

![Linear04](/img/HowToUseLinear/04.jpg?raw=true)
![Linear05](/img/HowToUseLinear/05.jpg?raw=true)
#  

<span style="color:#4d4d4d">이 샘플에서 Gravity가 꼭 필요하진 않으니 설정하지 않아도 됩니다.
#  

<span style="color:#4d4d4d">**STEP 05.** Setting Panel 아래의 Generate Code 버튼을 선택해주세요.
![Linear06](/img/HowToUseLinear/06.jpg?raw=true)
#  

<span style="color:#4d4d4d">**STEP 06.** Code Result Panel이 나오면 코드가 제대로 나왔는지 확인해주세요.
![Linear07](/img/HowToUseLinear/07.jpg?raw=true)
#  

### 2. Android studio에서 사용
<span style="color:#4d4d4d">자 이제 거의 다 왔습니다. 생성된 코드를 안드로이드 스튜디오에서 사용하는지 알아볼까요?

<span style="color:#4d4d4d">**STEP 01.** Code Result Panel에서 Copy 버튼을 선택 해주세요.
![Linear08](/img/HowToUseLinear/08.jpg?raw=true)
#  

<span style="color:#4d4d4d">**STEP 02.** 안드로이드 스튜디오 xml에 Ctrl + V하여 코드를 붙여넣기 합니다.
![Linear09](/img/HowToUseLinear/09.jpg?raw=true)
#  

<span style="color:#4d4d4d">**STEP 03.** 코드에서 빨간색 글씨가 나온다면, 해당하는 리소스 파일이 폴더에 없기 때문에 표시되는 것입니다. Cracker9에 drawable 리소스가 생성 되었으니 안드로이드 스튜디오에도 draw xml을 생성합니다.
![Linear10](/img/HowToUseLinear/10.jpg?raw=true)
Cracker9에서 draw1의 Copy버튼을 눌러서 코드를 복사해주세요.
#  

<span style="color:#4d4d4d">**STEP 04.** 안드로이드 스튜디오로 넘어와서  project 패널 > app > res > drawable을 선택하고 마우스 오른쪽을 클릭하세요. 아래와 같이 drawable 리소스 파일을 생성해줍니다.
![Linear11](/img/HowToUseLinear/11.jpg?raw=true)
#  

<span style="color:#4d4d4d">**STEP 05.** 아래의 창에 xml이름을 입력합니다. 이때 Cracker9에서 생성된 draw이름과 동일해야 합니다.
![Linear12](/img/HowToUseLinear/12.jpg?raw=true)
#  

<span style="color:#4d4d4d">**STEP 06.** draw xml이 drawable 폴더에 맞게 생성되었는지 확인해주세요.
![Linear13](/img/HowToUseLinear/04.jpg?raw=true)
#  

<span style="color:#4d4d4d">**STEP 07.** 아까와 같이 Ctrl+V 하여  draw 코드를 붙여넣기 해주세요.
![Linear14](/img/HowToUseLinear/14.jpg?raw=true)
#  

<span style="color:#4d4d4d">**STEP 08.** Color 리소스는 좀 더 쉽습니다. Project 패널에 이미 나와있는 color xml을 더블클릭하여 오픈 후 Cracker9에서 Color코드를 복사하여 붙여넣기 해주세요.
![Linear15](/img/HowToUseLinear/15.jpg?raw=true)

Color에 다른 코드가 작성되어 있다면, Cracker9에서 필요한 코드만 마우스로 드래그하여 복사하고 붙여넣기 할 수 있습니다.
![Linear16](/img/HowToUseLinear/16.jpg?raw=true)
#  

<span style="color:#4d4d4d">**STEP 09.** 마지막으로 Asset을 넣어보도록 하겠습니다.
Cracer9 App 상단에 보시면 Asset을 다운로드 할 수 있는 버튼을 선택한 후 폴더를 지정하여 다운로드 합니다.
![Linear17](/img/HowToUseLinear/17.jpg?raw=true)
#  

<span style="color:#4d4d4d">**STEP 10.** 다운로드 된 파일을 확인 후 해상도에 맞는 Asset 파일들을 선택합니다. 그리고 안드로이드 스튜디오에서 생성한 프로젝트의 drawable 리소스 폴더로 이동해주세요.
![Linear18](/img/HowToUseLinear/18.jpg?raw=true)
#  

<span style="color:#4d4d4d">**STEP 11.** 안드로이드 스튜디오 프로젝트에 Asset 리소스가 자동으로 올라오게 됩니다.
![Linear19](/img/HowToUseLinear/19.jpg?raw=true)
#  

<span style="color:#4d4d4d">이것으로 Linear Layout을 사용하는 방법과 생성된 코드를 안드로이드 스튜디오에서 어떻게 사용하는지 알아 보았습니다. 생성된 코드를 사용하는 방법은 모두 동일합니다. Cracker9을 사용하여 코드를 쉽고 빠르게 생성하고 레이아웃을 완성해보세요.
#  

<span style="color:#4d4d4d">위의 과정을 담은 영상을 첨부하니 참고해주세요.
[![Linear20](/img/HowToUseLinear/v01.jpg?raw=true)](https://youtu.be/mLO5JiA3y-U)
***
<span style="color:#4d4d4d">그럼, 그 외에 문의사항은 [hello@cracker9.io](helloo@cracker9.io) 로 메일주세요!
크래커나인는 디자이너와 개발자들이 Creative에 집중할 수 있도록 돕겠습니다.
