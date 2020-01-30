Ionic + Angular + Android

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
    JAVA_HOME (EX : C:\java-13-openjdk\java-13-openjdk)
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

