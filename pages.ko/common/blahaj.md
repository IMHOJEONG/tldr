# blahaj

> lolcat와 유사한 출력에 색깔을 입하는 도구로 다양한 깃발 및 상어를 함께 표시.
> 더 많은 정보: <https://codeberg.org/GeopJr/BLAHAJ>.

- 사용 가능한 깃발/색상 목록을 표시:

`blahaj --flags`

- 기본 trans 색상으로 상어(blahaj)를 출력:

`blahaj {{[-s|--shark]}}`

- 랜덤 깃발을 2배 크기로 출력:

`blahaj {{[-f|--flag]}} {{[-r|--random]}} {{[-m|--multiplier]}} 2`

- 텍스트를 출력하는 명령의 결과를 lesbian 색상으로 표시:

`{{cowsay "Hello, world"}} | blahaj {{[-c|--colors]}} lesbian`

- 텍스트를 문자 단위로 색상을 추가해 출력:

`echo "{{Hello, world}}" | blahaj {{[-i|--individual]}}`

- 텍스트 문서의 내용을 단어 단위로 색깔을 추가해 출력하며, 텍스트 대신 배경에 색상을 추가:

`blahaj {{[-w|--words]}} {{[-b|--background]}} {{path/to/file}}`
