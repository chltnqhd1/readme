# 오픈소스 readme 과제
## 리눅스 명령어
### top


### ps

ps 명령어는 현재 시스템에서 돌고있는 프로세스를 보여주는 가장 기본적인 명령어입니다.\
실행 중인 프로세스를 시각화 할 수 있으며, 기본적으로 터미널에서 스시템 프로세스를 조작합니다.\
예를 들어 'watch' 명령을 이용해 일정 시간마다 ps를 실행하여 실시간 감시자로 사용할 수 있습니다.\
'top'과 같지는 않으며 그저 간단히 보기위함입니다.

### jobs

작업의 상태를 표시하는 명령어입니다.\
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

리눅스에서 작업을 할 때 응용프로그램이나 프로세스가 멈추는 것을 볼 수 있습니다.\
이 때의 유일한 해결책은 그 프로세스를 종료하는 것입니다.\
대게 프로세스를 죽일 때 쓰입니다. 프로세스 죽이는 방법은 \
죽이려는 프로세스의 pid를 얻은 다음 kill 명령어의 인자로 넘기면 됩니다.


툴 형식은 \
`$ kill [options] <pid> [...]`

## vim 에디터 매크로

