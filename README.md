# Ygrail.github.io

Sungbae Yoon (윤성배) 개인 사이트 — Jekyll + GitHub Pages, https://ygrail.github.io

## 배포

1. GitHub에 `Ygrail.github.io` 이름으로 저장소를 새로 만든다. (계정명과 정확히 같아야 루트 도메인으로 서비스됨)
2. 이 폴더에서:

```bash
git init && git add . && git commit -m "Initial site" && git branch -M main && git remote add origin https://github.com/Ygrail/Ygrail.github.io.git && git push -u origin main
```

3. 저장소 **Settings → Pages → Source**를 `Deploy from a branch` / `main` / `/ (root)`로 둔다.
4. 1~2분 뒤 https://ygrail.github.io 에서 확인.

## 커스텀 도메인 (나중에 붙일 때)

루트에 도메인만 한 줄 적은 `CNAME` 파일을 만들고, `_config.yml`의 `url`과 `robots.txt`의 sitemap 주소를 같이 바꾼다.
그리고 도메인 등록기관 DNS에 아래 레코드를 넣는다 (호스트 `@` = 도메인 자체).

| 타입 | 호스트 | 값 |
| --- | --- | --- |
| A | @ | `185.199.108.153` |
| A | @ | `185.199.109.153` |
| A | @ | `185.199.110.153` |
| A | @ | `185.199.111.153` |
| AAAA | @ | `2606:50c0:8000::153` |
| AAAA | @ | `2606:50c0:8001::153` |
| AAAA | @ | `2606:50c0:8002::153` |
| AAAA | @ | `2606:50c0:8003::153` |
| CNAME | www | `ygrail.github.io.` |

그 다음 저장소 **Settings → Pages → Custom domain**에 도메인을 넣고 저장, DNS 검증이 끝나면 **Enforce HTTPS**를 켠다 (인증서 발급까지 최대 24시간).

확인:

```bash
nslookup 도메인
```

A 레코드가 위 4개로 보이면 정상.

## 증빙 자료 (수상 증명서 · 교육 자료) 올리기

파일을 `assets/files/` 에 넣기만 하면 된다. `index.md`가 쓰는 `evidence.html` include는
**해당 파일이 저장소에 실제로 있을 때만** 링크를 만들기 때문에, 파일이 없는 동안에는
아무것도 안 보이고 깨진 링크도 생기지 않는다.

지금 연결돼 있는 경로 두 개:

| 넣을 파일 | 표시되는 곳 |
| --- | --- |
| `assets/files/hacktheon2024.png` | CTF Awards → Hacktheon 항목의 `Certificate →` |
| `assets/files/hackhu-system-hacking.pdf` | Experience → HACKHU 항목의 `Slides →` |

다른 자료를 더 붙이고 싶으면 원하는 위치에 이 한 줄을 넣는다.

```liquid
{% include evidence.html path="/assets/files/파일명.pdf" en="Report →" ko="자료 →" %}
```

권장 사항:

- 증명서·상장은 PNG/JPG, 발표·교육 자료는 PDF로. 파일 하나당 10MB 이하가 무난하다 (GitHub는 100MB 초과 시 거부).
- 공개 저장소이므로 **이름·학번·주민번호 뒷자리·서명·연락처는 가리고** 올린다.
- 파일명은 영문 소문자와 하이픈으로 (한글 파일명은 URL이 지저분해진다).

## 로컬 미리보기

Ruby가 있으면:

```bash
bundle install && bundle exec jekyll serve
```

→ http://127.0.0.1:4000

## 구조

| 경로 | 역할 |
| --- | --- |
| `index.md` | 메인(whoami) 페이지 — 소개, quick info, 연구 관심사, 학력, 논문, 프로젝트, 활동, 스킬, personal |
| `portfolio.md` | 연구/프로젝트/활동 상세 페이지 (`/portfolio/`) |
| `_includes/header.html` | 상단 네비게이션 + EN/KR 스위치 |
| `_includes/externals/scripting.html` | 언어 토글 스크립트 |
| `assets/css/main.css` | 구조 + 터미널 테마. 색은 맨 위 `:root` 변수만 바꾸면 한 번에 바뀜 |
| `assets/css/theme-navy.css` | 라이트 네이비 테마 (main.css 위에 덧씌워짐) |
| `assets/img/profile.png` | **프로필 사진을 여기에 넣으면** 메인 상단에 자동 표시 |
| `assets/img/profile-chalice.svg` | 위 파일이 없을 때 쓰이는 성배 아이콘 (직접 그린 대체본) |

## 테마 전환

`_config.yml` 한 줄로 두 테마를 바꾼다. 마크업은 그대로 두고 CSS와 몇몇 라벨만 달라진다.

```yaml
theme_variant: navy       # 라이트 + 세리프 + 네이비 (현재 기본값)
theme_variant: terminal   # 다크 + 모노스페이스
```

| | `terminal` | `navy` |
| --- | --- | --- |
| 배경 / 악센트 | `#0f1115` / `#7ee787` | `#fbfcfe` / `#1e3a8a` |
| 제목 폰트 | JetBrains Mono | Source Serif 4 |
| 헤더 | `sbyoon@siftlab:~$` · `~/whoami` | `Sungbae Yoon` · `About` |
| 섹션 제목 | `// quick_info` | `Quick Info` |
| 히어로 | 터미널 창 (`$ whoami`, `$ cat about.md`) | 터미널 장식 없이 이름 + About |

## 수정할 때

### 색 바꾸기

`main.css`(터미널) 또는 `theme-navy.css`(네이비) 맨 위 `:root`의 `--accent`만 바꾸면 링크·강조·아이콘·타임라인 점이 전부 따라온다.

### 섹션 추가

섹션 제목은 두 테마가 같은 태그를 나눠 쓴다. 안쪽 텍스트는 터미널 테마용 슬러그, `data-label`은 네이비 테마용 제목이다. **둘 다 채워야** 네이비에서 제목이 보인다.

```html
<h2 class="sec__title" data-label="Talks">talks</h2>
```

### EN/KR 번역 추가

텍스트 요소에 `data-en` / `data-ko` 두 속성을 같이 달면 헤더 스위치로 전환된다. 안쪽 기본 텍스트는 JS가 꺼져 있을 때 보이는 값이므로 셋 다 채워두는 게 좋다.

```html
<p data-en="Security Researcher" data-ko="보안 연구자">Security Researcher</p>
```

속성 값 안에 태그를 넣을 때는 작은따옴표를 쓴다: `data-ko="<strong>안드로이드</strong> 보안"`.

### 포트폴리오 항목 추가

`portfolio.md`의 `pf-project` 블록을 복사해서 `id`, 제목, 기간, 설명, 태그를 바꾼다.
메인에서 바로 링크하려면 `index.md` 쪽에 `/portfolio/#해당-id`로 걸면 된다.

## 크레딧

구조는 [Pudhina](https://github.com/knhash/Pudhina) 계열 Jekyll 구성을 참고했고, 테마(다크 터미널)는 이 저장소에서 새로 작성했다. MIT License.
