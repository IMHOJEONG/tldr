# hexdump

> 파일 내용을 16진수, 10진수, 8진수 또는 ASCII 형식으로 출력.
> 덤프 파일, 바이너리 데이터 또는 디버그 출력 등을 확인할 때 유용.
> 관련 항목: `hexyl`, `od`, `xxd`.
> 더 많은 정보: <https://manned.org/man/freebsd/hexdump.1>.

- 파일의 16진수 표현 출력, 중복된 줄은 `*`로 대체:

`hexdump {{경로/대상/파일}}`

- 입력 오프셋을 16진수로, ASCII 표현을 두 컬럼으로 출력:

`hexdump -C {{경로/대상/파일}}`

- 입력의 특정 바이트 수만 해석하여 16진수 출력:

`hexdump -C -n {{number_of_bytes}} {{경로/대상/파일}}`

- 상세 출력 (중복 줄을 `*`로 생략하지 않음):

`hexdump -v {{경로/대상/파일}}`

- printf 스타일 포맷 문자열을 사용해 출력 형식 지정:

`hexdump -e '{{element_format .. end_format}}' {{경로/대상/파일}}`
