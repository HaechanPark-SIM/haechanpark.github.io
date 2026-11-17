# Haechan Park 홈페이지 — GitHub Pages 배포 가이드

이 폴더의 내용이 **그대로 GitHub 저장소의 최상위(root)** 에 들어가야 합니다. ZIP 파일 자체를 올리는 것이 아닙니다.

## 1. GitHub 저장소 만들기 (최초 1회)

1. https://github.com 에 로그인하고 우측 위 **+ → New repository** 클릭
2. 저장소 이름은 **`내GitHub아이디.github.io`** 로 입력합니다. 예: 아이디가 `haechanpark`이면 `haechanpark.github.io`
3. 무료 플랜에서는 **Public**으로 생성합니다. GitHub에 로그인하지 않은 사람도 사이트를 볼 수 있습니다.
4. **Create repository** 클릭 (Add a README file은 선택하지 않아도 됩니다.)

다른 저장소 이름(예: `academic-website`)을 사용해도 됩니다. 이 경우 주소는 `https://내GitHub아이디.github.io/academic-website/`입니다.

## 2. 홈페이지 파일 올리기 (최초 1회)

1. 다운받은 `Haechan_Park_GitHub_Pages.zip`을 **압축 해제**합니다.
2. 생성한 GitHub 저장소의 **Add file → Upload files** 로 이동합니다.
3. 압축 해제한 폴더 **안의 내용** (5개 HTML 파일, `assets` 폴더, `.nojekyll`, README 및 가이드)을 업로드합니다. 파일이 ZIP 하나로 올라가면 사이트는 작동하지 않습니다. `index.html`이 저장소 첫 화면에 보여야 합니다.
4. 아래 **Commit changes** 클릭. 브랜치는 `main`을 사용합니다.

`assets` 폴더 구조까지 정확히 업로드해야 합니다. 브라우저에서 폴더 업로드가 어려우면 [GitHub Desktop](https://desktop.github.com/)을 설치하고 저장소를 Clone한 다음, 압축 해제 파일을 복사해 Commit/Push 하세요.

## 3. GitHub Pages 켜기 (최초 1회)

1. 저장소 상단 **Settings** → 왼쪽 **Pages**
2. **Build and deployment → Source** 에서 **Deploy from a branch** 선택
3. **Branch**에서 `main`, 폴더에서 **`/ (root)`** 선택 후 **Save**
4. 잠시 뒤 Pages 화면의 **Visit site** 버튼으로 홈페이지를 열어봅니다. 첫 배포나 업데이트는 몇 분 걸릴 수 있으며 GitHub 문서에는 최대 10분 정도까지 안내되어 있습니다.

저장소 이름을 `내GitHub아이디.github.io`로 했다면 사이트 주소는:

`https://내GitHub아이디.github.io/`

## 4. 이후 수정하면 자동 반영

- **간단한 글 수정:** GitHub 저장소 → 해당 HTML 파일 선택 → 연필(**Edit this file**) → 텍스트 수정 → **Commit changes**. Github Pages가 자동 재배포됩니다.
- **논문 추가:** `assets/site.js`를 열어 `const publications` 배열 항목을 수정 후 Commit합니다.
- **캐러셀 사진 변경:** 새 이미지를 `assets/`에 올리고 `index.html`의 `src="assets/파일이름.png"` 부분을 바꿔 Commit합니다.
- **색상 변경:** `assets/site.css`에서 `--accent: #3d5082`를 수정합니다.
- **전체 디자인 수정:** ChatGPT에서 새 버전을 만들면 해당 파일을 GitHub 저장소의 동일 경로에 덮어쓴 뒤 Commit합니다. (GitHub Desktop을 쓰면 여러 파일 변경이 편합니다.)

⚠️ **중요:** 컴퓨터에 있는 파일만 수정하면 공개 사이트는 바뀌지 않습니다. GitHub 저장소에 **Commit(또는 Push)** 해야 변경됩니다.

## 5. 자주 생기는 문제

- **404 오류:** `index.html`이 저장소 최상위에 있는지, Settings → Pages의 `main / (root)` 설정이 맞는지 확인합니다.
- **이미지가 안 나옴:** `assets/` 폴더가 빠지지 않았는지, 이미지 파일 이름(대문자·소문자 포함)이 정확한지 확인합니다.
- **메뉴가 안 움직임:** `assets/site.js` 파일이 업로드되어 있는지 확인합니다.
- **수정이 반영되지 않음:** Commit 여부, **Actions** 탭의 Pages 배포 결과를 확인하고 몇 분 후 새로고침합니다.

## 6. 주요 파일

```
index.html                 # 홈 캐러셀
haechan-park.html          # 프로필
research-interests.html    # 연구 소개
publications.html          # 논문 목록
gallery.html               # 갤러리
assets/site.css            # 메인 색상과 스타일
assets/site.js             # 캐러셀·논문 필터·갤러리 동작, 논문 데이터
assets/*.svg               # 교체 가능한 연구 소개 이미지
.nojekyll                  # GitHub Pages 정적 파일 설정
```

공개 전에 약력·연락처·논문 정보·연구 이미지 사용 권한을 확인하세요. 현재 주요 연구 이미지는 실제 논문 Figure가 아닌 예시 일러스트입니다.
