# coreutils

> Uutils coreutils는 GNU coreutils를 Rust로 재구현한 크로스 플랫폼 도구 모음.
> Uutils는 여러 유틸리티를 하나의 실행 파일에서 호출할 수 있는 멀티콜 바이너리를 포함하여, 이를 통해 바이너리 크기를 줄이고 이식성을 높임.
> 더 많은 정보: <https://uutils.github.io/coreutils/docs/multicall.html>.

- 유틸리티를 인자와 함께 실행:

`coreutils {{유틸리티}} {{유틸리티_옵션}}`

- 파일을 긴([l]ong) 형식으로 나열:

`coreutils ls -l`

- `ls`의 도움말을 표시:

`coreutils ls --help`
