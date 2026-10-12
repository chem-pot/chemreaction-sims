# 화학 반응의 세계 시뮬레이션 — 올리는 방법

## 폴더 구조
```
(저장소 루트)
├─ index.html          ← 목록 페이지 (고칠 필요 없음)
├─ sims.json           ← 단원·시뮬레이션 목록 (관리 화면에서 만들어 덮어쓰기)
├─ assets/             ← 로고, 테두리 이미지
└─ sims/
   └─ u2/              ← 2단원
      ├─ battery/index.html   ← 전지 실험
      └─ (다음 실험)/index.html
```
- 폴더 이름은 영문·숫자로, 시뮬레이션 파일 이름은 index.html 로.

## 링크
| 무엇 | 주소 |
|---|---|
| 화학 반응의 세계 (단원 목록) | `https://chem-pot.github.io/chemreaction-sims/` |
| 2단원 | `https://chem-pot.github.io/chemreaction-sims/#/u/2` |
| 전지 실험 | `https://chem-pot.github.io/chemreaction-sims/sims/u2/battery/` |

## 새 시뮬레이션 추가
1. GitHub에서 `sims/u2/` 로 들어가 Add file → Upload files 로 새 폴더째 올리기 (예: `electrolysis/index.html`)
2. 사이트 맨 아래 **관리** → 단원에 `+ 시뮬레이션 추가` → 제목, 경로(`sims/u2/electrolysis/`) 입력
3. **sims.json 내려받기** → 저장소 루트에 올려 덮어쓰기 → 1~2분 뒤 반영

다른 곳에 올린 시뮬레이션은 경로 칸에 `https://...` 전체 주소를 넣으면 됩니다.

## 화학(2학년) 사이트를 따로 만들 때
이 저장소 내용을 그대로 새 저장소(예: `chem-sims`)에 올리고, 관리 화면에서 과목 이름과 단원만 바꿔서 sims.json을 덮어쓰면 됩니다.
