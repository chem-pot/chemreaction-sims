# 화학 시뮬레이션 모음 — 올리는 방법

## 폴더 구조
```
chem-sims/                  ← GitHub 저장소 하나
├─ index.html               ← 허브(목록) 페이지. 고칠 필요 없음
├─ sims.json                ← 과목·단원·시뮬레이션 목록 (관리 화면에서 만들어 덮어쓰기)
└─ sims/
   └─ hwabanse/             ← 과목 (화학 반응의 세계)
      └─ u2/                ← 2단원
         ├─ battery/index.html      ← 전지 실험
         └─ (다음 실험)/index.html
```
- 폴더 이름은 **영문·숫자**로 (한글이면 주소가 %EC%A0... 처럼 깨져 보여요)
- 시뮬레이션 파일 이름은 **index.html** 로 두면 주소가 `.../battery/` 로 깔끔해집니다

## 처음 한 번: GitHub Pages 켜기
1. GitHub에서 새 저장소 만들기 (예: `chem-sims`, **Public**)
2. `Add file → Upload files` 에 이 폴더 안의 내용물을 통째로 끌어다 놓고 Commit
3. `Settings → Pages → Source: Deploy from a branch → main / (root) → Save`
4. 1~2분 뒤 주소 생성: `https://아이디.github.io/chem-sims/`

## 생기는 링크 (예시)
| 무엇 | 주소 |
|---|---|
| 전체 목록 | `https://아이디.github.io/chem-sims/` |
| 화반세 과목 | `https://아이디.github.io/chem-sims/#/c/hwabanse` |
| 화반세 2단원 | `https://아이디.github.io/chem-sims/#/c/hwabanse/u/2` |
| 전지 실험 | `https://아이디.github.io/chem-sims/sims/hwabanse/u2/battery/` |

단원 페이지에 **링크 복사 / QR** 버튼이 있어서 클래스룸에 붙이거나 화면에 QR을 띄우면 됩니다.

## 새 시뮬레이션 추가할 때
1. GitHub에서 `sims/hwabanse/u2/` 로 들어가 `Add file → Upload files` → 새 폴더째 끌어다 놓기 (예: `electrolysis/index.html`)
2. 허브 페이지 맨 아래 **관리** → 해당 단원에 `+ 시뮬레이션 추가` → 제목, 경로(`sims/hwabanse/u2/electrolysis/`) 입력
3. **sims.json 내려받기** → GitHub 저장소 루트에 업로드해서 덮어쓰기
4. 1~2분 뒤 반영

## 이미 다른 곳(Vercel, 다른 저장소 등)에 올린 시뮬레이션
경로 칸에 `https://...` 전체 주소를 그대로 넣으면 됩니다. 파일을 옮기지 않아도 목록에 함께 정리돼요.

## 참고
- 관리 화면은 누구나 열 수 있지만, 고친 내용은 그 사람 브라우저에만 남고 공개 목록(sims.json)은 GitHub에 올린 사람만 바꿀 수 있어서 학생이 건드려도 문제없습니다.
- 각 시뮬레이션 안에 "목록으로 돌아가기" 링크를 넣고 싶으면 `<a href="../../../../#/c/hwabanse/u/2">← 2단원 목록</a>` 처럼 넣으면 됩니다.
