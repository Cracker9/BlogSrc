---
title: Tutorial - Constraint Layout 사용법
date: 2018-06-27 12:00:00
tags: 
- Android
- Layout
- Cracker9
categories:
- Tutorial
author: Cracker9
---
<span style="color:#4d4d4d">안녕하세요. 크래커나인 입니다.
오늘은 Constraint Layout을 사용하여 코드를 생성해보도록 하겠습니다.
***
### 1. Constraint Layout 소개
<span style="color:#4d4d4d">Constraint Layout은 2016년 Google I/O에서 처음 소개되었습니다. Constraint Layout이라는 개념은 개발자가 인터페이스를 더욱 풍부한 표현 방식으로 개발할 수 있도록 제공하기 시작했습니다.
더 정확한 Constraint Layout에 대한 설명은 이곳을 참고해주세요.
[참고 사이트](https://developer.android.com/reference/android/support/constraint/ConstraintLayout)
#  

### 2. Cracker9에서 관계맺기 방법
<span style="color:#4d4d4d">관계 맺는 방법은 지난번 설명했던 Relative에서 관계 맺기와 동일 합니다.

<span style="color:#4d4d4d">**STEP 01.** View Panel에서 Constraint로 코드를 구성할 View를 선택 후 Design Panel로 옮겨줍니다.
![Constraint00](/img/HowToUseConstraint/00.gif?raw=true)
#  

<span style="color:#4d4d4d">**STEP 02.** 부모 안에 포함된 첫번째 View를 선택하세요. 그리고 View의 왼쪽을 부모의 왼쪽과 연결해주세요.
![Constraint01](/img/HowToUseConstraint/01.jpg?raw=true)
#  

<span style="color:#4d4d4d">**STEP 03.**. View의 상단을 부모의 상단과 연결합니다.
![Constraint02](/img/HowToUseConstraint/02.jpg?raw=true)
#  

<span style="color:#4d4d4d">**STEP 04.** 두번째 View을 선택 후 View의 왼쪽을 첫번째 View의 왼쪽과 연결합니다.
![Constraint03](/img/HowToUseConstraint/03.jpg?raw=true)
#  

<span style="color:#4d4d4d">**STEP 05.** 두번째 View의 상단을 첫번째 View의 하단과 연결합니다.
![Constraint04](/img/HowToUseConstraint/04.jpg?raw=true)
#  

<span style="color:#4d4d4d">**STEP 06.** 세번째 View를 선택 후 부모의 상단과 연결합니다. 그 후 하단을 부모의 하단과 연결하여 Center로 만들어줍니다.
![Constraint05](/img/HowToUseConstraint/05_1.jpg?raw=true)
![Constraint05](/img/HowToUseConstraint/05_2.jpg?raw=true)
#  

<span style="color:#4d4d4d">**STEP 07.** 세번째 View의 오른쪽을 네번째 View의 왼쪽과 연결합니다.
![Constraint06](/img/HowToUseConstraint/06.jpg?raw=true)
#  

<span style="color:#4d4d4d">**STEP 08.**
네번째 View를 선택 후 부모의 상단과 연결합니다. 그 후 하단을 부모의 하단과 연결하여 Center로 만들어줍니다.
![Constraint07](/img/HowToUseConstraint/07_1.jpg?raw=true)
![Constraint07](/img/HowToUseConstraint/07_2.jpg?raw=true)
#  

<span style="color:#4d4d4d">**STEP 09.** 네번째 View의 오른쪽을 부모의 오른쪽과 연결합니다.
![Constraint08](/img/HowToUseConstraint/08.jpg?raw=true)
#  

<span style="color:#4d4d4d">**STEP 10.** 전부된 연결된 모습은 아래와 같습니다.
![Constraint09](/img/HowToUseConstraint/09.jpg?raw=true)
#  

<span style="color:#4d4d4d">**STEP 11.** 더 정확한 이해를 돕기 위해 영상을 첨부했습니다.
[![Constraint14](/img/HowToUseConstraint/v04.jpg?raw=true)](https://youtu.be/hs54q9w5Vi0)  
#  

<span style="color:#4d4d4d">**STEP 12.** Constraint Layout도 마찬가지로 View끼리 서로 연결된 결과는 각각 View를 선택해도 확인할 수 있으며, 더 자세한 사항은 오른쪽 Setting Panel > Relation에서도 확인 할 수 있습니다. 이때 방향 값은 Relative와 다르게 표현됩니다.
![Constraint11](/img/HowToUseConstraint/11.jpg?raw=true)
#  

<span style="color:#4d4d4d">**STEP 13.** Setting Panel 아래의 Generate Code 버튼을 선택해주세요.
![Constraint12](/img/HowToUseConstraint/12.jpg?raw=true)
#  

<span style="color:#4d4d4d">**STEP 14.** Code Result Panel이 나오면 코드가 제대로 나왔는지 확인해주세요.
![Constraint13](/img/HowToUseConstraint/13.jpg?raw=true)
#  


<span style="color:#4d4d4d">그럼, 그 외에 문의사항은 [hello@cracker9.io](helloo@cracker9.io) 로 메일주세요!
크래커나인는 디자이너와 개발자들이 Creative에 집중할 수 있도록 돕겠습니다.

Cracker9 이 없다면 ▶ [클릭](http://cracker9.io/#skip-downloads)
Cracker9으로 Constraint Layout 을 구성 해 보고 싶다면  ▶ [클릭](https://release.cracker9.io/code-snippet/artboards/e7916c1c-0fbb-4df1-a323-fc8a3ef48db4)

_____
 <a href="http://www.cracker9.io?utm_medium=cpc&utm_source=blog_origin&utm_campaign=0.11.x&utm_content=How_to_use_Constraint" onclick="gtag('event', 'button click', {'event_category': 'Homepage','event_label': 'How to Use Constraint'});">![cracker9](/img/Logo/Cracker9_Symbollogo.png?raw=true)</a>
_____
