# copilot

> GitHub Copilot과 상호작용.
> 더 많은 정보: <https://docs.github.com/en/copilot/concepts/agents/about-copilot-cli>.

- 대화형 모드를 시작:

`copilot`

- 모든 파일 편집을 허용:

`copilot --allow-tool write`

- 가장 최근 세션을 이어서 진행:

`copilot --continue`

- 세션 선택기를 사용하여, 이전 세션을 이어서 진행:

`copilot --resume`

- 특정 모델을 사용:

`copilot --model "{{gpt-5}}"`

- `git push`를 제외한 모든 Git 명령을 허용:

`copilot --allow-tool 'shell(git:*)' --deny-tool 'shell(git push)'`

- 대화형 모드 없이 프롬프트를 직접 실행하며, `copilot`이 모든 명령을 실행할 수 있도록 허용:

`copilot {{[-p|--prompt]}} "{{Fix the bug in main.js}}" --allow-all-tools`
