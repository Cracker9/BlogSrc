---
title: 안드로이드 디자인 어셋 이름 가이드
date: 2018-04-01
tags: 
- Android
- Design
- Asset
categories:
- Design
author: 구소희
---

안드로이드 디자인을 할 때는 해상도에 따른 디자인을 하는 것이 중요하다. 하지만 실무에서는 디자인 작업 후에도 파일 전달에 있어 협업 부분도 중요하다. 사소한 부분에서 커뮤니케이션이 비효율적으로 발생하면 프로젝트 전체에 영향을 미치기도 한다. 오늘 올리는 글은 초보 디자이너들이 실무에서 놓치기 쉬운 디자인 어셋 이름 가이드에 관한 이야기이다.
*(다만 번역하여 올리는 글이라 정확하지 않을 수도 있습니다. 원문 링크를 첨부하니 어느 것이든 편하게 보시길 바랍니다.)*
[원본 보러가기](https://medium.com/@AkhilDad/a-designers-guide-for-naming-android-assets-f790359d11e5)
___
이 기사는 주로 궁금증이 많은 디자이너를 대상으로하며 초보 개발자는 물론 경험 많은 개발자가 이미 알고있는 글일 수도 있습니다.
이 디자이너가 만든 아름답고 창조적인 Asset을 Android OS가 선택하는 방법에 대한 통찰력을 제공합니다.
이 기사의 주된 목적은 개발자가 설계 방식에 따라 파일 이름 지정하거나,
폴더에 Asset을 배치하거 혹은 다른 방식으로 요구할 수 있기 때문에 개발자와 디자이너 사이의 간격을 좁히기 위해 작성하였습니다.

## 안드로이드가 당신의 App 디자인을 사용하는 방법:
안드로이드는 다양한 화면 크기와 해상도로 다양한 기기를 지원하므로 Asset이 다양한 DPI로 생성됩니다.
그리고 디자이너들은 주로 Asset을 xxxhdpi, xxhdpi, xhdpi, hdpi, mdpi, ldpi에 맞추어 만듭니다.

안드로이드가 다양한 DPI에 대해 어떻게 Asset을 선택 하는지 예제로 살펴봅니다.

### 예제
Add 아이콘이 있는 연락처 화면이 있습니다.
Add 아이콘에 대해 디자이너가 만든 Asset의 이름은 모두 DPI가 다른 add_icon.png 입니다.
이제 개발자가 알맞게 폴더에 넣으면 add_icon.png가 Android System에서 자동으로 선택됩니다. 폴더는 다음과 같습니다.

drawable-xxhdpi - xxhdpi의 add_icon.png
drawable-xhdpi - xhdpi의 add_icon.png
drawable-hdpi - hdpi의 add_icon.png
drawable-mdpi - mdpi의 add_icon.png
drawable-ldpi - ldpi add_icon.png

![1](https://cdn-images-1.medium.com/max/1600/1*S-QcwGET_Fw6kbAn-mfYLw.png)
*Drawable folders for assets in an app (ldpi is obsolete and not used nowadays)*

만약 DPI에 맞는 add_icon.png이라는 이름을 잊었거나 iPhone 용 Asset을 만들어서 add_icon.png/ add_icon@2x.png / add_icon@3x.png 등으로 이름을 지정 했을경우에는
Android에서 올바른 사용을 위해 모든 DPI에 맞는 add_icon.png로 이름으로 변경해야합니다.

따라서 개발자는 모든 해상도에 맞춰 add_icon.png의 이름을 변경해야 하지만 게으른 개발자는 별다른 신경을 쓰지 않고 폴더에 Asset을 전부 넣을 수 있습니다.
만일 Android에서 add_icon.png을 요구하면 시스템에서 add_icon.png의 크기를 조정하고 모든 디바이스에 단일 크기로 표시합니다.
그렇게 되면 당신의 디자인이 좋아 보이지 않을 것입니다.

그렇다면 디자이너는 어떻게 해야 할까요?
Android에서 원하는 Asset 이름 규칙을 배워봅시다.
DPI가 다른 폴더를 만들어 폴더에 "add_icon.png"라는 이름의 다른 버전의 add_icon.png을 배치하십시오.

## Android Asset 이름 규칙:
Asset이름은 APP의 고유한 이름으로 결정할 수 있지만 다음 사항을 염두에 두어야합니다.
1. 유효한 문자 세트는 [ a-z / _ / 0-9 ] 즉 모든 소문자, 숫자 및 밑줄 입니다.
2. Asset 이름의 첫 글자는 _ (밑줄) 또는 작은 대소 문자를 사용하며 숫자는 첫 글자가 될 수 없습니다.
3. 이미지 확장자가 .PNG 또는 .JPG와 같은 경우에는 대문자를 사용하지 마십시오.
4. -(하이픈)과 공백을 사용할 수 없기 때문에 두 단어를 구별 할 때는 구분 기호로 _ (밑줄) 을 사용하십시오.
5. Asset 이름은 App에서 화면 전체에서 고유해야 합니다.
   또한 크기가 다른 두 개의 추가 버튼이 있는 경우 두 가지 이름을 모두 add_icon.png로 지정할 수 없습니다.
   add_icon_small.png 및 add_icon_big.png와 같은 두 가지 아이콘을 DPI로 만들어야 합니다.

## 팁:
디자인 팀에서 Aseet이름 규칙을 설정하면 누구나 동일한 규칙을 따라야합니다.
좋은 Asset 이름 규칙은 다음과 같습니다.
1. ic - 모든 아이콘의 접두어
2. bg - 모든 배경에 대한 접두어
3. selected - 선택된 상태의 접미사
4. pressed - 눌려진 상태의 접미사 등등..

##### 예제
1. ic_asset_name
2. ic_asset_name_pressed
3. ic_asset_name_selected
4. ic_asset_name_disabled
5. ic_asset_name_activated
6. bg_splash

## 그리고 다음과 같이 개발자에게 요구하세요.
1. 당신이 이미지를 자르는 것은 당신이 이미 자른 이미지를 회전시키는 것 뿐이니 치수는 동일합니다. 아이콘을 갖고 있고 개발자가 아이콘을 원한다면 개발자가 코드를 통해 회전 시키도록 요청하십시오.
2. App에 평면 색상 (단색 색상의 그라데이션 없음) 아이콘이 포함되어 있고 색상을 다르게 하고 싶으면 개발자에게 대신 부탁하세요.
3. Gradient 이미지도 있습니다. 타원형, 직사각형, 둥근 사각형, 정사각형과 같은 기본적인 모양이 아니라면 색상 코드를 제공 할 수 있습니다. 방사형, 선형 및 원형 Gradient도 만들 수 있으므로 걱정하지 마십시오.
4. 테두리가 있는 Button과 기본 그림자도 만들 수도 있습니다. 또한 9patch, 패턴, 그리고 평면 Asset을 사용하도록 강요하십시오.

#### 몇 가지 추가 정보
* 색상에 대해 rgb 값보다 16 진수 코드를 제공하십시오.
* App에 대한 하나의 폴더를 만들고 그 폴더에 지원하는 모든 Dpi폴더를 만든 다음 모든 팀원은 해당 폴더에 컷아웃을 배치해야합니다.
  따라서 이미 누군가 add.png 파일을 만든 경우 add.png를 다시 만들려고하면 모두에게 대체 경고가 표시됩니다.

_____

* Homepage_ http://cracker9.io
* Blog_ https://blog.cracker9.io
* Facebook_ https://www.facebook.com/cracker9.io

_____