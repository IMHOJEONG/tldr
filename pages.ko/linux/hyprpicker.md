# hyprpicker

> wlroots 기반 컴포지터 (예: Hyprland)를 위한 경량 Wayland 색상 선택 도구.
> Wayland 세션 필요. 클립보드 자동 복사를 사용하려면, `wl-copy`가 설치되어 있어야 함.
> 더 많은 정보: <https://wiki.hypr.land/Hypr-Ecosystem/hyprpicker/>.

- 기본 형식으로 색상 선택 (16진수):

`hyprpicker`

- 지정한 형식으로 색상 출력:

`hyprpicker {{[-f|--format]}} {{hex|rgb|hsl|hsv|cmyk}}`

- 선택한 색상을 클립보드에 복사:

`hyprpicker {{[-a|--autocopy]}}`

- 컬러 출력을 비활성화하고 일반 텍스트만 출력:

`hyprpicker {{[-n|--no-fancy]}}`

- 선택한 색상을 쉘 변수에 저장:

`{{color}}=$(hyprpicker {{[-f|--format]}} {{hex}})`

- 도움말 표시:

`hyprpicker {{[-h|--help]}}`
