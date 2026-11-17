# Lococo 회사 소개 홈페이지

주소: **https://company.lococo.beauty** (GitHub Pages)
쇼핑몰 lococo.beauty 와는 별개인 **회사 소개 사이트**입니다. 독자는 브랜드(B2B)·언론·투자자·지원자.

## 글 고치는 법 (GitHub 화면에서, 설치 없음)

1. 고칠 파일을 연다 (아래 표) → 오른쪽 위 연필(✏️ Edit) 버튼.
2. 고친다 → 아래 **Commit changes** → 메시지 한 줄(예: "브랜드 페이지 문구 수정") → **Commit directly to the main branch**.
3. 1~2분 뒤 사이트에 반영된다. 진행 상황은 저장소 위 **Actions** 탭 (초록 체크 = 끝).

### 되돌리기
- 저장소 위 **Commits**(시계 아이콘) → 되돌릴 커밋 → 오른쪽 `…` → **Revert** → 커밋. 그 전 상태로 다시 배포됩니다.
- 파일 하나의 예전 내용을 보려면 파일 열고 **History**.

## 어디를 고치나

| 바꾸고 싶은 것 | 파일 |
|---|---|
| 첫 화면 문장, '하는 일' 3개, 슬로건 아래 문장 | `index.md` (영어) · `ko/index.md` (한국어) — 위쪽 `---` 사이 |
| 회사 소개 | `about.md` · `ko/about.md` |
| 브랜드 파트너십 | `brands.md` · `ko/brands.md` |
| 프로젝트 카드 | `_data/projects.yml` (영어·한국어 같이) |
| 소식·보도 목록 | `_data/news.yml` |
| 첫 화면 숫자 4개 | `_data/stats.yml` |
| 연혁 | `_data/timeline.yml` |
| 함께한 브랜드·판매 브랜드 | `_data/partners.yml` |
| 팀 | `_data/team.yml` (사진은 `assets/img/` 에 올리고 파일명 적기) |
| 메일 주소·SNS·회사 소개서 링크·법인 주소 | `_data/site.yml` |
| 메뉴·버튼 이름 | `_data/strings.yml` |
| 모양·색 | `assets/css/style.css` (Lococo Blue `#2966FF`) |

- 영어 페이지는 루트, 한국어 페이지는 `ko/` 폴더. 둘은 따로 고칩니다.
- `_data/*.yml` 은 **들여쓰기(칸 수)와 따옴표**를 그대로 두고 글자만 바꾸세요. 틀리면 Actions 가 빨간 ✕ 가 되고 사이트는 이전 상태로 남습니다 → Revert 하거나 고쳐서 다시 커밋.
- 사진: `assets/img/` 에 올리기 (GitHub 화면 **Add file → Upload files**). 2MB 아래 권장.

## 쓰지 말 것
- 개인 전화번호, 개인 메일, 계약 조건·가격. 이 사이트는 누구나 봅니다.
- IR 자료의 미확정 숫자. 숫자는 회사 소개서(외부 전달용)에 있는 것만.

## 구조 (개발자용)
- Jekyll(GitHub Pages 기본). 플러그인은 jekyll-seo-tag · jekyll-sitemap 만.
- `_layouts/home.html` 첫 화면, `_layouts/page.html` 나머지, `_includes/` 조각, `_data/` 목록.
- 배포: `.github/workflows/pages.yml` — main 에 커밋되면 빌드 → Pages.
- 로컬 미리 보기: `bundle install && bundle exec jekyll serve` → http://localhost:4000

## 도메인
GitHub → Settings → Pages → Custom domain 에 `company.lococo.beauty`, DNS 에 `company CNAME team-lococo.github.io`. 적용 뒤 **Enforce HTTPS** 체크.
