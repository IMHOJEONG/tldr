# wait4x http

> 유연한 검증 옵션을 사용해 HTTP(S) 엔드포인트를 사용할 수 있을 때까지 대기.
> 더 많은 정보: <https://github.com/wait4x/wait4x>.

- HTTP 엔드포인트가 지정한 상태 코드를 반환할 때까지 대기:

`wait4x http {{https://example.com/health}} --expect-status-code {{200}}`

- 응답 본문이 `regex` 패턴과 일치할 때까지 대기:

`wait4x http {{https://api.example.com/status}} --expect-body-regex '{{\"status\":\s*\"healthy\"}}'`

- GJSON 경로 구문을 사용하여 지정한 JSON 필드가 존재할 때까지 대기:

`wait4x http {{https://api.example.com/status}} --expect-body-json "{{services.database.status}}"`

- 사용자 지정 요청 헤더를 사용하여 응답 대기:

`wait4x http {{https://api.example.com}} --request-header "{{Authorization: Bearer token123}}"`

- 지정한 응답 헤더가 특정 값과 일치할 때까지 대기:

`wait4x http {{https://api.example.com}} --expect-header "{{Content-Type=application/json}}"`

- TLS 클라이언트 인증서를 사용해 응답 대기:

`wait4x http {{https://example.com}} --cert-file {{경로/대상/인증서.pem}} --key-file {{경로/대상/키.pem}}`

- 사용자 지정 타임아웃 및 반전 검사를 사용해 대기 (엔드포인트가 중단될 때까지 대기):

`wait4x http {{https://example.com/health}} --expect-status-code {{200}} --invert-check --timeout {{60s}}`
