# TypeScript quick start
Typescript 정적 파일 언어로 Javascript처럼 동적언어인 자바스크립트 상위집합의 개념으로 JAVA와 같은 언어처럼 타입을 선언하므로써, Type에러로 인한 사이드 이펙트를 사전에 방지 할 수 있습니다.
물론 개발을 함에 있어서 if문 등을 사용하는 쉴드 패턴을 이용해 이러한 이슈를 해결 할 수 있지만, 런타임에서 많은 오버해드를 줄일 수 있는 획기적인 방법입니다.
또한 interface 같은 Java와 C# 같은 상위언어에서 사용하는 객체지향 프로그래밍의 환경을 제공하고, class와 extends 같은 ES6의 자바스크립트를 지원하므로써, Javascript를 더욱 정적인 객체지향 프로그래밍을 하도록 도와줍니다.
Typescript로 개발을 하여 개발단계에서 사전 타입검사등을 진행하고, 빌드시 생성되는 자바스크립트 파일로 런타임을 하므로써 발생할 수 있는 이슈를 방지하고 오버해드를 최소화 할 수 있습니다.
Typescript는 타입스크립트 컴파일러를 통해 컴파일을 진행합니다.

``` text
컴파일링: 한 언어의 소스코드를 다른 언어로 변경하는것
트랜스파일링: 한언어의 소스코드를 비슷한 추상화 수준의 다른 언어로 바꾸는 것
```
Typescript는 다른언어인 Javascript로 변경하기 때문에 컴파일링이라고 할 수 있지만, 비슷한 추상화 수준의 언어로 트랜스파일링 한다고도 볼 수 있습니다.

## 컴파일 방법
``` text
tsc 파일명 // 기본은 ES3로 컴파일
tsc 파일명 -t 자바스크립트버전 // 해당 자바스크립트 버전으로 컴파일 -t는 --target의 약자
tsc 파일명 -watch // 해당파일을 감지하여 변경부분이 있으면 컴파일
```

## tsconfig.json
각 환경에 따라 typescript 컴파일에 대한 환경을 지정해 놓을 수 있다.

``` text
tsc --init // package.json 과 같이 명령어를 사용해 tsconfig.json파일을 생성
```

## 타입검사
정적타입검사 - JAVA, C++   // 컴파일 시점에 타입검사
동적타입검사 - Javascript  // 런타임 시점에 타입검사
점진적타입검사 - Typescript, python // 컴파일 시점에 타입검사 수행 및 타입 선언 생략 허용(자동 any타입)

