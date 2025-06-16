 Snake Game (C++ & ncurses)

프로젝트 개요
이 프로젝트는 Linux 터미널 기반으로 작동하는 Snake 게임입니다.  
ncurses 라이브러리를 활용해 그래픽 없이도 실시간으로 뱀의 움직임을 구현하였고,  
성장 아이템, 독 아이템, 게이트 등의 다양한 요소를 통해 게임성을 높였습니다.

주요 파일 구조

| 파일명       | 설명                          |
|--------------|-------------------------------|
| `snake.cpp`  | 메인 게임 루프 및 전체 로직 구현 |
| `map.h`      | 게임 맵 정의 및 맵 데이터 관리 |
| `sclass.h`   | Snake 클래스 및 관련 기능 정의 |
| `vector.h`   | 좌표 계산용 Vector 클래스 구현 |

---
 실행 환경

- C++17 이상 컴파일러
- Linux / WSL 환경 (Ubuntu 권장)
- **ncurses 라이브러리 설치 필요**

설치 명령어

```bash
sudo apt update
sudo apt install libncurses5-dev

----
컴파일 및 실행
g++ snake.cpp -lncurses -o snake
./snake
