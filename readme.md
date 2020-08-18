﻿가람 - "훈민정음은 디자인이다"
=============
<img src="https://github.com/Oasis1819/Garam/blob/master/snapshot/GaramLogo.png?raw=true" width="300">
   
가람(Garam)은 Typescript로 만들어진 신토불이 인터프리터 언어입니다.   
조선 4대 군주이신 세종대왕께서 한글을 반포하신 날을 기념으로 개발되었으며, 튜링 완전한 언어입니다.   

탄생 비화
-------------
이제 조선도 진보했습니다, 우리 조선은 백성 모두가 개발을 할 수 있도록   
훈민정음으로 튜링 완전한 언어를 만들기로 했습니다.   

용어 설명
-------------
```사회``` : 런타임 또는 프로그램   
```상소문``` : 깃허브 이슈  
```역적``` : 프로그램 버그   
```관군``` : ~~뭔가 이상한~~ 개발자   
```주식회사 10의 100승``` : Google   

명령어
-------------
가람의 명령어는 8개로 구성되어 있습니다.   
각자 한글의 아름다움과 특징을 고려하여 만들어졌습니다.   
   
```ㅗ``` : 포인터 증가   
```ㅜ``` : 포인터 감소   
```ㅏ``` : 값 증가   
```ㅓ``` : 값 감소   
```ㅇ``` : 값 출력하기   
```ㅁ``` : 값 입력받기   
```ㅑ``` : 현재 포인터가 가르키는 값이 0이면 ```ㅕ``` 다음으로 이동   
```ㅕ``` : 현재 포인터가 가르키는 값이 0이 될때까지 ```ㅑ```으로 가기   

이외의 명령어는 인식되지 않습니다.   
우리 조선은 백성들에게 이 점을 참고하여 코드를 읽을 수 있는 글로 작성할 것을 권고하고 있습니다.   
그렇지 않으면 사헌부에서 여러분을 심판할 것입니다.   

예제
-------------
입력받은 문자 계속 출력하기   
```ㅏㅑㅁㅇㅕ```
   
"2" 출력하기   
```
ㅏㅏㅏㅏㅏㅏ
ㅏㅏㅏㅏㅏㅏ
ㅏㅏㅏㅏㅏㅏ
ㅏㅏㅏㅏㅏㅏ
ㅏㅏㅏㅏㅏㅏ
ㅏㅏㅏㅏㅏㅏ
ㅏㅏㅏㅏㅏㅏ
ㅏㅏㅏㅏㅏㅏ
ㅏㅏ
ㅇ
```
   
Node.JS에서 "반갑소 세상아!" 출력하기   
```typescript
// Written with Typescript
import Garam from "garam-interpreter"

var Interpreter = new Garam()
Interpreter.Interpret(
`
ㅏㅏㅏㅏㅏㅏㅏㅏㅏㅏ
ㅑ
    ㅗ ㅏㅏㅏㅏㅏ ㅏㅏ
    ㅗ ㅏㅏㅏㅏㅏ ㅏㅏㅏㅏㅏ
    ㅗ ㅏㅏㅏ
    ㅗ ㅏ
    ㅜㅜㅜㅜ ㅓ
ㅕ
ㅗ ㅏㅏ ㅇ //H
ㅗ ㅏ ㅇ //E
ㅏㅏㅏㅏㅏ ㅏㅏ ㅇ //L
ㅇ //L
ㅏㅏㅏ ㅇ //O
ㅗ ㅏㅏ ㅇ //Space
ㅜㅜ ㅏㅏㅏㅏㅏ ㅏㅏㅏㅏㅏ ㅏㅏㅏㅏㅏ ㅇ //W
ㅗ ㅇ //o
ㅏㅏㅏ ㅇ //r
ㅓㅓㅓㅓㅓ ㅓ ㅇ //l
ㅓㅓㅓㅓㅓ ㅓㅓㅓ ㅇ //d
ㅗ ㅏ ㅇ //!
ㅗ ㅇ //create new line
`
, (ApplyValue:any) => {}, (Out:string) => {
    process.stdout.write(Out)
})
```

타입스크립트 혁명
-------------
```타입스크립트```가 혁명을 일으켜 ```가람```을 유지하던 ```코틀린```을 몰아내었습니다.   
또한 개발자의 급격한 개발능력 성장으로, 몇년 간 있었던 ```역적```이 진압되었습니다.   
이 혁명으로 인해 아래와 같은 활용이 가능해집니다.   
 * ```주식회사 10의 100승```이 개발한 Blockly와 연동하여 조선 어린이들에게 블록코딩 제공
 * 온라인 IDE에 적용
 * 기타 등등


상소문 올리기
-------------
우리 조선은 백성들의 안전한 코딩생활을 위해 노력하고 있습니다.   
가정이 무너지고 사회가 무너지게 하는 ```역적```은 ```상소문```을 통해 제보할 수 있습니다.   
적발된 버그는 ```관군```이 거제도로 끌고 가 ```사회```로부터 소멸시킵니다.
