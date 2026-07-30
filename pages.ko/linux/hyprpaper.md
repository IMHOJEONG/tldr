# hyprpaper

> Hyprland용 배경화면 유틸리티로, 배경화면을 동적으롷 변경할 수 있음.
> `~/.config/hypr/hyprpaper.conf` 설정 파일을 통해 제어됨.
> 더 많은 정보: <https://wiki.hypr.land/Hypr-Ecosystem/hyprpaper/>.

- `hyprpaper` 데몬 시작:

`hyprpaper`

- 지정한 모니터의 배경화면 변경:

`hyprctl hyprpaper wallpaper "{{모니터}},{{경로/대상/이미지.png}}"`

- 지정되지 않은 모든 모니터의 기본 배경화면과 맞춤 방식 설정:

`hyprctl hyprpaper wallpaper ",{{경로/대상/이미지.png}},{{contain|cover|tile|fill}}"`
