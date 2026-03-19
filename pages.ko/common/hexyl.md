# hexyl

> 터미널에서 사용하는 간단한 16진수 뷰어. 다양한 바이트 유형을 구분하기 위해 색상 출력을 사용.
> 관련 항목: `od`, `xxd`, `hexdump`.
> 더 많은 정보: <https://github.com/sharkdp/hexyl/blob/master/doc/hexyl.1.md>.

- 파일의 16진수 표현 출력:

`hexyl {{경로/대상/파일}}`

- 파일의 처음 n 바이트에 대한 16진수 표현 출력:

`hexyl {{[-n|--length]}} {{n}} {{경로/대상/파일}}`
