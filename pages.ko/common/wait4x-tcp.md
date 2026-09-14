# wait4x tcp

> TCP 포트를 사용할 수 있을 때까지 기다림.
> 더 많은 정보: <https://github.com/wait4x/wait4x>.

- TCP 포트를 사용할 수 있을 때까지 대기:

`wait4x tcp {{localhost:8080}}`

- 지정한 타임아웃 동안 포트가 사용 가능해질 때까지 대기:

`wait4x tcp {{localhost:3306}} --timeout {{60s}}`

- 포트가 사용되지 않는 상태가 될 때까지 대기 (반전 검사):

`wait4x tcp {{localhost:8080}} --invert-check`

- 여러 포트를 병렬로 대기:

`wait4x tcp {{localhost:3306 localhost:6379 ...}}`

- 포트를 사용할 수 있게 된 후 명령 실행:

`wait4x tcp {{localhost:3306}} -- {{경로/대상/스크립트.sh}}`

- 지수 백오프를 사용하여 포트를 대기:

`wait4x tcp {{localhost:8080}} --backoff-policy exponential --backoff-exponential-max-interval {{30s}}`
