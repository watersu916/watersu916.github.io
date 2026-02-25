# 🚀 GitHub Pages 배포 가이드

이 멋진 윤슬 포트폴리오를 `https://<사용자이름>.github.io` 주소로 배포하는 방법입니다.

## 1단계: GitHub 저장소 만들기
1. [GitHub](https://github.com/new)로 이동합니다.
2. **Repository name**에 `사용자이름.github.io`를 입력합니다. (예: `hong-gildong.github.io`)
   * *반드시 본인의 GitHub ID와 일치해야 자동으로 기본 도메인 배포가 됩니다.*
3. 나머지 설정은 기본값으로 두고 **Create repository**를 클릭합니다.

## 2단계: 로컬 코드 연결 및 업로드
터미널(PowerShell)을 열고 아래 명령어를 순서대로 입력하세요.

```powershell
# 1. 원격 저장소 주소 설정 (브라우저 주소창에서 복사하세요)
git remote add origin https://github.com/<사용자이름>/<사용자이름>.github.io.git

# 2. 메인 브랜치 이름 확인 (기본적으로 main 혹은 master입니다)
git branch -M main

# 3. GitHub로 업로드
git push -u origin main
```

## 3단계: 배포 확인
1. GitHub 저장소의 **Settings** 탭으로 이동합니다.
2. 왼쪽 메뉴에서 **Pages**를 클릭합니다.
3. `Your site is live at...` 라는 메시지와 함께 생성된 URL을 확인하세요.
4. 이제 전 세계 어디서든 본인의 포트폴리오에 접속할 수 있습니다!

---
✨ **Tip**: 나중에 내용을 수정하고 싶다면, `index.html`을 고친 후 아래 명령어를 반복하면 됩니다:
```powershell
git add .
git commit -m "Update portfolio content"
git push origin main
```
