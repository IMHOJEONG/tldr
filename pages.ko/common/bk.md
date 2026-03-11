# bk

> Buildkite 빌드, 파이프라인 및 에이전트를 관리.
> 더 많은 정보: <https://github.com/buildkite/cli#usage>.

- API 토큰과 조직을 설정:

`bk configure`

- 사용할 조직을 선택:

`bk use {{조직_slug}}`

- `pipeline.yaml` 파일 초기화:

`bk init`

- 현재 조직의 모든 파이프라인을 표시:

`bk pipeline list`

- 파이프라인에 대한 빌드를 트리거:

`bk build create {{파이프라인_slug}}`

- 특정 빌드의 상태를 확인:

`bk build view {{빌드_번호}}`

- 현재 조직의 모든 에이전트를 표시:

`bk agent list`

- 도움말 표시:

`bk {{[-h|--help]}}`
