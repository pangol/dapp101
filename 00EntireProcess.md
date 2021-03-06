# 이더리움 Dapp 학습 과정 둘러보기

## 1.Dapp을 올릴 블록체인을 선택하고 해당 블록체인에 대한 학습

이더리움을 설치하고 geth라는 cli 도구를 통해서 컴퓨터에 설치한 노드와 통신하는 법을 익힙니다. (cli는 명령어를 타이핑해서 통신하는 인터페이스를 말합니다.)

이 부분에서는 geth 의 명령어가 무엇이 있는지 옵션이 무엇을 뜻하는지를 익히는 게 중요하더라구요. 자주 사용하는 옵션을 기억해두면 편합니다.

이더리움에서는 private network를 구동하기 위한 옵션 체크하고 계정에서 이더보내기, 채굴해보기 등등을 익힙니다.

## 2. Smart Contract 작성을 위한 프로그래밍 언어 익히기와 컴파일

윈도우에서 돌아가는 프로그램을 만들기 위해서는 C++, C#을 사용하듯이 이더리움 위에 올라갈 Dapp을 만들기 위해서 사용해야 하는 언어가 있습니다.

그 중에 문서가 제일 많은 solidity 선택! 에디터는 VIM을 사용해서 했습니다. vim을 사용해서 solidity 소스를 작성하고 solc 컴파일러를 이용해서 소스를 컴파일합니다.


Dapp 배포를 위해서는 소스를 컴파일 후에 얻어야할 정보가 **abi**라는 인터페이스와 **binary code** 두 가지 입니다.

이 두가지를 컴파일 할 때 output으로 빼내고 private network구동 후에 배포를 시킵니다. (Dapp 연습할 때 가장 헷갈리는 부분!!! -0-)

한 두 번 해보면 감이 잡힙니다. 허나 하다보면 뭐가 막 불편합니다. 그래서 IDE를 찾아봤더니 REMIX라는 걸 가장 많이 사용하더군요. 제작부터 배포까지 가능합니다. REMIX 사용법을 익히고 넘어갑니다.

## 3. Front-end(웹)와 Smart Contract 연결해서 DApp 만들기
Web application개발할 때와 비슷합니다. web3라고 하는 자바스크립트 기반으로 만들어진 라이브러리를 사용해서 이더리움의 private network와 통신하는 법을 익히며

nodejs를 설치하고 express, web3를 사용해서 private network와 통신한 내용을 Front단에 뿌려주는 식으로 개발을 해봅니다.

## 4. 개발 프레임워크 Truffle 익히기

스마트 컨트랙트 작성법을 알고 web3을 이용해서 노드와의 커뮤니케이션을 익혔다면 컨트랙트 컴파일, 배포, 테스트까지 자동화 해주는 Truffle을 이용하면 개발 속도가 더 빨라질겁니다.

## 마무리
Dapp101은 빠르게 실전처럼 익히는 걸로 중점을 두고 제작되었습니다.

이후의 커리큘럼은 위에 명시된 모든 과정을 빠르게 훑으며 설치의 어려움을 덜기 위해 이더리움 네트워크는 테스트 네트워크로 Ganache를 사용하고 Truffle을 사용해서 제작하게 됩니다.

