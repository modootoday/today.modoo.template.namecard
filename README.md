# 모두의오늘 온라인 명함 템플릿 사용 가이드

[![GitHub stars](https://img.shields.io/github/stars/modootoday/today.modoo.template.namecard.svg?style=social)](https://github.com/modootoday/today.modoo.template.namecard/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/modootoday/today.modoo.template.namecard.svg?style=social)](https://github.com/modootoday/today.modoo.template.namecard/network/members)
[![GitHub issues](https://img.shields.io/github/issues/modootoday/today.modoo.template.namecard.svg)](https://github.com/modootoday/today.modoo.template.namecard/issues)
[![GitHub license](https://img.shields.io/github/license/modootoday/today.modoo.template.namecard.svg)](https://github.com/modootoday/today.modoo.template.namecard/blob/main/LICENSE)

> 🌟 **데모 페이지**: [https://modootoday.github.io/today.modoo.template.namecard/](https://modootoday.github.io/today.modoo.template.namecard/)
> 
> 🔗 **GitHub 레포지토리**: [https://github.com/modootoday/today.modoo.template.namecard](https://github.com/modootoday/today.modoo.template.namecard)
> 
> 이 링크에서 온라인 명함 템플릿의 실제 모습을 확인하고 소스 코드를 볼 수 있습니다.

## 목차
1. [소개](#소개)
2. [GitHub 계정 생성](#1-github-계정-생성)
3. [온라인 명함 템플릿으로 레포지토리 생성](#2-모두의오늘-온라인-명함-템플릿으로-레포지토리-생성)
4. [명함 정보 설정](#3-_configyml-파일-수정하여-명함-정보-설정)
5. [온라인 명함 게시](#4-github-pages-활성화하여-온라인-명함-게시)
6. [주의사항](#주의사항)
7. [문제 해결 및 지원](#문제-해결-및-지원)

---

## 소개

모두의오늘 온라인 명함 템플릿은 GitHub Pages를 활용하여 누구나 쉽게 자신만의 디지털 명함을 만들 수 있도록 설계되었습니다. 이 가이드를 따라 단계별로 진행하면, 전문적이고 세련된 온라인 명함을 몇 분 안에 만들 수 있습니다.

---

## 1. GitHub 계정 생성

> 이미 GitHub 계정이 있다면 이 단계를 건너뛰세요.

1. [GitHub](https://github.com) 웹사이트에 접속합니다.
2. 우측 상단의 "Sign up" 버튼을 클릭합니다.
3. 다음 정보를 입력합니다:
   - 이메일 주소
   - 비밀번호 (강력한 비밀번호 사용 권장)
   - 사용자 이름 (영문, 숫자, 하이픈 사용 가능)
4. 이메일 수신 여부를 선택합니다.
5. 계정 인증 절차를 완료합니다:
   - "Verify account" 퍼즐 해결
   - 이메일로 전송된 인증 코드 입력
6. 계정 설정을 위한 추가 질문에 답하여 가입을 완료합니다.

---

## 2. 모두의오늘 온라인 명함 템플릿으로 레포지토리 생성

1. GitHub에 로그인합니다.
2. 모두의오늘 온라인 명함 템플릿 레포지토리로 이동합니다:
   **[https://github.com/modootoday/today.modoo.template.namecard](https://github.com/modootoday/today.modoo.template.namecard)**
3. 우측 상단의 "Use this template" 버튼을 클릭합니다.
4. "Create a new repository" 페이지에서:
   - **Owner**: 본인의 GitHub 계정 선택
   - **Repository name**: 원하는 이름 입력 (예: 'my-digital-namecard')
   - **Description**: (선택사항) 설명 추가
   - **Public/Private**: 공개 여부 선택
5. "Create repository from template" 버튼을 클릭하여 완료합니다.

---

## 3. _config.yml 파일 수정하여 명함 정보 설정

1. 생성된 레포지토리에서 '_config.yml' 파일을 찾아 클릭합니다.
2. 파일 편집 모드로 진입합니다. (연필 아이콘 클릭)
3. 다음 설정을 **신중히** 수정합니다:

```yaml
# Card settings (개인 정보로 수정하세요)
card:
  name: 홍길동  # 이름
  title: 소프트웨어 엔지니어  # 직함
  email: hong@example.com  # 이메일
  phone: 010-1234-5678  # 전화번호
  company: 테크 주식회사  # 회사명
  image: https://example.com/profile-image.jpg  # 프로필 이미지 URL

# Display settings (필요에 따라 true/false로 설정)
display:
  name: true
  title: true
  email: true
  phone: true
  company: true
```

**주의사항**:
- `image` URL은 반드시 실제 존재하는 이미지 주소여야 합니다.
- 공개를 원치 않는 정보는 `display` 설정을 `false`로 변경하거나 해당 정보를 비워두세요.
- 모든 정보는 정확하고 최신의 것이어야 합니다.

4. 변경사항을 꼼꼼히 검토한 후, "Commit changes" 버튼을 클릭하여 저장합니다.

---

## 4. GitHub Pages 활성화하여 온라인 명함 게시

1. 레포지토리 페이지에서 "Settings" 탭을 클릭합니다.
2. 좌측 사이드바에서 "Pages"를 선택합니다.
3. "Source" 섹션 설정:
   - "Deploy from a branch" 선택
   - "Branch": `main` 선택
   - 폴더: `/(root)` 선택
4. "Save" 버튼을 클릭합니다.
5. (선택사항) "Custom domain" 설정
6. "Enforce HTTPS" 옵션을 체크하여 보안 강화

> 설정 완료 후 GitHub가 사이트를 빌드하고 배포하는 데 몇 분이 소요될 수 있습니다.
> 배포가 완료되면 설정 페이지 상단에 표시되는 URL에서 귀하의 온라인 명함을 확인할 수 있습니다.
> 
> 📌 **참고**: 귀하의 온라인 명함은 데모 페이지([https://modootoday.github.io/today.modoo.template.namecard/](https://modootoday.github.io/today.modoo.template.namecard/))와 유사한 형태로 보이게 됩니다. 단, 귀하의 개인 정보로 채워진 상태입니다.

---

## 주의사항

- 📝 _config.yml 파일 수정 후 변경사항 적용에 최대 10분 소요될 수 있습니다.
- 🔒 개인정보 보호에 유의하세요. 공개하고 싶지 않은 정보는 입력하지 마세요.
- 🖼️ 프로필 이미지는 전문적이고 적절한 것을 선택하세요.
- 🔄 정기적으로 정보를 업데이트하여 항상 최신 상태를 유지하세요.
- 🌐 GitHub Pages URL은 `https://<username>.github.io/<repository-name>`
  형식입니다.

---

## 문제 해결 및 지원

- 📘 자세한 GitHub Pages 사용법은 [공식 문서](https://docs.github.com/en/pages)를 참조하세요.
- ❓ 템플릿 사용 중 문제가 발생하면 [Issues 페이지](https://github.com/modootoday/today.modoo.template.namecard/issues)에 
  질문을 올려주세요.
- 💡 기능 제안이나 개선 아이디어가 있다면 [Pull Request](https://github.com/modootoday/today.modoo.template.namecard/pulls)를 
  제출해 주세요.
- 🆘 긴급한 도움이 필요하다면 모두의오늘 커뮤니티에 문의하세요.

---

**🎉 축하합니다!** 이 가이드를 따라 설정하면 "모두의오늘 온라인 명함 템플릿"을 사용하여 전문적이고 효과적인 온라인 명함을 쉽게 만들 수 있습니다. 완성된 명함은 데모 페이지와 유사하지만, 귀하의 고유한 정보로 채워진 상태일 것입니다.

**🔗 중요 링크**:
- 데모 페이지: [https://modootoday.github.io/today.modoo.template.namecard/](https://modootoday.github.io/today.modoo.template.namecard/)
- GitHub 레포지토리: [https://github.com/modootoday/today.modoo.template.namecard](https://github.com/modootoday/today.modoo.template.namecard)

[![GitHub stars](https://img.shields.io/github/stars/modootoday/today.modoo.template.namecard.svg?style=social)](https://github.com/modootoday/today.modoo.template.namecard/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/modootoday/today.modoo.template.namecard.svg?style=social)](https://github.com/modootoday/today.modoo.template.namecard/network/members)

이 프로젝트가 마음에 드신다면, GitHub에서 스타를 눌러주세요! 👆
