# GitHub 업로드 & 배포 방법

이 폴더 전체가 배포 가능한 GitHub 저장소입니다.
아래 순서대로 하면 웹페이지로 공개됩니다.

## 1단계 · 파일 채워넣기

- `docs/` 폴더에 소개 자료를 넣고 파일명을 `introduction.pdf` 로 맞춥니다.
  (PPT라면 PDF로 저장해서 넣는 걸 추천 — 웹에서 미리보기가 됩니다.)
- `videos/` 폴더에 소개 영상을 넣고 파일명을 `intro.mp4` 로 맞춥니다.
- `index.html` 과 `README.md` 를 열어 아래 항목을 실제 값으로 바꿉니다.
  - 프로젝트 이름 / 한 줄 소개
  - 웹 링크 주소 (https://example.com)
  - 앱 링크 주소 (https://example.com/app)

> 파일명을 바꾸면 index.html 안의 경로도 함께 바꿔주세요.

## 2단계 · GitHub에 올리기 (웹에서 드래그 앤 드롭)

1. github.com 로그인 → 우측 상단 **+** → **New repository**
2. 저장소 이름 입력 → **Public** 선택 → **Create repository**
3. 새로 생긴 저장소 페이지에서 **uploading an existing file** 클릭
4. 이 폴더 안의 파일/폴더를 통째로 드래그해서 올림 → **Commit changes**

## 3단계 · GitHub Pages로 배포 (웹페이지로 공개)

1. 저장소 → **Settings** → 왼쪽 메뉴 **Pages**
2. **Source** 를 `Deploy from a branch` 로 두고, Branch 를 `main` / `/(root)` 선택 → **Save**
3. 1~2분 뒤 `https://<사용자이름>.github.io/<저장소이름>/` 주소로 공개됩니다.

## 참고 · 큰 영상 파일

- GitHub 일반 업로드는 파일당 최대 100MB 입니다.
- MP4가 100MB를 넘으면 Git LFS를 쓰거나, 영상만 YouTube/Vimeo에 올리고
  `index.html` 의 `<video>` 부분을 해당 링크 카드로 바꾸는 방법이 있습니다. 알려주시면 그 형태로 바꿔드릴게요.
