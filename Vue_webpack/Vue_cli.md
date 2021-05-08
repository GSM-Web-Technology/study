## Vue CLI 초기 세팅

### Vue CLI

> Vue Cli는 프로젝트를 개발할 수 있게 해주는 유용한 도구이다.  
> CLI란 Command Line Interface의 약자로서 타이핑으로 명령어를 입력하여 원하는 명령을 실행시키는 도구를 말한다.  
> Vue CLI로 명령을 실행시키면 자동으로 최적화된 webpack 형태의 결과물을 생성 시켜준다.

### Vue CLI 2.x 와 Vue CLI 3.x 버전 비교

#### 프로젝트 생성

- **CLI2** : eslint, unit test, night watch 등 낯선 것들 선택 필요
- **CLI3** : default (babel,eslint)를 선택하면 가장 기본적인 설정으로 프로젝트 생성(나중에 옵션을 추가 가능하다)

### 프로젝트 구성

- CLI2 : simple, webpack, webpack-simple, pwa 등 템플릿 리스트 중 하나를 선택해서 프로젝트 구성
- CLI3 : 프로젝트에 플러그인 기반으로 원하는 설정 추가

### 웹팩 설정 파일

- CLI2 : `webpack.config.js`파일이 최상단 디렉터리에 있다.
- CLI3 : root 디렉터리에 `vue.config.js`파일을 설정하고 내용 추가

### node modules

- CLI2 : 자동 설치 X `$npm install` 필요
- CLI3 : 자동 설치 O

### 설치 환경

- node.js
- npm

### CLI 설치

```shell
$ npm i -g vue-cli // vue-cli 2.x
$ npm i -g @vue/cli // vue-cli 3.x
```

### 버전 확인

```shell
$ vue -- version
```

### 프로젝트 생성

> babel과 eslint 기반인 default 옵션을 선택한다.

```shell
$ vue init webpack 'ProjectName' // vue-cli 2.x
$ vue create 'ProjectName' // vue-cli 3.x
```

### 로컬 서버 실행

```shell
$ npm run dev // vue-cli 2.x
$ npm run serve // vue-cli 3.x
```

`http://localhost:8080/`에 들어가면 로컬 페이지를 볼 수 있다.  
vue cli의 기본 템플릿은 babel, eslint, unit-mocha를 포함한다.

> - **Babel** : 자바스크립트 컴파일러다. 최신버전의 자바스크립트 문법은 브라우저가 이해하지 못하기 때문에 Babel은 이 브라우저가 이해할 수 있는 문법으로 변환시켜준다.
> - **ESLint** : 코딩 스타일 가이드를 따르지 않거나 문제가 있는 코드, 안티 패턴을 찾아 표시를 달아 놓는 도구이다.
> - **unit-mocha** : 자바스크립트 진영에서 테스트 러너를 지원하는 테스트 프레임워크이다.
