---
title: 컴퓨터 공학도가 테스트해 본 크래커나인 사용기
date: 2018-12-05
tags: 
- 크래커나인
- Cracker9
- 업무 협업툴
- GUI가이드라인
- 안드로이드 앱개발
- 안드로이드스튜디오
- 크래커나인 사용성테스트
- 사용성테스트
- 크래커나인 사용기
- 크래커나인 사용후기
- 크래커나인 리뷰
- 크래커나인 제플린

categories:
- Interview

author: Cracker9

---

## **크래커나인 팀에는 크래커나인의 편의성을 올리기 위해 주니어 개발자들을 대상으로 사용성 테스트를 실시 하였습니다.**

##  

<span style="color:blue">**Cracker9 >** 본인 소개를 부탁드립니다.

**컴공학도 A >** 안녕하세요~ 저는 컴퓨터공학을 전공하고 있는 4학년 대학생 입니다.

**컴공학도 B >** 안녕하세요~ 저도 4학년 컴공학도 입니다.

##  

<span style="color:blue">**Cracker9 >** 안드로이드 개발은 얼마나 해보셨나요?

**컴공학도 B >** 저는 대학교 2학년 때부터 본격적으로 안드로이드 개발을 공부하였고, 현재는 디자인을 전공하는 학우들과 같이 App개발을 하면서 안드로이드에 대해 공부하고 있습니다.

**컴공학도 A >** 저도 스터디나 동아리에 참여하여 개발 공부를 하고 있습니다.

![](/img/Univ_Interview/0.png)

##  

<span style="color:blue">**Cracker9 >** App을 개발하고 있으시다고요? 그렇다면 GUI 정보는 어떻게 받아서 개발하시나요?

**컴공학도 B >** 처음에는 어떻게 전달받아야 할지 몰랐었는데, 디자인하는 분들이 Zeplin을 통해 GUI 가이드 정보를 주셔서 지금은 Zeplin을 사용하고 있습니다.

##  

<span style="color:blue">**Cracker9 >** 혹시 '크래커나인' 이라는 툴을 접해 본 적이 있었나요?

**컴공학도 A >** 아니요, 크래커나인 툴에 대해 몰랐어요.

##  

<span style="color:blue">**Cracker9 >** 크래커나인은 GUI 로 부터 코드를 생성해주는 툴 입니다.

**컴공학도 B >** 아이디어가 좋은데요? Zeplin으로 GUI 정보를 받아도 사실 개발할 때에는 직접 GUI 스펙을 기입하고, 코드로 일일이 짜는 것이 번거로운 일이었거든요.

#   

## **그럼, 크래커나인을 사용하여 Android View를 구성해보는 테스트를 진행하겠습니다.**
##   

![](/img/Univ_Interview/1.png)

<span style="color:blue">**Cracker9 >** 왼쪽에 보이는 View panel에서 원하는 View들을 선택하여 오른쪽의 Design panel 로 Drag & drop 하면 됩니다. 옮긴 후 맨 오른쪽 Setting tab에서 View의 ID 값, Layout, Size 등의 옵션을 설정하여 맨 오른쪽 하단의 Generate code를 선택하시면 Layout code가 추출됩니다.

##  

**컴공학도 B >** 보통 디자이너분들이 디자인하면 Margin 값이 있잖아요? 겉에서 Padding 으로 감싸면 그 값을 자동으로 잡아주면 좋을 것 같아요~

<span style="color:blue">**Cracker9 >** 기본적으로 Padding 이 잡혀있는 디자인이 있으면 Custom Layout 기능을 통해 감싸는 View를 생성하면 됩니다.

![](/img/Univ_Interview/2.gif)

**컴공학도 B >** 아하! 이런 방법이 있었군요! 좋은 기능이네요~ 다만 처음 사용하는 저 같은 사람에게는 이 아이콘을 보고, 이러한 기능이 있는지 인식이 잘 안되는게 아쉬워요.

#   

## **크래커나인을 충분히 테스트 해 본 후 인터뷰를 진행했습니다.**
##   
<span style="color:blue">**Cracker9 >** 크래커나인의 어떤 기능이 가장 편리했나요?

**컴공학도 A >** 연결을 클릭으로 하는 것은 되게 좋은 것 같아요. Android Studio 는 Drag 해서 작업하는게 불편했거든요.

##  

<span style="color:blue">**Cracker9 >** 클릭으로 연결하는게 Drag 보다 편리한가요?

**컴공학도 A >** 네, 작은 것 같은 경우 Drag 가 안되서 불편했었거든요.

**컴공학도 B >** Code 결과 창에 xml 로 다운 받을 수 있는 기능이 정말 편리 했습니다.

##  

<span style="color:blue">**Cracker9 >** 크래커나인에 있었으면 좋을 것 같은 기능이 있나요?

**컴공학도 B >** 개인적인 의견인데, String 이나 Color 외에도 Dimension 이라 해서 많이 쓰는 수치를 뽑아놓고 불러다 쓰거든요. 그것도 같이 만들어주는 기능이 있으면 좋겠어요. 또, 이미지 중에 이런 옵션도 있으면 좋겠어요. 해상도에 넘치는 부분이 있으면 잘라내라는 명령어가 있는데, 그런 것도 코드로 만들수 있었으면 좋겠어요.

**컴공학도 A >** Color 는 값만 있었으면 좋겠어요. 습관일수도 있는데 Mac 쓰다보면 확대 할때 패드로 하니까.. 습관의 문제니까 툴에 적응하면 괜찮을 것 같기도 해요.

##  

<span style="color:blue">**Cracker9 >** Zeplin 사용하다가 크래커나인 툴을 사용했을때 장단점 등 전반적인 느낌이 어떠셨나요?

**컴공학도 A >** 저처럼 안드로이드를 공부하거나 초보 개발자들에게는 좋을 것 같습니다. 저 또한 전반적으로 편리했구요. 다만, '시니어 개발자들은 직접 코드를 작성하는 것을 더 선호하시지 않을까?' 라는 생각이 드네요.

**컴공학도 B >** 단점이라기 보다 변경이 되었으면 하는 부분은 대부분 수치라는게 많이 쓰이지 않거든요. 꽉찬 영역들은 Match parent 로 많이 쓰니까 'Default 가 아예 Match parent 면 좋지 않을까?' 라는 생각이 들었어요. 그리고 제 생각으로는 Zeplin 보다 훨씬 더 편리한 툴인 것 같아요. 사실, Zeplin은 GUI 정보만 제공해주는 것에서 끝이지만 크래커나인은 Layout 코드까지 생성해주니까요. 개발의 효율성 면에서 휠씬 좋은 것 같아요. 실제로 스터디할 때 적극적으로 사용해보고 싶은 툴이에요.

_____

* Homepage_ <a href="http://www.cracker9.io?utm_medium=cpc&utm_source=blog_origin&utm_campaign=0.11.x&utm_content=Univ_Interview">http://cracker9.io</a>
* Facebook_ https://www.facebook.com/cracker9.io
_____
