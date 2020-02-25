Ionic + Angular + Android
```
0.	정의
Ionic이란?
Cordova 기반 하이브리드 앱 개발 프레임워크

1.	Node.js 설치
https://nodejs.org/en/
올바르게 설치되었다면, CMD 창에서 npm -v와 node -v 명령어가 실행됩니다.

2.	Typescript 설치
npm install typescript -g

3.	Cordova와 ionic 설치
npm install -g @ionic/cli native-run cordova-res
npm install –g ionic cordova

4.	Angular 설치
npm install –g @angular/cli

5.	프로젝트 생성
ionic start myApp tabs --type=angular –capacitor

6.	프로젝트 폴더로 들어갑니다.
cd myApp

7.	프로젝트를 실행합니다.
ionic serve
ionic serve –lab (IOS, Android 두개의 화면을 동시에 볼수있습니다.)

5. JAVA 세팅
5.1 JDK를 다운받아, 설치합니다.
5.2 시스템 변수를 설정합니다. 
JAVA_HOME (EX : C:\java-13-openjdk\java-13-openjdk-13.0.1.9-2.windows.ojdkbuild.x86_64)
5.3 Path에 추가합니다.
%JAVA_HOME%\bin
(위로 이동 버튼으로 리스트 항목의 가장 위로 올립니다.)
5.4 올바르게 설정되었다면, CMD 창에서 java와 javac 명령어가 실      
행됩니다.



6. 안드로이드 세팅
1. 안드로이드 스튜디오를 설치합니다.
https://developer.android.com/studio/?hl=ko

2. 시스템 변수에서 새롭게 추가합니다.
ANDROID_SDK_ROOT
C:\Users\(사용자 이름)\AppData\Local\Android\Sdk
3. Path에 추가합니다.
%ANDROID_SDK_ROOT%\tools\bin
%ANDROID_SDK_ROOT%\platform-tools
%ANDROID_SDK_ROOT%\emulator

4. 올바르게 설정됬다면, CMD창에서 adb 명령어가 실행됩니다.
5. AVD Manager을 설정합니다.
6. ionic 프로젝트 폴더의 platforms/android 를 open합니다.
7. 프로젝트를 안드로이드 스튜디오로 build 합니다.
8. 실행을 확인합니다. 

ionic build android
ionic cordova prepare android
ionic cordova platform add android
ionic cordova emulate android
Ionic cordova run android
```

```
npm uninstall -g ionic --save
npm uninstall -g ionic@3.20.0 --save
npm uninstall -g ionic --save
npm uninstall -g ionic@5.4.15 --save
npm uninstall -g ionic --save
npm cache clean -f
재시작
npm install g ionic@3.20.0
```

```
coreybutler/nvm-windows
release 1.1.6 install

nvm install 8.11.3
nvm install 0.12.7

nvm use 8.11.3

npm install -g cordova@8.0.0
npm install -g ionic@3.20.0
```
```
as-is
ionic 3.9.1
node 8.11.3
cordova 8.0.0

to-be
ionic 1.7.14
node 4.2.4
cordova 6.5.0
```

### Angular
1. 단방향 데이터 바인딩인 이유는?
```
양방향 데이터 바인딩의 경우, 렌더링 호출 이슈가 있을수있음
```
### RxJS
```
RxJS?
Observable을 사용해서 비동기 및 이벤트 기반 프로그램을 작성하기 위한 라이브러리
비동기에 대한 솔루션
리액트 프로그래밍과 함수형 프로그래밍 철학의 교집합

프로그램 오류란 사용자의 입력에 따라 프로그램이 예상하는 결과를 얻지 못하는 것

SPA : 페이지 하나로 이루어진 웹 어플리케이션

입력 오류 해결
동기, 비동기 데이터를 Observable로 일원화하는것

상태 오류 해결
Observable은 read-only로 단방향

로직 오류 해결
반복,분기,변수제거를 위해 함수형 프로그래밍 사용

Observable 만들기
array -> from -> pipe -> fillfrom???

오퍼레이터 (Observable 실험 및 조작)
Observable은 데이터를 observer가 subsribe하게되면 전달한다.
Obserber는 Observable에서 전달하는 데이터를 소비하는 주체로, next,error,complete 세 가지 메소드를 가지고있음

of : 각각 단일 데이터 값을 전달, observable
range : 범위 내 값
fromEvent : 브라우저에서 발생하는 이벤트 받아옴
from : 모든 데이터
promise : 성공(resolve)시 데이터를 전달, complete 호출
실패(reject)시 자동구독해제
interval(1000) 1초마다 호출

promise와 observer의 공통점
push방식
에러처리 지연

promise와 observer의 차이점
지연X, 취소지원X, 딱 한번 호출, 데이터 1개만 전달가능해


```

아이오닉 아이콘,스플래시 변경
```
이미지 만들어서 resources에 넣어두기
ionic cordova resources
아이디/패스워드 입력
ionic cordova platform rm android
ionic cordova platform add android
```

아이오닉 무료테마
```
달력 :
https://market.ionicframework.com/starters/calendar
npm install customcal --save
npm install moment --save


기본디자인 :
https://market.ionicframework.com/themes/ionic-material-design
```
