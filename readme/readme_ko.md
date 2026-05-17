# Pinterest 미디어 분석 도구 (Pinterest Media Analyzer)

> 🔍 Pinterest 공개 콘텐츠의 메타데이터 분석을 지원하는 학습·연구용 프론트엔드 도구

🌐 온라인 체험: [https://twittervideodownloaderx.com/pinterest_downloader_ko](https://twittervideodownloaderx.com/pinterest_downloader_ko)

---

## 📋 프로젝트 소개

본 프로젝트는 웹 기술 학습과 연구 목적으로 개발된 경량 프론트엔드 도구입니다. Pinterest 공개 페이지에서 제공되는 OEmbed 인터페이스 및 구조화 데이터 (Schema.org / Open Graph) 를 활용하여, 동영상·이미지 등 미디어 리소스의 메타정보를 추출하는 것을 지원합니다.

> 🎯 권장 활용 사례:
> - 개인 학습 자료 정리 및 아이디어 수집
> - 프론트엔드 개발 및 데이터 추출 기술 연구
> - 멀티미디어 메타데이터 구조 분석 학습
> - 저작권자로부터 허가받은 콘텐츠의 아카이브 지원

⚠️ **중요 안내**: 본 도구는 '완전히 공개된 정보'만 대상으로 하며, 로그인 인증·유료 콘텐츠·비공개 핀의 분석에는 대응하지 않습니다.

---

## ✨ 주요 기능

- 🔗 **링크 자동 인식**: Pinterest 공개 핀 페이지의 표준 URL / 단축 링크 / 모바일 링크를 자동 판별
- 🎬 **다양한 포맷 지원**: MP4 동영상, WebM 애니메이션, JPG/PNG 정지 이미지 등 리소스 정보 추출
- 📐 **해상도 정보 제공**: 이용 가능한 해상도·파일 형식을 목록으로 표시, 용도에 맞게 선택 가능
- 📱 **반응형 디자인**: PC / 태블릿 / 스마트폰 등 모든 기기에서 원활한 사용 경험 제공
- ⚡ **프론트엔드 우선 아키텍처**: 주요 분석 로직을 브라우저에서 실행하여 서버 부하 감소 및 빠른 응답 구현
- 🔐 **개인정보 보호 설계**: 사용자가 제출한 링크 기록·분석 결과 저장·개인 데이터 수집을 일절 수행하지 않음

---

## 🚀 사용 방법 (퀵 스타트)

1. Pinterest 앱 또는 웹사이트에서 참고하려는 **공개 콘텐츠**를 엽니다
2. 주소창에서 페이지 URL 을 복사합니다 (예: `https://www.pinterest.com/pin/1234567890/`)
3. 본 도구 입력란에 링크를 붙여넣고 '분석' 버튼을 클릭합니다
4. 시스템이 공개 메타데이터를 추출하여 이용 가능한 리소스 정보를 표시합니다
5. 원하는 형식·해상도를 선택한 후, 마우스 우클릭 → '다른 이름으로 저장'으로 로컬에 보관합니다

> 💡 활용 팁:
> - 대상 콘텐츠가 '공개 설정' 상태인지 반드시 확인해 주세요
> - 분석 실패 시 페이지를 새로고침하거나 네트워크 환경을 점검해 주세요
> - 개발 학습 목적이라면 브라우저 개발자 도구 (F12 → Network → Fetch/XHR) 와의 병용을 권장합니다

---

## ⚠️ 준수 사항 및 면책 조항 (필독)

본 프로젝트는 '기술적 중립성'과 '법적 준수'를 기본 원칙으로 운영됩니다. 이용 전 아래 사항을 반드시 숙지해 주세요.

### ✅ 권장되는 이용 방식
- 본인이 접근 권한을 가진 **공개 콘텐츠**만 대상으로 분석합니다
- 추출한 리소스는 **개인 학습·연구·사적 이용** 범위 내에서 활용합니다
- 재배포·2 차 창작·상업적 이용 시에는 반드시 원저작자에게 사전 허가를 획득합니다
- 작품 내 소재 출처·원저작자 명을 명시하여 크리에이터의 권리를 존중합니다

### ❌ 금지되는 행위
- 로그인 필수·유료·비공개 콘텐츠의 분석 시도
- 상업적 스크래핑·데이터 수집 서비스·광고 수익화 목적의 이용
- 단시간 대량 요청·자동화 도구 연동·플랫폼에 대한 부하 공격
- 워터마크·저작권 정보·메타데이터의 변조·삭제

> 📜 법적 근거:
> 본 도구 이용 시에는 대한민국 「저작권법」 「정보통신망 이용촉진 및 정보보호 등에 관한 법률」 및 Pinterest 사의 「Community Guidelines」 「Developer Policy」 를 준수해 주세요.
> 부적절한 이용으로 발생한 법적 책임·손해에 대해 개발자는 어떠한 책임도 지지 않습니다.

---

## 🛠 기술 구현 참고 (개발자 대상)

> 일반 사용자분들은 본 섹션을 건너뛰셔도 됩니다

### 아키텍처 개요
```
사용자 브라우저 → 프론트엔드 분석 모듈 → Pinterest 공개 인터페이스 / OEmbed → 구조화 데이터 추출 → 결과 표시
```

### 주요 기술 포인트
- `fetch` API + 적절한 CORS 프록시 설정을 통한 공개 페이지 메타데이터 획득
- `<script type="application/ld+json">` 내 Schema.org 구조화 데이터 파싱
- Open Graph 태그 (`og:video` / `og:image` / `og:title` 등) 활용 리소스 정보 보완
- 정규식 + DOM 파싱 이중 검증으로 링크 인식 안정성 향상

### 로컬 배포 가이드 (참고용)
```bash
# 1. 저장소 클론 (예시)
git clone https://github.com/yourname/pinterest-downloader-ko.git

# 2. 정적 파일 호스팅 (HTTPS 권장)
#    - Vercel / Netlify / Cloudflare Pages (간편 추천)
#    - Nginx + Let's Encrypt 인증서 (자체 구축)

# 3. 보안 헤더 설정 예시 (Nginx)
add_header Content-Security-Policy "default-src 'self'; script-src 'self' 'unsafe-inline';";
add_header X-Content-Type-Options "nosniff";
add_header Referrer-Policy "strict-origin-when-cross-origin";
```

> 🔐 운영 환경 주의사항:
> - 반드시 HTTPS 를 활성화하여 중간자 공격을 방지해 주세요
> - 과도한 요청을 제한하는 레이트 리미팅 설정을 권장합니다
> - 분석 로직의 과도한 공개는 악용 리스크를 높일 수 있으므로 주의가 필요합니다

---

## 🤝 기여 안내

프로젝트 개선에 함께해 주실 분들을 환영합니다!

| 기여 유형 | 내용 예시 |
|-----------|-----------|
| 🐛 오류 제보 | 분석 오류·화면 깨짐 등 Issue 등록 (URL + 브라우저 정보 + 재현 절차 첨부) |
| 💡 기능 제안 | UX 개선·다국어 지원·접근성 향상 등 건설적인 아이디어 공유 |
| 🌍 번역 협력 | 한국어 외 언어 대응 (중국어 / 영어 / 일본어 등) 번역·교정 지원 |
| 📚 문서 보완 | 사용 예시 추가·기술 원리 도해·준수 가이드 강화 등 |

> 본 프로젝트는 [MIT License](./LICENSE) 에 따라 공개됩니다. 학습·연구 목적의 자유로운 이용·수정을 환영하며, 상업적 커스터마이징 문의는 별도 연락처를 통해 부탁드립니다.

---

## ❓ 자주 묻는 질문 (FAQ)

**Q: "콘텐츠를 가져올 수 없습니다"라는 메시지가 표시되는데 왜 그런가요?**  
A: 가능한 원인: ① 링크 대상이 비공개·삭제된 콘텐츠 ② Pinterest 페이지 구조 일시적 변경 ③ 네트워크 제한·CORS 문제. 대응 방법: 공개 설정 확인 → 다른 네트워크에서 시도 → 시간 간격 두고 재시도.

**Q: 추출한 동영상에 워터마크가 포함되어 있는데 정상인가요?**  
A: 본 도구는 Pinterest 공식이 제공하는 원본 리소스 링크를 그대로 반환하는 방식입니다. 워터마크 유무는 업로드 시점 설정에 의존하며, 본 도구는 어떠한 추가·제거·변경 처리도 수행하지 않습니다.

**Q: 앨범이나 보드 단위 일괄 분석을 지원하나요?**  
A: 현재 버전은 단일 핀 분석에 특화되어 안정성과 규정 준수를 우선하고 있습니다. 일괄 처리 요청에 대해서는 먼저 Pinterest 사의 「Developer Policy」 준수 여부를 스스로 점검해 주시기 바랍니다.

**Q: 이용 이력이나 개인정보를 수집하나요?**  
A: 아닙니다. 본 프로젝트는 순수 정적 프론트엔드 페이지로, 백엔드 로그·분석 스크립트·Cookie 추적 기능을 일절 포함하지 않습니다. 모든 처리는 고객님의 브라우저 내에서 로컬로 완료됩니다.

---

## 🌱 우리의 지향점

> 기술 자체에는 선악이 없습니다. 중요한 것은 사용하는 사람의 '목적'과 '책임감'입니다.

저희는 개발자·이용자 여러분께 다음 가치를 함께 지켜주실 것을 부탁드립니다:

- 🔬 학습과 호기심을 동력으로 웹 기술의 원리를 깊이 이해하기
- 🤲 크리에이터의 권리를 존중하고, 적절한 출처 표기·허가 획득을 생활화하기
- 🌍 디지털 콘텐츠의 건전한 유통과 문화 다양성 유지에 기여하기

올바른 이용을 통해, 창작과 공유의 선순환을 함께 만들어 나갑시다 ✨

---

## 📄 라이선스

본 프로젝트는 [MIT License](./LICENSE) 에 따라 공개됩니다.  
상업적 이용·재배포 시에는 라이선스 조문 준수 및 출처 명시를 부탁드립니다.

```


Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.
```

---

  
*🔖 버전: v1.2.0-kr (프론트엔드 최적화 / 다국어 지원 강화 / 준수 사항 명시 보강)*