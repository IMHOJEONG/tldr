# clang-check

> 기본 오류를 검사하고 Clang의 추상 구문 트리(AST)를 다룸.
> Clang의 LibTooling 구성요소이며, C/C++ 코드를 디버깅 및 분석하는 데 유용.
> 더 많은 정보: <https://manned.org/clang-check>.

- 소스 파일에 대해 기본 검사를 실행:

`clang-check {{경로/대상/파일.cpp}} --`

- 디버깅을 위해 추상 구문 트리를 출력:

`clang-check {{경로/대상/파일.cpp}} -ast-dump --`

- 이름으로 AST를 필터링:

`clang-check {{경로/대상/파일.cpp}} -ast-dump -ast-dump-filter FunctionName`

- AST를 형식에 맞게 출력:

`clang-check {{경로/대상/파일.cpp}} -ast-print --`
