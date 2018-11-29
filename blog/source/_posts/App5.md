---
title: 안드로이드 디자이너와 개발자를 위한 놀라운 안드로이드 앱 5가지
date: 2018-03-20
tags: 
- Android
- App
categories:
- Design
author: 구소희
---


이 글은 안드로이드 개발자 이자 Medium에서 글을 연재 중인 Antonis Tsagaris의 글을 번역한 글 입니다.
원제 : 5 Amazing Android Apps for Android Developers & Designers - A list of my favorites
*(번역이 정확하지 않을 수도 있습니다. 원문 링크를 첨부하니 어느 것이든 편하게 보시길 바랍니다.)*
[원본 보러가기](https://hackernoon.com/5-amazing-android-apps-for-android-developers-designers-4678b8d231b4)

## 작업을 도와주는 앱
안드로이드 개발자로서 우리는 대부분 소비자를위한 앱을 만듭니다. 하지만 다른 개발자를위한 앱을 만드는 놀라운 개발자도 있다는 사실을 잊지 말아야 합니다.
소개하려는 다섯 가지 응용 프로그램은 Pixel XL의 'Developer'폴더에서 곧바로 나옵니다. (그만큼 자주 쓰는 앱이라는 뜻)
그 폴더에 있는 유일한 앱은 아니지만 내 작업 환경에서 없어서는 안되는 앱 입니다.

### Termux
아, Termux....! Termux가 얼마나 멋진지 대해서 전체 기사를 썼습니다.
오, 곧장 소개할테니 기다려보세요.

[Termux 소개 원문 글](https://hackernoon.com/how-termux-saved-my-ass-73db53b2dea1)

Termux는 패키지 관리자, 테마 기능, Floating Widget-모든 mod cons을 갖춘 Linux 터미널 에뮬레이터입니다.
다운로드 할 수있는 패키지 목록이 많으며

```
apt-get install {package name}
```

제가 어떻게 사용하냐구요? Termux를 사용하여 2013 Nexus 7에서 내 앱 중 하나에 대한 경량급 node.js 푸시 알림 서버를 실행했습니다.
즉, Node.js, Express 및 다양한 Node_module을 Termux에 설치 해야함을 의미합니다. 이는 사소한 일이었습니다.

어제, TypeScript 컴파일러를 설치하고 싶었습니다. 왜냐하면 제가 배운 연습용 JavaScript를보고 싶었기 때문입니다.
저는 순신간에 낙담했습니다.

```
apt-get install tsc
```

npm을 통해 TypeScript 패키지를 설치하는 것이 비법이었다는 것을 깨달을 때까지 아무런 요령도 피우지 못했습니다.

![1](https://cdn-images-1.medium.com/max/1600/1*tBFbouwQajh8WpowZsMyDQ.png)

[Termux is free in the Play Store](https://play.google.com/store/apps/details?id=com.termux)
추가 기능 중 일부는 유료이지만, 그것은 돈주고 살만합니다.

[Buy Antonis Tsagaris a Coffee - BuyMeACoffee.com](https://www.buymeacoffee.com/XozUExS)

### Screener
이제 앱을 만들어 Play 스토어에 게시하려고 합니다.
앱스토어 목록에서 멋지게 보이게하려면 어떻게 해야할까요? 디바이스 프레임에 스크린샷을 넣으면 됩니다.

Screener를 사용하면 많은 양의 디바이스 프레임을 다운로드하고 스크린 샷을 배치 할 수 있습니다.
화면의 채광 효과와 디바이스 뒤의 그림자를 추가하여 멋져 보이게 할 수 있습니다. 또한 생성 된 배경은 스크린 샷 자체를 기반으로 채색됩니다.

Screener을 사용하기 전
![2](https://cdn-images-1.medium.com/max/1600/1*PlpM5tdXAuzAuda056hkFA.png)

Screener를 사용한 후 ![3](https://cdn-images-1.medium.com/max/1600/1*20YRIJrC5_S7BV9gbtFUTQ.png)

[Screener Play is free in the Play Store](https://play.google.com/store/apps/details?id=de.toastcode.screener)

### Material Cue
Material Design Guidelines를 존중한다면 Material Cue가 필요할 것입니다.
Google은 Material Cue가 필요하지 않습니다.
그러나 당신은 필요로 할 것 입니다.
![4](https://cdn-images-1.medium.com/max/1600/1*r8b3FnWP5YxsRGKeL-7Xcw.png)

Material Cue에서 격자 오버레이를 선택하면 요소의 배치를 확인할 수 있습니다. Navigation Drawer 요소, FAB 위치 지정 등과 같은 것들을 위해 이 기능은 매우 중요합니다.

[Material Cue is free in the Play Store](https://play.google.com/store/apps/details?id=com.actinarium.materialcue&hl=en)

### Graphice
Graphice는 개발자 중의 개발자 Francisco Franco가 만든 놀랍고 아무도 흉내낼수 없는 색상 추출 도구입니다.
파시스트의 독재자로서의 짧은 기간 이후 (너무 이른 것일까? 아마 그렇지는 않음), Francisco는 화려한 안드로이드 앱을 만들어서 자신을 구하기로 결정했고, Graphice는 대히트의 최신작이다.

Palette API가 출시 된 이래로 색상 추출 앱은 Play 스토어에서 10 페니(심지어 나는 하나의 균열이 있었다.)이지만 Graphice가 가장 좋은 앱입니다. 제가 만든 것보다 낫습니다. 젠장.

Graphice가 제가 만든 비슷한 응용 프로그램을 보지 못했다는 점은 사진에서 팔레트를 추출 할 영역을 선택할 수 있다는 것입니다.
또한 각 사진에서 추출 할 색상 수를 지정할 수 있습니다.

![5](https://cdn-images-1.medium.com/max/1600/1*e5Rm-zGBvAzoe9mRB6WWQg.png)

따라서 당신이 다음 앱을 위한 아주 좋은 색상 팔레트를 찾고 있다면 무엇을 써야 하는지 알겠죠?

[Graphice is free in the Play Store](https://play.google.com/store/apps/details?id=com.franco.graphice&hl=en)
합리적인 $2.49 IAP로 일부 프리미엄 기능을 사용할 수 있습니다.

### Pocket Casts
여기 팟 캐스트 앱은 무엇입니까?
당신은 Fragments와 Android Developer Backstage를 자연스럽게 구독 할 수 있습니다.

이들은 매우 지식이 풍부하고 숙련된 사람들이며 지루할 틈이 없습니다.
추가 권장 사항 : Android 팟 캐스트 중에 Beef & Dairy Network podcast 팟 캐스트를 듣고 싶어한다면, 꼭 들어보세요.
![6](https://cdn-images-1.medium.com/max/1600/1*ylOn9g5005lmEXVSNw-Jxw.png)

[Pocket Casts costs a very reasonable $3.99 in the Play Store.](https://play.google.com/store/apps/details?id=au.com.shiftyjelly.pocketcasts&hl=en)

### 칭찬할만한 언급 : AIDE
AIDE. 어떻게 저의 마음을 아프게 할 수 있나요

이동 중에 Android 앱을 코딩 할 수 있는 경량의 멋진 앱이었을 때는 AIDE를 사랑했습니다.

그리고 그들은 Everglaze에 있는 1주일 넘은 시체를 부풀게 하기로 결정했습니다. (저는 CSI : Miami를 많이 보곤했습니다.) 충성스러운 모든 사용자들을 실망시켰습니다.
*(그 뒤 문장이 번역이 안되는데, 잘 쓰고 있던 앱이 더이상 서비스를 제공하지 않는다는 말을 전하고 있다.)*

![7](https://cdn-images-1.medium.com/max/1600/1*k4b8_2XcQTtCZv-tqnnm6g.png)
AIDE는 Play 스토어의 모든 서비스에 연결되지 않습니다. 젠장.

_____

* Homepage_ http://cracker9.io
* Blog_ https://blog.cracker9.io
* Facebook_ https://www.facebook.com/cracker9.io

_____