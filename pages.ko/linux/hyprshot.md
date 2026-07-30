# hyprshot

> Hyprland Wayland 컴포지터용 스크린샷 유틸리티.
> 더 많은 정보: <https://github.com/Gustash/Hyprshot>.

- 선택한 영역의 스크린샷 촬영:

`hyprshot {{[-m|--mode]}} region`

- 선택한 창의 스크린샷 촬영:

`hyprshot {{[-m|--mode]}} window`

- 선택한 출력 장치의 스크린샷 촬영:

`hyprshot {{[-m|--mode]}} output`

- 현재 활성 창의 스크린샷 촬영:

`hyprshot {{[-m|--mode]}} active {{[-m|--mode]}} window`

- 화면을 고정한 상태에서, 선택한 영역의 스크린샷 촬영:

`hyprshot {{[-z|--freeze]}} {{[-m|--mode]}} region`

- 선택한 창의 스크린샷을 촬영 후, 지정한 출력 디렉터리에 저장:

`hyprshot {{[-o|--output-folder]}} {{경로/대상/디렉터리}} {{[-m|--mode]}} window`

- 선택한 창의 스크린샷을 촬영 후, 스크린샷을 클립보드에만 저장:

`hyprshot --clipboard {{[-m|--mode]}} output`
