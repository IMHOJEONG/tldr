# clear

> 터미널 화면을 지움.
> 더 많은 정보: <https://manned.org/clear>.

- 화면을 지움:

`clear`

- 터미널의 스크롤백 버퍼는 유지한 채 화면만 지움(Bash에서 `<Ctrl l>`을 누르는 것과 동일):

`clear -x`

- 정리할 터미널 유형을 지정 (기본값은 환경 변수 `$TERM`의 값):

`clear -T {{터미널_종류}}`

- `clear`가 사용하는 `ncurses` 버전을 표시:

`clear -V`
