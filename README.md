# CCZ-CROSS 티스토리 스킨

![CCZ-CROSS](https://img.shields.io/badge/version-1.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Tistory](https://img.shields.io/badge/platform-Tistory-orange.svg)

CCZ-CROSS는 다양한 글을 여러 기기에서 읽기 좋게 보여주는 티스토리 블로그 스킨입니다. 심플하고 클래식한 테마를 반응형으로 제공하며, 크로스브라우징을 지원하여 다양한 브라우저 환경에서 최적의 사용자 경험을 제공합니다.

- **데모페이지**: [http://ccz-cross.tistory.com](http://ccz-cross.tistory.com)
- **설정 가이드**: [http://webdir.tistory.com/491](http://webdir.tistory.com/491)
- **제작자**: [흉내쟁이 (COPYCATZ)](http://copycatz.tistory.com)
- **업데이트**: [HANBANGA](https://thesauro.tistory.com/)

---

## 📋 목차

- [프로젝트 개요](#프로젝트-개요)
- [특징](#특징)
- [브라우저 지원](#브라우저-지원)
- [기술 스택](#기술-스택)
- [파일 구조](#파일-구조)
- [설치 방법](#설치-방법)
- [테마 커스터마이징](#테마-커스터마이징)
- [라이선스](#라이선스)

---

## 🎯 프로젝트 개요

### 스킨 정보

| 항목 | 내용 |
|------|------|
| **스킨 이름** | CCZ-CROSS |
| **버전** | 1.0 |
| **제작자** | 흉내쟁이 (COPYCATZ) |
| **홈페이지** | http://copycatz.tistory.com |
| **이메일** | uzugoer@gmail.com |
| **라이선스** | MIT License |
| **업데이트** | HANBANGA (https://thesauro.tistory.com/) |

### 목적

CCZ-CROSS 스킨은 다음과 같은 목적으로 제작되었습니다:

- **크로스브라우징**: 다양한 브라우저와 운영체제에서 일관된 디자인 제공
- **반응형 디자인**: 모바일, 태블릿, 데스크탑 등 다양한 디바이스 지원
- **사용자 경험 향상**: 직관적인 네비게이션과 깔끔한 레이아웃
- **커스터마이징 용이성**: CSS Custom Properties를 통한 쉬운 테마 변경

---

## ✨ 특징

### 주요 기능

- 🎨 **클래식한 테마**: 심플하고 세련된 디자인
- 📱 **반응형 디자인**: 모바일, 태블릿, 데스크탑 지원
- 🌓 **라이트/다크 모드**: 사용자 시스템 설정에 따른 자동 테마 전환 및 수동 전환 지원
- ⚙️ **옵션 설정**: 스킨 설정을 통한 기능 ON/OFF 가능
- 📝 **서식 스타일**: 글 작성시 도움이 될만한 다양한 서식 제공
- 🎯 **크로스브라우징**: IE7부터 최신 브라우저까지 광범위한 지원

### 디자인 특징

- **썸네일 지원**: 글 목록에서 썸네일 이미지 표시
- **카테고리 네비게이션**: 계층형 카테고리 구조 지원
- **검색 기능**: 실시간 태그 검색 지원
- **방명록**: 말풍선 스타일의 방명록 UI
- **댓글 시스템**: 계층형 댓글 및 답글 지원

---

## 🌐 브라우저 지원

### 데스크탑 브라우저

| 브라우저 | 지원 버전 |
|----------|-----------|
| Internet Explorer | 7, 8, 9, 11 |
| Firefox | 최신 버전 |
| Chrome | 최신 버전 |
| Opera | 최신 버전 |

### 모바일 브라우저

| 플랫폼 | 브라우저 | 지원 버전 |
|--------|----------|-----------|
| iOS | Safari | 전체 |
| Android | 내장 브라우저 | 2.3.x 이상 |
| Android | Chrome | 전체 |

---

## 🔧 기술 스택

### 핵심 기술

- **HTML5**: 시맨틱 마크업 사용
- **CSS3**: 
  - CSS Custom Properties (CSS Variables) 사용
  - Flexbox 레이아웃
  - 미디어 쿼리를 통한 반응형 디자인
  - 그리드 시스템
- **JavaScript**:
  - jQuery 3.7.1 (의존성)
  - jQuery Migrate 3.4.1
  - 커스텀 플러그인 (plugins.js, main.js)

### CSS Custom Properties

스킨은 CSS Custom Properties를 적극적으로 사용하여 테마 커스터마이징을 용이하게 합니다.

```css
:root,
[data-theme="light"] {
    /* 배경색 */
    --bg-body: #f8f8f8;
    --bg-content: #fff;
    --bg-sidebar: #f8f8f8;
    --bg-header: #333;
    
    /* 텍스트색 */
    --text-primary: #555;
    --text-secondary: #777;
    --text-heading: #222;
    
    /* 강조색 */
    --color-primary: #81a9db;
    --color-success: #91CCAA;
    --color-warning: #f0ad4e;
    --color-danger: #FC9F8A;
    
    /* 테두리색 */
    --border-color: #dedede;
    --border-light: #eee;
}

[data-theme="dark"] {
    /* 다크 모드용 변수 */
    --bg-body: #1a1a1a;
    --bg-content: #242424;
    --text-primary: #d0d0d0;
    --color-primary: #8fb5e3;
    /* ... */
}
```

---

## 📁 파일 구조

```
CCZ-CROSS/
├── images/                          # 이미지 및 리소스 폴더
│   ├── admin_48.svg                 # 관리자 아이콘
│   ├── anonymous_48.svg             # 익명 사용자 아이콘
│   ├── bg.svg                       # 배경 패턴 (육각형)
│   ├── cczicon.eot                  # 아이콘 폰트 (EOT)
│   ├── cczicon.svg                  # 아이콘 폰트 (SVG)
│   ├── cczicon.ttf                  # 아이콘 폰트 (TTF)
│   ├── cczicon.woff                 # 아이콘 폰트 (WOFF)
│   ├── fonts.css                    # 폰트 스타일시트
│   ├── main.js                      # 메인 자바스크립트
│   ├── plugins.js                   # 플러그인 자바스크립트
│   ├── preloader.svg                # 프리로더 이미지
│   ├── reply_bul.svg                # 댓글 불릿 아이콘
│   ├── reset.css                    # CSS 리셋 파일
│   ├── secret_48.svg                # 비밀글 아이콘
│   ├── icon_alert_danger.svg        # 경고 아이콘 (위험)
│   ├── icon_alert_info.svg          # 정보 아이콘
│   ├── icon_alert_modern.svg        # 모던 알림 아이콘
│   ├── icon_alert_success.svg       # 성공 아이콘
│   └── icon_alert_warning.svg      # 경고 아이콘
│
├── index.xml                        # 스킨 설정 파일 (티스토리 스킨 XML)
├── skin.html                        # 스킨 HTML 템플릿 (1,309줄)
├── style.css                        # 메인 스타일시트 (5,348줄)
└── README.md                        # 이 문서
```

### 파일별 설명

| 파일 | 설명 |
|------|------|
| [`index.xml`](index.xml:1) | 티스토리 스킨 설정 파일. 스킨 정보, 제작자 정보, 기본 설정값 포함 |
| [`skin.html`](skin.html:1) | 스킨의 HTML 템플릿. 레이아웃, 네비게이션, 콘텐츠 영역 정의 |
| [`style.css`](style.css:1) | 메인 스타일시트. 레이아웃, 테마, 반응형 디자인 정의 |
| `images/` | 이미지, 아이콘 폰트, 자바스크립트 파일 포함 |

---

## 📦 설치 방법

### 1. 스킨 다운로드

1. [CCZ-CROSS 공식 페이지](http://webdir.tistory.com/491)에서 스킨 파일을 다운로드합니다.
2. 압축 파일을 해제합니다.

### 2. 티스토리 스킨 업로드

1. 티스토리 관리자 페이지에 로그인합니다.
2. **꾸미기 > 스킨** 메뉴로 이동합니다.
3. **스킨 변경** 버튼을 클릭합니다.
4. **스킨 추가** 버튼을 클릭합니다.
5. 다운로드한 스킨 폴더를 업로드합니다.

### 3. 스킨 적용

1. 업로드한 스킨을 선택합니다.
2. **적용** 버튼을 클릭합니다.
3. 블로그를 새로고침하여 변경사항을 확인합니다.

### 4. 기본 설정

스킨 적용 후 다음 설정을 확인합니다:

- **HTML/CSS 편집**: 필요한 경우 커스텀 CSS 추가
- **사이드바 설정**: 표시할 사이드바 모듈 선택
- **카테고리 설정**: 카테고리 구조 확인
- **프로필 설정**: 블로거 프로필 이미지 및 설명 입력

---

## 🎨 테마 커스터마이징

### 라이트/다크 모드 전환

스킨은 자동 및 수동 테마 전환을 지원합니다.

#### 자동 전환 (시스템 설정)

시스템의 다크 모드 설정을 따릅니다:

```css
@media (prefers-color-scheme: dark) {
    :root:not([data-theme="light"]) {
        /* 다크 모드 스타일 */
    }
}
```

#### 수동 전환

헤더의 테마 전환 버튼을 클릭하여 라이트/다크 모드를 전환할 수 있습니다.

```html
<button type="button" id="theme-toggle" class="theme-toggle" 
        aria-label="테마 전환" title="라이트/다크 테마 전환">
    <i class="icon icon-sun" aria-hidden="true"></i>
    <i class="icon icon-moon" aria-hidden="true"></i>
</button>
```

### CSS Custom Properties 수정

[`style.css`](style.css:1) 파일의 CSS Custom Properties를 수정하여 스킨의 색상 테마를 변경할 수 있습니다.

#### 기본 색상 변경

```css
:root {
    /* 강조색 (Primary Color) */
    --color-primary: #81a9db;  /* 파란색 */
    
    /* 성공 색상 */
    --color-success: #91CCAA; /* 녹색 */
    
    /* 경고 색상 */
    --color-warning: #f0ad4e; /* 주황색 */
    
    /* 위험 색상 */
    --color-danger: #FC9F8A;  /* 빨간색 */
    
    /* 정보 색상 */
    --color-info: #5bc0de;     /* 청록색 */
}
```

#### 다크 모드 색상 변경

```css
[data-theme="dark"] {
    --color-primary: #8fb5e3;  /* 다크 모드용 파란색 */
    --color-success: #a3d4b8;  /* 다크 모드용 녹색 */
    --color-warning: #f5be6a;  /* 다크 모드용 주황색 */
    --color-danger: #ffb3a3;   /* 다크 모드용 빨간색 */
    --color-info: #6fcce8;     /* 다크 모드용 청록색 */
}
```

### 레이아웃 조절

#### 콘텐츠 너비 조절

```css
@media (min-width: 992px) {
    #main-inner {
        margin-right: 320px;  /* 사이드바 너비 */
    }
    
    #sidebar {
        width: 320px;          /* 사이드바 너비 */
    }
}
```

#### 폰트 크기 조절

```css
body {
    font-size: 16px;  /* 기본 폰트 크기 */
}

@media (min-width: 992px) {
    body {
        font-size: 14px;  /* 데스크탑 폰트 크기 */
    }
}
```

### 썸네일 설정

글 목록에서 썸네일을 표시하려면 글 작성시 대표 이미지를 설정해야 합니다.

1. 글 작성 페이지에서 **대표 이미지**를 설정합니다.
2. 썸네일 비율은 기본적으로 4:3 (`ratio-4by3`)입니다.
3. 필요한 경우 [`skin.html`](skin.html:489)에서 썸네일 클래스를 수정할 수 있습니다.

```html
<div class="list-row pos-right ratio-fixed ratio-4by3 crop-center lts-narrow fouc clearfix">
    <s_article_rep_thumbnail>
        <a class="has-object t-photo" href="[##_article_rep_link_##]">
            <div class="thumbnail">
                <div class="cropzone">
                    <img src="[##_article_rep_thumbnail_url_##]">
                </div>
            </div>
        </a>
    </s_article_rep_thumbnail>
    <!-- ... -->
</div>
```

---

## 📄 라이선스

### MIT License

CCZ-CROSS 스킨은 MIT 라이선스 하에 배포됩니다.

```
MIT License

Copyright (c) 2024 흉내쟁이 (COPYCATZ)

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

### 사용 제한 사항

- ✅ **자유로운 사용**: 개인 및 상업적 사용 가능
- ✅ **수정 허용**: 소스 코드 자유로운 수정 가능
- ✅ **배포 허용**: 수정된 버전 배포 가능
- ✅ **저작권 표시**: 원저작자 표시 유지

### 추가 참고 사항

- 썸네일 추출과 관련된 소스는 [ishaiin](http://ishaiin.com/) 님이 판매중인 스킨의 썸네일 추출 소스를 참고하였습니다. 공개 라이센스가 아니기에 이의 재사용을 금합니다.
- 스킨 사용 중 발생하는 문제에 대해서는 제작자가 책임지지 않습니다.

---

## 🤝 기여

이 스킨은 오픈 소스 프로젝트입니다. 버그 리포트, 기능 요청, 코드 기여는 언제든 환영합니다.

1. 이슈 트래커에서 버그를 리포트하거나 기능을 요청하세요.
2. Pull Request를 통해 코드를 기여할 수 있습니다.

---

## 📞 지원

- **제작자 블로그**: [http://copycatz.tistory.com](http://copycatz.tistory.com)
- **업데이트 블로그**: [https://thesauro.tistory.com/](https://thesauro.tistory.com/)
- **이메일**: uzugoer@gmail.com

---

## 📝 변경 이력

### 버전 1.0
- 초기 릴리스
- 반응형 디자인 지원
- 라이트/다크 모드 지원
- 크로스브라우징 지원

---

<div align="center">

**Made with ❤️ by [COPYCATZ](http://copycatz.tistory.com)**

**Updated by [HANBANGA](https://thesauro.tistory.com/)**

</div>
