# 인스타 예약 게시 + 댓글 자동 DM

이 저장소는 GitHub Actions 로 돌아간다. 컴퓨터가 꺼져 있어도 동작한다.

- `videos/NNN.mp4` — 올릴 영상
- `posts.json` — 예약표 (`at` = 한국시간). `post.yml` 이 10분마다 시간이 지난 것 하나를 릴스로 올린다
- `posted.json` — 올린 릴스 목록 (DM 감시 대상)
- `dm_sent.json` — DM 보낸 댓글 기록 (같은 댓글에 두 번 안 보냄)
- `config.json` — 인포크 주소·내 인스타 아이디·대가성 문구·공통 DM 키워드 (공개돼도 되는 것만)
- `dm.yml` 5분마다 댓글을 읽어 키워드가 있으면 버튼 카드 DM
- `refresh.yml` 매달 1일·15일 인스타 토큰 연장

Secrets: `IG_TOKEN`, `IG_USER_ID`, `GH_PAT`
