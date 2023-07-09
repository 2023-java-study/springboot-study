# springboot-study
스프링부트 스터디

### 윈도우 사용자를 위한 wsl설정
wsl 을 사용하게 되면 vmmem이란 프로세스가 많은 메로리를 점유하고 있는 것을 볼 수 있다.

[WSL의 고급 설정 구성](https://learn.microsoft.com/ko-kr/windows/wsl/wsl-config)
1. window+r로 실행창 켜기
2. %userprofile% 입력
3. 해당 경로에서 `.wslconfig`파일 생성
4. .wslconfig파일에 `memory = Windows에서 총 메모리의 50% 또는 8GB 중 적은 쪽, 20175 이전 빌드에서의 경우 Windows에서 총 메모리의 80%`,`swap=0또는1` 설정
