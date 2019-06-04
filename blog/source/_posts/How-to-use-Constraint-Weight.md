---
title: Tutorial - Constraint Layout의 Weight 사용법
date: 2018-06-27 14:30:00
tags: 
- Android
- Layout
- Cracker9
categories:
- Tutorial
author: Cracker9
---
<span style="color:#4d4d4d">안녕하세요. 크래커나인 입니다.
이번에는 Cracker9 App으로 Constraint Layout 코드를 생성해보도록 하겠습니다.

<span style="color:#4d4d4d">지난번 Linear Layout에서 Weight를 사용하는 방법에 대해 다루면서 Linear와 Constraint에서 Weight를 사용하는 방법이 다르다고 언급했었습니다. 자, 그럼 Constraint Layout에서 Weight 입력을 어떻게 하는지 알아볼까요?
***
<span style="color:#4d4d4d">**STEP 01.** View Panel에서 Design Panel로 아이템을 끌어옵니다.

<span style="color:#4d4d4d">**STEP 02.** Constraint에서 Weight를 주기 위해서는 부모가 아닌 자식 View를 선택해야 합니다. 또한 자식 View를 전부 선택하는 것이 아닌, 원하는 View를 선택하여 가변영역이 필요한 부분에 설정할 수 있습니다. 가변영역이 필요한 자식 View를 Ctrl 키 or Command 키를 누르면서 멀티 선택 합니다.
![Constraint_W01](/img/HowToUseConstraintWeight/01.jpg?raw=true)
#  

<span style="color:#4d4d4d">**STEP 03.** 상단의 Design Tool bar에서 Weight_horizontal 버튼을 눌러주세요.
![Constraint_W02](/img/HowToUseConstraintWeight/02.jpg?raw=true)
#  

<span style="color:#4d4d4d">**STEP 04.** 그림과 같이 Weight 편집 모드 상태가 되면 가변이 필요한 숫자 box [114dp]를 클릭하여 화살표 모양으로 바꿔줍니다.
![Constraint_W03](/img/HowToUseConstraintWeight/03.jpg?raw=true)
#  

<span style="color:#4d4d4d">**STEP 05.** Save버튼을 눌러주세요.

<span style="color:#4d4d4d">**STEP 06.** 오른쪽 Setting Panel에서 Weight list에 Weight가 생성되었는지 확인합니다.
![Constraint_W04](/img/HowToUseConstraintWeight/04.jpg?raw=true)
#  

<span style="color:#4d4d4d">원래 코드로 Constraint에 Weight를 주기 위해서는 Chain된 상태에서 방향에 따라  layout_width, 또는 layout_height에 0dp를 줍니다.
<pre><code>android:layout_width="0dp"</code></pre><pre><code>android:layout_height="0dp"</code></pre>

<span style="color:#4d4d4d">그리고 weight를 설정해주면 weight 비율로 간격이 설정됩니다.
<pre><code>app:layout_constraintVertical_weight="1"</code></pre><pre><code>app:layout_constraintHorizontal_weight="1"</code></pre>

<span style="color:#4d4d4d">Cracker9에서는 이를  Weight를 입력하면 자동으로 Chain 속성 부여될 수 있도록 하였습니다. 그래서 weight를 입력 후 Chain으로 묶여진 것을 바로 확인 할 수 있습니다.
![Constraint_W05](/img/HowToUseConstraintWeight/05.jpg?raw=true)
#  

<span style="color:#4d4d4d">주황색으로 연결된 부분은 Chain으로 연결되어있다는 표시입니다. 본래는 Chain으로 연결되면 아래와 같이 표시되는데, 현재 보여드린 샘플은 간격사이가 좁아서 Chain 연결선까지는 보여지지는 않습니다. 만일 간격사이가 좁았다면 아래와 같이 연결선이 보여집니다.
![Constraint_W06](/img/HowToUseConstraintWeight/06.jpg?raw=true)
#  

<span style="color:#4d4d4d">**STEP 07.** Setting Panel 아래의 Generate Code 버튼을 선택해주세요.
![Constraint_W07](/img/HowToUseConstraintWeight/07.jpg?raw=true)
#  

<span style="color:#4d4d4d">**STEP 08.** Code Result Panel이 나오면 코드가 제대로 나왔는지 확인해주세요.
![Constraint_W08](/img/HowToUseConstraintWeight/08.jpg?raw=true)
#  

<span style="color:#4d4d4d">위의 과정을 담은 영상을 첨부하니 참고해주세요.
[![constraint_W09](/img/HowToUseConstraintWeight/v05.jpg?raw=true)](https://youtu.be/eVKLorgs12A)

<span style="color:#4d4d4d">그럼, 그 외에 문의사항은 [hello@cracker9.io](helloo@cracker9.io) 로 메일주세요!
크래커나인는 디자이너와 개발자들이 Creative에 집중할 수 있도록 돕겠습니다. <br><br>

Cracker9 이 없다면 ▶ [클릭](http://cracker9.io/#skip-downloads)
Cracker9 으로 Constraint Layout 의 Weight 사용 해보고 싶다면  ▶ [클릭](https://release.cracker9.io/code-snippet/artboards/23821565-f6e0-44a9-8928-f0bf15f98005)


_____
 <a href="http://www.cracker9.io?utm_medium=cpc&utm_source=blog_origin&utm_campaign=0.11.x&utm_content=How_to_use_Constraint_Weight" onclick="gtag('event', 'button click', {'event_category': 'Homepage','event_label': 'How to Use Constraint Weight'});">![cracker9](/img/Logo/Cracker9_Symbollogo.png?raw=true)</a>
_____
