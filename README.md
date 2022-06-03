# 오픈소스 readme 과제
## 리눅스 명령어
### top

__리눅스 시스템을 실시간으로 전반적인 상황을 모니터링하거나 프로세스 관리를 할 수 있는 유틸리티명령어 입니다.__\
어떤 프로세스가 CPU를 과다하게 잡고 있는지 분석이 가능합니다.


<img src="https://user-images.githubusercontent.com/88511523/171817739-90ab1b25-9d9e-453f-9f44-782c94503100.png" width="85%" height="85%"/>

해당사진은 요약 영역은 top에서 상단에 위치하고 있습니다. 이 요약영역은 전체 프로세스가 OS에 대해서 리소스를\
어느정도 차지하고 있는지를 알려줍니다. 요약 영역에 나타나는 대표적인 값은\
시간(System time), 유저(User), 로드 에버리지(Load Average), 테스크(Tasks), CPU, 메모리(memory)로\
아래의 이미지를 보시면 각 영역에 대해 나타내는 값이 어디에 위치하는지 알 수 있습니다.



### ps

 __현재 시스템에서 돌고있는 프로세스를 보여주는 가장 기본적인 명령어입니다.__\
실행 중인 프로세스를 시각화 할 수 있으며, 기본적으로 터미널에서 스시템 프로세스를 조작합니다.\
예를 들어 'watch' 명령을 이용해 일정 시간마다 ps를 실행하여 실시간 감시자로 사용할 수 있습니다.\
'top'과 같지는 않으며 그저 간단히 보기위함입니다. ps는 ps한 시점에 proc에서 검색한 cpu 사용량을\
top은 proc에서 일정 주기로 합산해 cpu 사용율 출력해줍니다.


### jobs

 __백그라운드로 실행되는 작업목록(작업번호, 상태, 명령어)의 상태를 표시하는 명령어입니다.__\
현재 쉘 세션에서 실행시킨 백그라운드 작업의 목록이 출력되며, \
각 작업에는 번호가 붙어 있는 kill 명령어 뒤에 '%번호' 등으로 사용할 수 있습니다.


툴 형식은\
`jobs [옵션][작업번호]`


사용할 수 있는 옵션은
|옵션|설명|
|:--:|:--:|
|-l|프로세스 그룹 ID를 state 필드 앞에 출력|
|-n|프로세스 그룹 중에 대표 프로세스 ID를 출력|
|-p|각 프로세스 ID에 대한 한 행씩 출력|
|command|지정한 명령어를 실행|


### kill

 __프로세스를 죽일 때 쓰이는 명령어 입니다.__\
리눅스에서 작업을 할 때 응용프로그램이나 프로세스가 멈추는 것을 볼 수 있습니다.\
이 때의 유일한 해결책은 그 프로세스를 종료하는 것입니다.\ 프로세스 죽이는 방법은 \
죽이려는 프로세스의 pid를 얻은 다음 kill 명령어의 인자로 넘기면 됩니다.


툴 형식은 \
`$ kill [options] <pid> [...]`


## vim 에디터 매크로

### 매크로란?

특정한 움직임 또는 입력을 키에 저장함으로써 단순하면서 반복되는 동작을
쉽고 빠르게 해주는 것을 말합니다.

### vim에디터에서 매크로 사용방법

|단축키|설명|
|:--:|:--:|
|q + [설정키]|[설정키]에 recording 시작|
|q|recoding 종료|
|@[설정키]|1회 실행|
|@@|방금 실행한 매크로 실행|
|n@[설정키]|매크로 n회 실행|
|Ctrl+a|숫자 증가|
|Ctrl+x|숫자 감소|

### 숫자 증가 매크로

매크로를 지정하고 숫자를 증가시키고 싶을 때 빠르게 할 수있는데\
순서는\
1. 1 숫자 입력
2. 매크로 시작
3. 1 숫자를 복사해서 다음줄에 붙여넣기
4. 두번째줄 1에 커서를 올리고 Ctrl+a(숫자 증가)
5. 매크로 종료

이런 식으로 매크로를 실행하면 1 2 3 4 5... 로 출력이 됩니다.








