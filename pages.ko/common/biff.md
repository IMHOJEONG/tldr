# biff

> 날짜 및 시간 계산, 파싱, 형식 지정을 수행하는 간단한 유틸리티.
> 더 많은 정보: <https://github.com/burntsushi/biff>.

- 원하는 시간으로 현재 시간을 출력:

`biff time fmt {{[-f|--format]}} rfc3339 now`

- 하나의 명령으로 여러 상대 시간을 출력:

`biff time fmt {{[-f|--format]}} '%c' now -1d 'next sat' 'last monday' '9pm last mon'`

- 다른 시간대의 현재 시간을 출력하고 가장 가까운 15분 단위로 반올림:

`biff time in Asia/Bangkok now | biff time round {{[-i|--increment]}} 15 {{[-s|--smallest]}} minute`

- 두 시간대 사이에서 시간을 변환:

`TZ='Japan' biff time in America/New_York 02:30`

- 현재 시간을 기준으로 과거 또는 미래 시간을 출력:

`biff time add {{-1d|1d|1w|-1m|1y|...}} now`

- 현재 시간에 복합적인 기간을 추가:

`biff time add '1 week, 12 hours ago' now`

- 과거 날짜 이후의 경과 시간을 계산하고 원하는 정밀도로 반올림:

`biff span since 2025-01-20T12:00 {{[-l|--largest]}} year`

- 로그 파일에서 타임스탬프를 찾고 로컬 시간으로 변환하여 표시:

`biff tag lines /tmp/access.log | biff time in system | biff time fmt {{[-f|--format]}} '%c' | head {{[-n|--lines]}} 3 | biff untag {{[-s|--substitute]}}`
