# hyprsunset

> Hyprland용 블루라이트 필터 .
> 선택적으로 `~/.config/hypr/hyprsunset.conf` 설정 파일을 사용할 수 있음.
> 더 많은 정보: <https://wiki.hypr.land/Hypr-Ecosystem/hyprsunset/>.

- hyprsunset 서비스 시작:

`hyprsunset`

- 지정한 색온도와 감마 값으로 hyprsunset 서비스 시작:

`hyprsunset {{[-t|--temperature]}} {{온도}} {{[-g|--gamma]}} {{감마_값}}`

- 실행중인 hyprsunset 서비스의 색온도 조정:

`hyprctl hyprsunset temperature {{온도}}`

- 실행중인 hyprsunset 서비스의 감마 값 조정:

`hyprctl hyprsunset gamma {{감마_값}}`

- 색온도를 기본값(6000K)으로 초기화:

`hyprctl hyprsunset reset temperature`

- 감마를 기본값(100%)으로 초기화:

`hyprctl hyprsunset reset gamma`
