# nara-bid-office

수주 실행 시스템(`nara-bid-exec`, 비공개)의 **오피스 대시보드 출력물만** 담는 공개 저장소입니다.

- 주소: https://bizsinsightclub.github.io/nara-bid-office/
- `index.html` 하나가 전부입니다. 본문은 **AES-256-GCM 으로 암호화**돼 있고(PBKDF2-SHA256 키 유도),
  비밀번호를 입력하면 브라우저 안에서만 복호됩니다. 서버로 전송되는 것은 없습니다.
- 여기에는 코드·제안 본문·비밀번호가 **없습니다.** 갱신은 비공개 저장소에서 `node scripts/publish-office.mjs` 로 합니다.

## 한계 (정직하게)

- GitHub Pages 는 공개 URL 입니다. 누구나 `index.html` 을 내려받아 **오프라인으로 비밀번호를 맞춰 볼 수 있습니다.**
  비밀번호를 길게 두십시오. 정적 페이지라 잠금(lockout)은 불가능합니다.
- 검색 엔진에는 `noindex` 를 걸어 두었지만, 주소를 아는 사람은 페이지를 볼 수 있습니다(내용은 암호문).
