# watchman

> 파일 변경 사항을 관찰하고 변경이 발생하면 지정한 작업을 실행하는 서비스.
> 더 많은 정보: <https://facebook.github.io/watchman/docs/cli-options>.

- 지정한 디렉터리가 속한 프로젝트의 루트 디렉터리를 추론하고, 해당 디렉터리 및 하위 폴더의 파일 변경 관찰:

`watchman watch-project {{경로/대상/디렉터리}}`

- 관찰 중인 디렉터리에서 지정한 파일 이름 패턴과 일치하는 파일이 변경되면 명령을 실행하도록 트리거를 추가:

`watchman -- trigger {{경로/대상/관찰중인_디렉터리}} {{트리거_이름}} '{{패턴}}' -- {{명령어}}`

- 관찰 중인 모든 디렉터리 목록 표시:

`watchman watch-list`

- 디렉터리 관찰과 연결된 트리거 삭제:

`watchman watch-del {{경로/대상/관찰중인_디렉터리}}`

- 모든 디렉터리 관찰과 트리거 삭제:

`watchman watch-del-all`

- 관찰 중인 디렉터리에 설정된 모든 트리거 목록 표시:

`watchman trigger-list {{경로/대상/관찰중인_디렉터리}}`

- 관찰 중인 디렉터리에서 지정한 트리거 삭제:

`watchman trigger-del {{경로/대상/관찰중인_디렉터리}} {{트리거_이름}}`

- 다음 `watchman` 명령이 실행될 때까지, `watchman`을 일시적으로 중지:

`watchman shutdown-server`
