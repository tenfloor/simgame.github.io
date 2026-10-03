# 심게임 홈페이지 (Jekyll)

GitHub Pages가 자동으로 빌드합니다. 파일을 고쳐서 올리면 1~2분 뒤 반영됩니다.

## 내용 수정은 `_data` 폴더에서

| 파일 | 내용 |
|---|---|
| `_data/company.yml` | 회사명, 슬로건, 소개 문장, 주소, 전화, 이메일 |
| `_data/nav.yml` | 상단 메뉴 |
| `_data/business.yml` | 사업 분야 카드 |
| `_data/process.yml` | 개발 절차 |
| `_data/projects.yml` | 수행 실적 (`home: true`면 홈에도 표시) |
| `_data/products.yml` | 제품/솔루션 |

## 페이지

| 주소 | 파일 |
|---|---|
| `/` | `index.html` |
| `/business/` | `business.html` |
| `/projects/` | `projects.html` |
| `/products/` | `products.html` |
| `/contact/` | `contact.html` |

새 페이지를 만들려면 기존 페이지 파일을 복사해 `title`, `permalink`를 바꾸고 `_data/nav.yml`에 메뉴를 추가합니다.

## 디자인

- `assets/css/style.css` ─ 색상은 맨 위 `:root`의 변수(`--accent` 등)만 바꾸면 전체에 적용됩니다.
- `_includes/` ─ 상단 메뉴, 하단 정보, 카드 모양 등 공통 조각

## GitHub Pages에 올리기

1. GitHub에서 `simgame.github.io` 저장소를 만듭니다 (Public).
2. 이 폴더 안의 파일과 폴더를 **전부** 저장소에 업로드합니다 (`_data`, `_includes` 같은 밑줄 폴더 포함).
3. Settings → Pages → Source: `Deploy from a branch`, Branch: `main` / `(root)` → Save.
4. 1~2분 뒤 https://simgame.github.io 에서 확인합니다.

회사 도메인을 연결하면 `_config.yml`의 `url`을 그 주소로 바꿔 주세요.
