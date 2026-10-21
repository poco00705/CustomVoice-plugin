# CustomVoice

BetterDiscord에서 기존 CustomVoice 백엔드의 음성 채널과 화면 공유를 이용하는 플러그인입니다. 현재 버전: **1.0.32**.

## 설치

[CustomVoice.plugin.js 다운로드](https://raw.githubusercontent.com/poco00705/CustomVoice-plugin/main/CustomVoice.plugin.js)를 BetterDiscord의 Plugins 폴더에 넣고 활성화하세요. 설정은 BetterDiscord → Plugins → CustomVoice에서 엽니다.

## 자동 업데이트

시작 시와 매 정시에 main의 최신 커밋을 확인합니다. 해당 커밋에 고정된 파일의 이름·버전을 검사하고, 설치된 파일보다 높은 버전일 때만 교체합니다. 교체 전 같은 폴더에 날짜가 붙은 .bak 백업을 만듭니다. BetterDiscord가 변경을 감지해 다시 로드합니다.

통화·방송 중에는 업데이트를 보류하고 다음 확인 시 재시도합니다. 로그인과 설정은 별도 BetterDiscord 데이터에 저장되어 유지됩니다. 네트워크 오류나 같거나 낮은 버전으로는 기존 파일을 교체하지 않습니다.

화면 공유의 시스템 소리 송출은 기본 켜짐입니다. 1.0.30에서 기존 설정도 최초 한 번 켜짐으로 전환합니다. 이후 공유 시작 창이나 방송 미리보기의 방송 설정에서 끌 수 있으며, 사용자가 끈 선택은 유지됩니다. 시스템 오디오는 선택한 앱에 한정되지 않을 수 있습니다.

## 새 버전 배포

개발 프로젝트에서 버전을 올리고 타입 검사·회귀 검사·빌드를 완료한 후 dist/CustomVoice.plugin.js를 이 저장소 main의 CustomVoice.plugin.js로 교체하세요. 이 저장소는 배포 파일만 포함하며 사용자 설정·세션·인증 정보는 업로드하지 않습니다.

## 1.0.32 서버 이전

기본 주소는 `https://mcv.modaweb.kr`입니다. 기존 `voice.222.121.56.92.sslip.io`와 `voice.125.132.41.195.sslip.io`를 쓰던 설정·기본 WebSocket 주소·저장 로그인 연결 정보를 업데이트 후 자동 전환합니다. 사용자 지정 서버 주소는 유지합니다. 서버 이전 과정에서 세션이 만료·삭제되었다면 재로그인이 필요할 수 있습니다.
