CUCKOO Fee Calculator GitHub Pages wrapper

이 폴더의 index.html은 Google Apps Script 웹앱을 GitHub Pages 주소에서 열 수 있게 해주는 iframe 래퍼입니다.
실제 계산/구글시트 연동은 계속 Apps Script 웹앱에서 동작합니다.

현재 연결된 Apps Script URL:
https://script.google.com/macros/s/AKfycbyjkb1sLB23L6LJarGo1S7Avs6ffccWjw42TFSzvBlkfnGAlkGjEJG8ivcIyxy3dPtJ/exec

배포 방법:
1. GitHub에서 새 저장소를 만듭니다. 예: cuckoo-fee-calculator
2. 이 github_pages 폴더 안의 index.html을 저장소 루트 또는 docs 폴더에 업로드합니다.
3. 저장소 Settings > Pages에서 배포 소스를 main branch / root 또는 docs로 지정합니다.
4. 발급된 https://계정명.github.io/저장소명/ 주소로 접속합니다.

주의:
- Code.gs와 구글시트 연동은 GitHub Pages 단독으로 실행되지 않습니다.
- GitHub Pages는 정적 HTML/CSS/JS 호스팅이므로, 현재 구조에서는 Apps Script 웹앱을 계속 유지해야 합니다.
- Apps Script의 doGet()에서 XFrameOptionsMode.ALLOWALL이 설정되어 있어 iframe 방식 사용이 가능합니다.
