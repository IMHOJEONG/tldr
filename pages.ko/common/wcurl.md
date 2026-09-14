# wcurl

> 파일 쉽게 다운로드하기 위한 `curl`의 단순화한 래퍼.
> 관련 항목: `wget`, `curl`.
> 더 많은 정보: <https://curl.se/wcurl/manual.html>.

- URL의 내용을 URL에 지정된 파일 이름으로 다운로드 (이 경우 `index.html`):

`wcurl {{https://example.com/index.html}}`

- URL의 내용을 지정한 이름의 파일로 다운로드:

`wcurl {{[-o|--output]}} {{경로/대상/파일}} {{https://example.com/index.html}}`

- 진행률 표시줄 활성화 및 HTTP/2를 기본으로 사용해 URL의 내용을 다운로드:

`wcurl --curl-options "--progress-bar --http2" {{https://example.com/index.html}}`

- 중단된 다운로드 이어서 실행:

`wcurl --curl-options "--clobber --continue-at -" {{https://example.com/index.html}}`
