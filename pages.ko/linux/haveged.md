# haveged

> 하드웨어 기반 난수 생성기.
> 더 많은 정보: <https://manned.org/haveged>.

- 난수 생성:

`sudo haveged`

- 포그라운드에서 `haveged` 실행:

`sudo haveged {{[-F|--Foreground]}}`

- `haveged` 출력 파일 경로 설정:

`sudo haveged {{[-f|--file]}} {{경로/대상/파일}}`

- 데몬의 실행 레벨 설정:

`sudo haveged {{[-r|--run]}} {{실행_레벨}}`

- 수집 버퍼 크기(KiB 워드 단위) 설정:

`sudo haveged {{[-b|--buffer]}} {{inKW_단위_버퍼_크기}}`

- 실행 중인 `haveged` 프로세스 또는 데몬에 명령 전달:

`sudo haveged {{[-c|--command]}} {{명령어}}`

- 캐시 크기(KiB 워드 단위) 설정:

`sudo haveged {{[-d|--data]}} {{KW_단위_캐시_크기}}`

- 출력 파일에 기록할 바이트 수 설정:

`sudo haveged {{[-n|--number]}} {{바이트_수}}`
