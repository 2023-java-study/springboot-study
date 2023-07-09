# springboot-study
스프링부트 스터디

### 윈도우 사용자를 위한 wsl설정
wsl 을 사용하게 되면 vmmem이란 프로세스가 많은 메로리를 점유하고 있는 것을 볼 수 있다.

[WSL의 고급 설정 구성](https://learn.microsoft.com/ko-kr/windows/wsl/wsl-config)
1. window+r로 실행창 켜기
2. %userprofile% 입력
3. 해당 경로에서 `.wslconfig`파일 생성
4. .wslconfig파일에 `memory = Windows에서 총 메모리의 50% 또는 8GB 중 적은 쪽, 20175 이전 빌드에서의 경우 Windows에서 총 메모리의 80%`,`swap=0또는1` 설정

### Intellij에서 wsl내의 프로젝트 build 속도 개선
Windows Defender가 wsl를 검사해서 그렇다고 한다.
1. 개인정보 및 보안 -> `Windows 보안` 이동
2. 바이러스 및 위협 방지 이동
3. 바이러스 및 위협 방 설정 의 `설정관리` 이동
4. 마지막의 제외에서 `제외 추가 또는 제거` 이동
5. 제외 사항 추가(파일, 폴더, 프로세스)
6. 프로세스: idea64.exe추가(얘 안하면 build속도 개선이 없었음)
7. 파일 : 사용하는 Intellij.exe의 경로 선택
8. 폴더 : C:\Users\zhfpt\AppData\Local\Packages\CanonicalGroupLimited.Ubuntu_79rhkp1fndgsc\LocalState
