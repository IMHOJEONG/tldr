# copr-cli

> Fedora-Projects의 copr 인스턴스와 상호작용하여 RPM을 빌드하고 배포.
> 더 많은 정보: <https://manned.org/copr-cli>.

- copr에 로그인된 사용자 정보:

`copr-cli whoami`

- 로컬 spec 파일을 copr에서 빌드:

`copr-cli build {{저장소}} {{path/to/spec_file}}`

- 빌드 상태를 확인:

`copr-cli list-builds {{저장소}}`

- 공개(Git) 저장소의 spec 파일을 사용하여 copr 빌드를 실행:

`copr-cli buildscm {{저장소}} --clone-url {{https://git.example.org/repo}} --spec {{스펙_파일_이름}}`
