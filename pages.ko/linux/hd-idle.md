# hd-idle

> 일정 시간 동안 사용되지 않은 외장 디스크를 자동으로 회전 정지시킴.
> 더 많은 정보: <https://manned.org/hd-idle>.

- 하드 디스크 회전 정지 관리 서비스 시작. (기본적으로 10분 동안 사용하지 않으면, 디스크를 회전 정지):

`systemctl start hd-idle`

- 지정한 디스크를 즉시 회전 정지:

`hd-idle -t {{/dev/sdX}}`

- 모든 디스크의 자동 회전 정지를 비활성화하고, "sda"와 "sdb" 디스크에 각각 지정한 유휴 시간(초)을 설정:

`hd-idle -i 0 -a /dev/sda -i {{300}} -a /dev/sdb -i {{1200}}`
