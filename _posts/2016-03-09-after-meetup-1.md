---
layout: post
title: "Meetup #1 후기"
date: 2016-03-09 23:38:20 +0900
---

[Riiid!(뤼이드)][riiid]에서 [코틀린 코리아의 첫 미트업][meetup]을 마쳤습니다.

간단한 후기를 공유합니다.


# 1. 코틀린 소개 / 김상우(VCNC)

![1](https://cloud.githubusercontent.com/assets/1744446/13640505/4c33ee3e-e658-11e5-8540-ff1d82524467.jpg)

코틀린의 [공식 홈페이지][kotlinlang]를 탐험하시면서 문법을 훑어주셨습니다.

코틀린은 `Runtime`과 `stdlib`이 크지 않기 때문에
안드로이드에서는 다른 대안언어보다 코틀린이 좋다고 하셨습니다! :+1:

Java 서버개발하시는 분깨서 코틀린과 스칼라를 두고 뭐가 좋은지 질문하셨는데
서버사이드에서는 스칼라를 사용하는 입장에서 굳이 코틀린으로 해야할 이유를 모르겠다고 하셨습니다.

가장 좋은 학습 방법에 대해서도 설명해주셨는데 대략 아래와 같습니다.

- 공식 문서가 그리 어렵지 않다.
  - Java를 하신 분이라면 금방 익힐 수 있다.
- 인텔레제이에서는 Java코드를 붙여넣기하면 코틀린으로 변환할 것인지 물어본다.
  - 어떻게 변환됐는지 살펴보라.

> 참고로 Java코드를 변환하는 메뉴도 제공합니다. 인텔리제이의 `Code` 메뉴의 멘 아래쪽 즈음에 있습니다.


# 2. 코틀린과 렘(Realm) / 김용욱(Realm)

![2](https://cloud.githubusercontent.com/assets/1744446/13640506/4c3557e2-e658-11e5-83b1-d9f04c86cdd2.jpg)

모바일 데이터베이스인 Realm을 코틀린과 함께 사용하는 방법을 설명해주셨습니다.

> 참석하신 분들 중 반 이상이 렘을 사용하신다는?!!

들어가기에 앞서 [렘과 자바][realm-java]를 통해 sqlite보다 빠르고 간편한 사용방법을 간단히 소개를 해주셨고,
*안녕하세요 코틀린 시리즈*
[[1]][realm-kotlin-1], [[2]][realm-kotlin-2], [[3]][realm-kotlin-3] 중에서
[[2]][realm-kotlin-2]의 `객체 없는 함수`를 잠깐 언급해주셨습니다.

> 참고로 내용을 추가하자면 @JvmName 어노테이션을 이용하면
> 컴파일된 클래스 이름을 바꿀 수 있고, 자바에서 바꾼 이름으로 사용할 수 있습니다.  
> [Package-Level Functions][pkg-level-func]

오늘의 주제인 코틀린과 Realm을 함께 사용하는 방법은 [슬라이드][kotlin-with-realm]를 참고해주세요!
`Realm 0.88`부터는 `kapt`를 디펜던시에 걸지 않고(6페이지), 오직 플러그인만 설정하면 사용할 수 있다고 합니다.

> Gradle 플러그인으로 디펜던시를 신경 안쓸 수 있다는 꿀팁!  
> [Realm `0.88`][realm-0.88]이 곧 나온다고 쩌렁쩌렁 자랑하셨습니다. :joy:



# 3. Ready for Production / 허재위(Riiid!)

![3](https://cloud.githubusercontent.com/assets/1744446/13640507/4c3cc842-e658-11e5-92f2-a66c7d43d19a.jpg)

뤼이드의 안드로이드 프로덕션에서 코틀린과 함께 사용하고 있는 기술들에 대해서 설명해주셨습니다.

Github의 특정 계정의 저장소 목록을 불러와서
`Star`가 많은 순서로 목록을 보여주는 앱을 데모로 보여주셨고,
데모에 사용된 기술로는 코틀린과 함께 [Dagger2][dagger2], [RxAndroid][rx-android], [Retrofit2][retrofit],
[OkHttp3][okhttp], [Mockito][mockito]등이 사용되었습니다.

데모 소스및 자료는 [깃허브 페이지][ready-for-prod]를 참고하세요 :star:

> 혼자 안드로이드 개발하는 입장에서 이렇게 하는게 개발하는게 맞는지에 대한 의구심이 있다고 하십니다. :sweat:
> 피드백좀 주세요 :sob:


# 4. Talks

![4](https://cloud.githubusercontent.com/assets/1744446/13640508/4c4c2c10-e658-11e5-89cd-6c6f7f9492e3.jpg)

마지막으로 미트업의 꽃:tulip:인 개발자들끼리 수다를 떠는 시간을 가졌습니다.

생각보다 많은 분들이 늦게까지 남아서 *의도한대로!!!!!* 서로 이야기를 많이 나누어주셔서 감사했습니다.  
또한 스피커로 참여해주신 분들과, 뒤에서 도와주신 분들에게도 정말 감사드립니다! :bow:

이번에 함께하지 못한 분들이 많아서 좀 안타까웠는데,
자리가 또 마련되면 다음에는 꼭 함께할 수 있도록 노력하겠습니다. :smile:

**끝으로 못오신 분들을 위해 참석하신 분들의 후기도 공유해주시면 감사하겠습니다.**

다음에 봬요 :hand:






[riiid]: http://riiid.co/
[meetup]: http://www.meetup.com/kotlinkr/events/229274004/
[kotlinlang]: http://kotlinlang.org
[realm-java]: http://www.slideshare.net/dalinaum/realm-java
[realm-kotlin-1]: https://realm.io/kr/news/kotlin-1/
[realm-kotlin-2]: https://realm.io/kr/news/kotlin-2/
[realm-kotlin-3]: https://realm.io/kr/news/kotlin-3/
[kotlin-with-realm]: http://www.slideshare.net/dalinaum/a-brief-introduction-to-realm-with-kotlin
[ready-for-prod]: http://goo.gl/FIhEuK
[pkg-level-func]: https://kotlinlang.org/docs/reference/java-to-kotlin-interop.html#package-level-functions
[realm-0.88]: https://speakerdeck.com/realm/realm-model-classes-the-past-present-and-future-1
[dagger2]: https://github.com/google/dagger
[rx-android]: https://github.com/ReactiveX/RxAndroid
[android]: http://developer.android.com/
[retrofit]: https://github.com/square/retrofit
[okhttp]: https://github.com/square/okhttp
[mockito]: https://github.com/mockito/mockito
