# LocationX 브로셔 사이트 (GitHub Pages)

BLE AoA 실시간 위치추적 솔루션 **LocationX**의 소개 브로셔 정적 사이트.
`index.html` 단일 파일로 구성되어 있으며 별도 빌드가 필요 없다.

## 게시 방법 (GitHub Pages)

1. GitHub에 저장소를 만든다 — 사용자 페이지로 쓰려면 `wshan1977.github.io`,
   프로젝트 페이지로 쓰려면 아무 이름(예: `locationx`)이나 가능.
2. 이 폴더 내용을 push:

   ```bash
   git init
   git add .
   git commit -m "LocationX 브로셔 사이트"
   git branch -M main
   git remote add origin https://github.com/wshan1977/<저장소이름>.git
   git push -u origin main
   ```

3. GitHub 저장소 → **Settings → Pages** → Source: `Deploy from a branch`,
   Branch: `main` / `(root)` 선택 → 저장.
4. 몇 분 뒤 `https://wshan1977.github.io/<저장소이름>/` 에서 확인.

## 이미지 넣기

`images/` 폴더에 아래 파일명으로 사진을 넣으면 페이지에 자동 표시된다
(없는 동안은 "이미지 준비 중" 플레이스홀더가 표시됨). 자세한 목록은
[images/README.md](images/README.md) 참고.

## 수정 포인트

- 태그 2종(Hart/Motion)의 상세 사양은 `index.html`의 `<!-- TODO -->` 주석
  위치에 채워 넣는다 (센서 사양, 착용/부착 형태, 배터리).
- 문의처(이메일·회사 정보)를 footer에 추가하려면 `<footer>` 블록을 수정.
