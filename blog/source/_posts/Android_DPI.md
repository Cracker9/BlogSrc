---
title: 초보 디자이너를 위한 안드로이드 DP(Dip), PX, DPI의 개념
date: 2018-03-13
tags: 
- Android
- Unit
- DPI
- PX
- DP
categories:
- Design
author: 구소희
---

## 안드로이드는 처음인데요
안드로이드를 처음 접하게 되면 DP, PX, Dpi이란 말을 듣게된다. 안드로이드는 다양한 스마트폰 화면 크기와 해상도를 지원하고 있기 때문에 필요한 개념이다. 처음에는 헷갈리기 쉽지만 생각보다 어렵지 않다. 그리고 이와 관련된 지식을 알고 있으면 디자인,개발 작업에 도움이 된다.

### 스크린의 실제 단위 PX
많이 들어봤을 법한 PX은 화면을 구성하는 최소 단위이다.
PX 단위는 화면의 전체 화면 크기와 상관없이 지정한 수치만큼 표시되는 절대적 표시 단위이므로 안드로이드에서는 PX보다는 DP 단위를 사용하면 좋다.
그 이유는 아래 DP단위 개념을 설명에서 알 수 있다.

### DPI
DPI는 Dot Per Inch로 1인치에 들어가는 픽셀을 나타내는 단위이다.
에를 들면 100DPI는 1인치당 픽셀이 100개 포함된다는 것을 말한다.
개수가 많을 수록 고밀도이며 안드로이드에서 주요 DPI는 아래와 같다.
* ldpi : 120dpi
* mdpi : 160dpi (기본)
* hdpi : 240dpi
* xhdpi : 320dpi
* xxhdpi : 480dpi
* xxxhdpi : 640dpi

안드로이드의 기준 DPI는 160 DPI이다.
160 DPI인 경우 밀도 독립단위 DP와 PX이 같은 크기를 갖는다.
즉, 16DPI에서는 1dp는 1px이 된다.

## 다양한 디바이스 크기에 대응하기 위해 필요한 DP
DP는 픽셀 독립 단위이다.
화면의 크기가 달라도 동일한 비율로 보여주기 위해 안드로이드에서 정의한 단위이며 큰 화면,작은 화면에 상관 없이 같은 크기로 나타난다.

![예시1](https://developer.android.com/images/screens_support/density-test-bad.png)
예시1) 같은 사이즈의 애플리케이션에 Low, Medium, High-density 화면에 PX 단위로 크기를 지정했을 때
![예시2](https://developer.android.com/images/screens_support/density-test-good.png)
예시2) 같은 사이즈의 애플리케이션에 Low, Medium, High-density 화면에 DP 단위를 지원했을 때

위의 예시들을 보면 안드로이드에서 왜 DP단위를 써야 하는지 알 수 있다

## 위의 개념들을 실무에 응용
DP, Px, DPI 실무에서 응용된다.
실제로 디자이너는 디자인 후 이미지를 보내줄때 해상도별로 Png파일을 보내줘야 하고 개발자도 리소스 파일을 해상도별로 관리해야 한다.
![해상도별 Png](https://github.com/sohee9/test_Doc/blob/master/%E1%84%89%E1%85%B3%E1%84%8F%E1%85%B3%E1%84%85%E1%85%B5%E1%86%AB%E1%84%89%E1%85%A3%E1%86%BA%202018-03-23%20%E1%84%8B%E1%85%A9%E1%84%8C%E1%85%A5%E1%86%AB%2011.50.00.png?raw=true)

## DP와 PX의 단위 변환
개발을 하다보면 DP를 PX로 바꿔줘야할 경우가 있다.
안드로이드 레이아웃을 코드 작성 할때 는 DP를 사용할 수가 없기 때문이다.
사용하는 공식은 아래와 같다.

* px = dp * 단말 DPI/기본 160
* dp = px * 기본 160/단말 DPI

mdpi 지원 단말일 경우 dpi는 160 이므로 1dp * 160/160 = 1pixel이 된다.
xxhdpi 지원 단말일 경우, 5dp를 pixel로 계산하면
5dp * 480/160 = 15 pixel 이므로 xxhdpi 단말의 5dp는 15pixel이 된다.

## 단위 변환을 계산해주는 도구
디자이너는 가이드를 작성할 때 DP계산이 필요하고 개발자는 코드를 작성할 때 PX 계산이 필요하다.
머릿속으로 계산이 빨리 되면 상관없겠지만, 일하면서 여간 쉬운 일은 아니다.(숫자에 약한 디자이너라면 더더욱...!) 그래서 계산이 힘든 사람들을 위해 작업 시간도 줄여주는 도구 몇가지 소개한다.

***

   ▶ Homepage: http://cracker9.io
   ▶ Blog: https://blog.cracker9.io
   ▶ Twitter: https://twitter.com/HelloCracker9
   ▶ Facebook: https://www.facebook.com/cracker9.io

***