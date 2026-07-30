# hddtemp

> S.M.A.R.T. 정보를 사용하여 HDD의 온도를 표시.
> 더 많은 정보: <https://manned.org/hddtemp>.

- 지정한 드라이브의 온도 표시:

`hddtemp {{타입}}:{{/dev/sdX}}`

- `sda`로 할당된 SATA 드라이브의 온도 표시:

`hddtemp SATA:/dev/sda`

- 지정한 간격(`n`초)마다 온도를 syslog에 기록:

`hddtemp {{[-S|--syslog]}} {{n초}} {{타입}}:{{/dev/sdX}}`

- 온도를 단위 없이 숫자만 출력:

`hddtemp {{[-n|--numeric]}} {{타입}}:{{/dev/sdX}}`

- 온도 단위 지정:

`hddtemp {{[-u|--unit]}} {{C|F}} {{타입}}:{{/dev/sdX}}`

- 온도를 읽기 전에 ATA 드라이브 활성화:

`hddtemp {{[-w|--wake-up]}} {{타입}}:{{/dev/sdX}}`

- 디버그 모드로 실행해 S.M.A.R.T. 필드와 값을 표시:

`hddtemp {{[-D|--debug]}} {{타입}}:{{/dev/sdX}}`

- 드라이브 유형 호환성 검사 생략:

`hddtemp {{[-q|--quiet]}} {{타입}}:{{/dev/sdX}}`
