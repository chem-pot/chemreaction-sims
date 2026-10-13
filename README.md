# 케미작렬 시뮬레이션 — 올리는 방법

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
| 첫 화면 (두 과목) | `https://chem-pot.github.io/chemreaction-sims/` |
| 화학 반응의 세계 2단원 | `https://chem-pot.github.io/chemreaction-sims/#/hwabanse/2` |
| 물질과 에너지 1단원 | `https://chem-pot.github.io/chemreaction-sims/#/mulen/1` |
| 전지 실험 | `https://chem-pot.github.io/chemreaction-sims/sims/u2/battery/` |

(예전 주소 `#/u/2`도 화학 반응의 세계 2단원으로 연결됩니다.)

## 새 시뮬레이션 추가
1. GitHub에 시뮬레이션 폴더 올리기 — 추천 위치: `sims/hwabanse/u1/실험이름/index.html`, `sims/mulen/u3/실험이름/index.html`
2. 사이트 맨 아래 **관리** → 해당 단원 `+ 시뮬레이션 추가` → 제목, 경로 입력
3. **sims.json 내려받기** → 저장소 루트에 덮어쓰기 → 1~2분 뒤 반영

다른 곳에 올린 시뮬레이션은 경로 칸에 `https://...` 전체 주소를 넣으면 됩니다.
단원 이름 앞의 번호(Ⅰ., 1.)는 화면에서 자동으로 "1단원"으로 바뀌어 보이고, 괄호 숫자는 등록된 시뮬레이션 개수입니다.
