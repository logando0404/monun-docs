# 서버 설정하기(~1.16.5)

모장은 [21w19a SNAPSHOT](https://www.minecraft.net/en-us/article/minecraft-snapshot-21w19a) 버전과 함께, 앞으로 Java 16 버전을 사용한다고 발표했습니다. 하지만 이는 Java 1.8 버전만을 요구했던 Bukkit, Spigot, Paper의 코드 중 호환되지 않는 부분이 있었고, 1.17 이전의 NMS 코드는 최신 버전에서 더 이상 사용할 수 없습니다. 이는 NMS 코드를 이용했던 Tap과 Kommand에 영향을 미쳤고, 구 버전의 Tap과 Kommand를 사용하는 플러그인들은 더 이상 1.17에서 실행되지 않습니다. 또한, 1.17 이전의 Tap은 플러그인 형태의 라이브러리이기 때문에 플러그인을 직접 다운로드 받아야합니다.

## 옛 버전의 서버 실행하기
### Server-Script
server-script에서, 사용자가 Config를 통해 서버 프로그램을 받아오는 URL을 직접 사용할 수 있습니다. 방법은 간단합니다.

1. server.sh.conf를 연타(없을 경우 스크립트를 한번 돌리거나 만든다)
2. `server=https://papermc.io/api/v2/projects/<project>/versions/<version>/builds/<build>/downloads/<downloads>`을 추가하거나 수정합니다.
  - (예: project - paper, version - 버전, build - 빌드번호, downloads - paper-버전-빌드번호.jar)
3. 서버 실행

### 직접 다운로드 하기
1. [PaperMC Legacy](https://papermc.io/legacy) 페이지에 들어갑니다.
2. 원하는 버전을 선택합니다.
3. 서버를 실행합니다.

### 플러그인 넣기
Tap의 경우, [여기](https://github.com/monun/tap/releases)에 빌드된 버전이 있습니다. 여기에서 요구되는 버전의 플러그인을 다운받아 서버의 플러그인 디렉토리에 넣으면 됩니다.

<!---이미지 추가 예정-->
