# nwipe

> 다양한 표준 데이터 삭제 방식으로 디스크의 데이터를 안전하게 삭제.
> 더 많은 정보: <https://manned.org/nwipe>.

- 대화형 Ncurses 인터페이스 실행:

`sudo nwipe`

- 확인 메시지 없이 기본 방식 (DoD 3-pass)으로 지정한 장치의 데이터 삭제:

`sudo nwipe --autonuke {{/dev/sdX /dev/sdY ...}}`

- 사용자 지정 삭제 방식으로 지정한 디스크의 데이터 삭제:

`sudo nwipe {{[-m|--method]}} {{zero|one|gutmann|dod522022m|...}} {{/dev/sdX}}`

- 디스크의 데이터를 삭제하고 완료 후 시스템 종료:

`sudo nwipe --autonuke --autopoweroff {{/dev/sdX}}`

- 버전 정보 표시:

`nwipe {{[-V|--version]}}`
