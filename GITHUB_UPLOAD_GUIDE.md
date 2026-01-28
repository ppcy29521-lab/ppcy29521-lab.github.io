# GitHub Pages 업로드 가이드

## 📤 파일 업로드 방법

### 방법 1: GitHub 웹사이트에서 직접 업로드 (가장 쉬움)

1. **GitHub 저장소로 이동**
   - 브라우저에서 `https://github.com/ppcy29521-lab/ppcy29521-lab.github.io` 접속
   - (또는 본인의 저장소 이름으로 접속)

2. **파일 업로드**
   - 저장소 페이지에서 **"Add file"** → **"Upload files"** 클릭
   - 또는 드래그 앤 드롭으로 파일을 올릴 수 있습니다

3. **업로드할 파일들**
   ```
   📁 루트 폴더:
   - index.html (필수!)
   - data.json
   - README.md (선택사항)
   
   📁 assets 폴더:
   - assets/background.png
   - assets/center-photo.png
   - assets/map.png
   ```

4. **커밋 및 푸시**
   - 파일을 업로드한 후 하단에 커밋 메시지 입력 (예: "웹사이트 업로드")
   - **"Commit changes"** 버튼 클릭
   - 몇 분 후 `https://ppcy29521-lab.github.io` 에서 확인 가능

---

### 방법 2: GitHub Desktop 사용

1. **GitHub Desktop 다운로드**
   - https://desktop.github.com/ 에서 다운로드

2. **저장소 클론**
   - GitHub Desktop에서 저장소 클론 또는 열기

3. **파일 복사**
   - 로컬 저장소 폴더에 `index.html`, `data.json`, `assets` 폴더 복사

4. **커밋 및 푸시**
   - GitHub Desktop에서 변경사항 확인
   - 커밋 메시지 입력 후 "Commit to main"
   - "Push origin" 클릭

---

### 방법 3: Git 명령어 사용 (터미널)

```bash
# 저장소 클론 (처음 한 번만)
git clone https://github.com/ppcy29521-lab/ppcy29521-lab.github.io.git
cd ppcy29521-lab.github.io

# 파일 복사 후
# index.html, data.json, assets 폴더를 이 폴더에 복사

# 변경사항 추가
git add .

# 커밋
git commit -m "웹사이트 업로드"

# 푸시
git push origin main
```

---

## 📝 중요 사항

### ✅ 반드시 확인할 것들:

1. **파일 이름 확인**
   - 반드시 `index.html` 이어야 합니다 (대소문자 구분)
   - `test.html`이 아닙니다!

2. **폴더 구조**
   ```
   저장소 루트/
   ├── index.html
   ├── data.json
   ├── README.md
   └── assets/
       ├── background.png
       ├── center-photo.png
       └── map.png
   ```

3. **GitHub Pages 설정 확인**
   - 저장소 → Settings → Pages
   - Source: `Deploy from a branch`
   - Branch: `main` (또는 `master`)
   - Folder: `/ (root)`

4. **배포 시간**
   - 파일 업로드 후 **1-5분** 정도 기다려야 합니다
   - 첫 배포는 더 오래 걸릴 수 있습니다

---

## 🔄 업데이트 방법

### 공지사항이나 갤러리 수정 후:

1. **관리자 모드로 로그인**
   - 웹사이트에서 "관리자 로그인" 클릭
   - ID: `pcy6848`, PW: `psj@30303`

2. **내용 수정**
   - 공지사항 추가/수정/삭제
   - 갤러리 사진 추가/수정/삭제

3. **JSON 다운로드**
   - 수정 후 "📥 JSON 다운로드" 버튼 클릭
   - `data.json` 파일이 다운로드됩니다

4. **GitHub에 업로드**
   - 방법 1, 2, 3 중 하나로 `data.json` 파일을 GitHub에 업로드
   - 기존 `data.json` 파일을 새로 다운로드한 파일로 교체

5. **확인**
   - 몇 분 후 웹사이트 새로고침하여 변경사항 확인

---

## 🖼️ 이미지 추가 방법

### 갤러리에 이미지 추가:

1. **이미지 파일 준비**
   - 이미지 파일 (JPG, PNG 등)

2. **GitHub에 이미지 업로드**
   - 저장소에 `assets/images/` 폴더 생성 (없으면)
   - 이미지 파일을 `assets/images/` 폴더에 업로드

3. **이미지 URL 확인**
   - 업로드 후 이미지 파일 클릭
   - "Download" 버튼 옆의 "..." 메뉴 → "Copy path" 클릭
   - 또는 직접 URL 확인: `https://ppcy29521-lab.github.io/assets/images/파일명.jpg`

4. **갤러리에 추가**
   - 관리자 모드로 로그인
   - "사진 추가" 클릭
   - 이미지 URL 입력 (예: `https://ppcy29521-lab.github.io/assets/images/photo1.jpg`)
   - 저장 후 JSON 다운로드하여 GitHub에 업로드

---

## ❓ 문제 해결

### 웹사이트가 안 보여요
- `index.html` 파일 이름 확인 (대소문자 정확히)
- GitHub Pages 설정 확인 (Settings → Pages)
- 몇 분 더 기다려보기

### 이미지가 안 보여요
- 이미지 URL이 정확한지 확인
- `https://` 로 시작하는지 확인
- GitHub에 이미지 파일이 업로드되었는지 확인

### 변경사항이 반영이 안 돼요
- 브라우저 캐시 삭제 (Ctrl+F5 또는 Cmd+Shift+R)
- 시크릿 모드로 확인
- GitHub에 파일이 제대로 업로드되었는지 확인

---

## 📞 도움이 필요하시면

- GitHub Pages 문서: https://docs.github.com/pages
- 저장소 Issues 탭에서 질문 가능
