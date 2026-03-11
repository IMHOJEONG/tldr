# biber

> `biblatex` 패키지를 위한 백엔드 참고문헌 처리기.
> 관련 항목: `latexmk`.
> 더 많은 정보: <https://texdoc.org/serve/biber.pdf/0#section.3>.

- BibLaTeX 제어 파일을 사용하여 참고문헌 데이터를 생성:

`biber {{경로/대상/파일.bcf}}`

- 설정 파일을 사용하여 참고문헌 데이터를 생성:

`biber {{경로/대상/파일.bcf}} {{[-g|--configfile]}} {{경로/대상/설정_파일}}`

- 디버깅을 활성화:

`biber {{경로/대상/파일.bcf}} {{[-D|--debug]}}`
