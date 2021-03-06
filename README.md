# AdFit Android SDK Guide

** Ver 3.0.3 **


### 꼭 읽어주세요!

AdFit SDK `v3.0.x` 은 기존 버전(v2.x.x)에 비해 클래스명, 내부 API 등 많은 부분이 변경되었습니다.

반드시 [SDK 연동 가이드](https://github.com/adfit/adfit-android-sdk/wiki)를 참고해 주시기를 부탁드립니다.

## Activity `onPause/onResume/onDestroy` 호출시, BannerAdView 의 `pause/resume/destroy` api 를 반드시 호출하지 않을 경우, 광고 수신에 있어 불이익을 받을 수 있습니다.

## Activity Context 이외의 Context 를 이용하여 BannerAdView 를 생성할 경우, 광고 SDK 가 이상동작을 할 수 있습니다.

---
이 가이드는 Android Application에 모바일 광고를 노출하기 위한 광고 데이터요청과 처리 방법을 설명합니다.

사이트/앱 운영정책에 어긋나는 경우 적립금 지급이 거절 될 수 있으니 유의하시기 바랍니다.

* 문의 고객센터 [https://cs.daum.net/question/1440.html](https://cs.daum.net/question/1440.html)
* 사이트/앱 운영 정책 [http://adfit.biz.daum.net/html/use.html](http://adfit.biz.daum.net/html/use.html)

이 문서는 Kakao 신디케이션 제휴 당사자에 한해 제공되는 자료로 가이드 라인을 포함한 모든 자료의 지적재산권은 주식회사 카카오가 보유합니다.

Copyright © Kakao Corp. All rights reserved.

---

