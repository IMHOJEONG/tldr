# hatch

> 현대적이고, 확장 가능한 Python 프로젝트 관리 도구.
> 관련 항목: `poetry`.
> 더 많은 정보: <https://hatch.pypa.io/latest/cli/reference/>.

- 새로운 Hatch 프로젝트 생성:

`hatch new {{프로젝트_이름}}`

- 기존 프로젝트에 Hatch 초기화:

`hatch new --init`

- Hatch 프로젝트 빌드:

`hatch build`

- 빌드 산출물 삭제:

`hatch clean`

- Create a default environment with dependencies defined in the `pyproject.toml` 파일에 정의된 의존성을 기반으로 기본 환경 생성:

`hatch env create`

- 환경 의존성을 표 형태로 출력:

`hatch dep show table`
