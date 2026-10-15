# Awesome Translation Tools

> 여행, 웹 브라우징, 서식 유지 문서 번역, 학술 연구, 오픈소스 로컬 엔진 및 개발자 파이프라인을 아우르는 번역 도구 및 워크플로 큐레이션 디렉터리.

[English](README.md) | [简体中文](README.zh-CN.md) | [日本語](README.ja.md) | [한국어](README.ko.md) | [Deutsch](README.de.md) | [Français](README.fr.md) | [Español](README.es.md) | [Português (Brasil)](README.pt-BR.md) | [Italiano](README.it.md) | [Русский](README.ru.md) | [العربية](README.ar.md) | [हिन्दी](README.hi.md) | [Bahasa Indonesia](README.id.md) | [Türkçe](README.tr.md)

---

번역 작업의 요구 사항은 실제 사용 맥락에 따라 근본적으로 다릅니다. 모바일 기기로 길거리 표지판이나 식당 메뉴를 빠르게 판독해야 하는 상황, 브라우저에서 외국 기술 문서를 대역으로 읽어야 하는 상황, 레이아웃을 깨뜨리지 않고 복잡한 프레젠테이션 슬라이드나 계약서를 변환해야 하는 상황, 학술 논문의 수학 공식을 보존해야 하는 상황, 터미널 파이프라인을 통해 대량의 텍스트를 로컬에서 일괄 번역해야 하는 상황, 자막이 없는 외국어 스트리밍 영상을 시청해야 하는 상황 등 저마다 다른 해결책이 필요합니다.

저희는 **[Equalang](https://equalang.com/?utm_source=github)** 팀입니다. 이 디렉터리는 널리 사용되는 상용 번역 제품과 오픈소스 프로젝트의 공식 문서화된 기능, 접근 경로, 배포 방식 및 사용상 한계와 제약 사항을 작업 중심(Task-oriented)으로 체계적으로 정리하여, 사용자가 자신의 워크플로에 가장 적합한 도구를 찾을 수 있도록 돕습니다.

---

## 목차

- [1. 이동 중 여행 및 구두 대화: 멀티모달 및 음성 입력](#1-on-the-go-travel--spoken-exchange-multi-modal-and-spoken-inputs)
  - [Google Translate](#google-translate)
  - [Apple Translate](#apple-translate)
  - [Microsoft Translator](#microsoft-translator)
  - [Papago](#papago)
  - [iTranslate](#itranslate)
- [2. 맥락 유지 웹 읽기 및 언어 학습: 페이지를 벗어나지 않는 독해](#2-in-context-web-reading--language-learning-reading-without-leaving-the-page)
  - [Immersive Translate](#immersive-translate)
  - [Mate Translate](#mate-translate)
  - [Reverso](#reverso)
  - [Yandex Translate](#yandex-translate)
- [3. 복잡한 문서 레이아웃 및 엔터프라이즈 워크플로: 서식과 자산 보존](#3-complex-document-layouts--enterprise-workflows-preserving-formats-and-assets)
  - [DeepL](#deepl)
  - [O.Translator](#otranslator)
  - [SimplifyAI](#simplifyai)
  - [Lingvanex](#lingvanex)
  - [SYSTRAN](#systran)
  - [AI 만화 번역기](#ai-manga-translator)
- [4. 학술 연구, 작문 교정 및 인간-기계 협업: 번역 품질 향상](#4-academic-writing-refinement--human-in-the-loop-collaboration-polishing-the-output)
  - [Youdao Translate (NetEase Youdao)](#youdao-translate-netease-youdao)
  - [Baidu Translate](#baidu-translate)
  - [TranSmart (Tencent Interactive Translation)](#transmart-tencent-interactive-translation)
  - [LingoCloud (Caiyun Xiaoyi)](#lingocloud-caiyun-xiaoyi)
  - [QuillBot Translate](#quillbot-translate)
- [5. 오픈소스 생태계: 로컬 엔진, API, 데스크톱 클라이언트 및 학술 PDF 파이프라인](#5-open-source-ecosystem-local-engines-apis-desktop-clients--scientific-pdf-pipelines)
  - [5.1 과학 및 학술 PDF 파이프라인](#51-scientific--academic-pdf-pipelines)
    - [PDFMathTranslate (pdf2zh)](#pdfmathtranslate-pdf2zh)
    - [BabelDOC](#babeldoc)
  - [5.2 자체 호스팅 가능한 엔진 및 API](#52-self-hostable-engines--apis)
    - [LibreTranslate](#libretranslate)
    - [Argos Translate](#argos-translate)
  - [5.3 데스크톱 및 터미널 프론트엔드](#53-desktop--terminal-frontends)
    - [Pot (pot-desktop)](#pot-pot-desktop)
    - [Translate Shell](#translate-shell)
- [6. 연결된 엔드투엔드 워크플로:](#6-connected-end-to-end-workflows-equalang) [Equalang](https://equalang.com/?utm_source=github)
  - [1. 서식과 레이아웃을 보존하는 전체 파일 문서 번역](#1-whole-file-document-translation-with-layout-preservation)
  - [2. 브라우저 내 웹 읽기 및 자막 생성](#2-in-browser-reading--subtitle-generation)
  - [3. 별도 설치 없는 현장 음성 소통 및 대화](#3-installation-free-spoken-communication--on-site-exchange)
  - [4. AI 에이전트 및 개발자를 위한 연동 생태계](#4-integration-for-ai-agents-and-developers)
- [7. 작업별 도구 선택 가이드](#7-task-based-decision-guide)
- [8. 디렉터리 수록 원칙 및 검증 기준](#8-directory-principles--verification-criteria)
- [9. 참고 자료](#9-sources)

---

<a id="1-on-the-go-travel--spoken-exchange-multi-modal-and-spoken-inputs"></a>
## 1. 이동 중 여행 및 구두 대화: 멀티모달 및 음성 입력

여행과 현장 업무에서는 빠른 실행 속도, 안정적인 멀티모달 인식, 네트워크 연결이 제한된 환경에서의 오프라인 지원이 핵심입니다.

<a id="google-translate"></a>
### Google Translate
[모바일 Google Translate](https://support.google.com/translate)는 실시간 카메라 OCR, 사진 가져오기, 손글씨 입력, 화면 분할 대면 대화 모드를 지원합니다. 여행자는 네트워크가 원활하지 않은 환경에 대비해 언어 팩을 미리 다운로드하여 오프라인 텍스트 및 오프라인 카메라 번역 기능을 사용할 수 있습니다. 음성 대화 번역은 다양한 화면 레이아웃을 제공하지만, 오프라인 실시간 음성 통역은 특정 Pixel 기기 및 일부 언어 쌍으로 제한됩니다.

데스크톱 브라우저에서 Google Translate는 DOCX, PDF, PPTX, XLSX 파일을 지원하는 전용 [문서 번역 포털](https://support.google.com/translate/answer/2534559?co=GENIE.Platform%3DDesktop&hl=en)을 제공합니다. 이 데스크톱 도구는 디지털 전자 문서용으로 설계되었으며, 순수 이미지로만 구성된 스캔본 PDF 페이지는 OCR 번역 없이 원본 이미지 그대로 다운로드 파일에 유지됩니다.

<p align="center"><img src="assets/google-page@2x.webp" alt="Google Translate 공식 제품 소개 페이지" width="640"><br><sub>Google Translate 공식 제품 소개 페이지 및 모바일 앱 다운로드 영역</sub></p>

<a id="apple-translate"></a>
### Apple Translate
iPhone 및 iPad 사용자라면 시스템 기본 탑재 [Apple 번역 앱](https://support.apple.com/en-gb/guide/iphone/iphd74cb450f/ios)을 별도 설치 없이 바로 사용할 수 있습니다. 텍스트 입력, 음성 입력, 카메라 텍스트 인식, 화면 분할 대면 대화 모드를 지원합니다. 대화 모드는 사용자가 말하는 언어를 자동으로 감지하므로 화자가 바뀔 때마다 마이크 버튼을 수동으로 전환할 필요가 없습니다. 언어 팩을 다운로드해 두면 셀룰러 연결 없이도 기기 내 온디바이스 텍스트 번역이 가능합니다.

Apple 운영체제 생태계 내에서 [실시간 번역 기능](https://support.apple.com/en-us/123720)은 메시지(Messages), 전화(Phone), FaceTime으로도 확장됩니다. 통화 실시간 번역은 Apple Intelligence의 일부로, 호환되는 하드웨어와 시스템 버전이 필요하며 지역별 지원 정책의 적용을 받습니다(예: 중국 본토에서 구매한 기기는 현재 이러한 고급 Apple Intelligence 통화 기능을 지원하지 않습니다).

<p align="center"><img src="assets/apple-page@2x.webp" alt="iPhone 번역 가이드 Apple 공식 지원 페이지" width="640"><br><sub>iPhone에서 단어 및 문구를 번역하는 방법을 안내하는 Apple 공식 지원 페이지</sub></p>

<a id="microsoft-translator"></a>
### Microsoft Translator
[Microsoft Translator 모바일 앱](https://www.microsoft.com/en-us/translator/apps/features/)의 대표적인 특징은 [다자간 다중 기기 대화 기능(multi-device conversation)](https://www.microsoft.com/en-us/translator/help/multi-device-conversation/)입니다. 호스트가 모바일에서 대화 세션을 생성하면, 참여자는 모바일 앱이나 데스크톱 웹 브라우저에서 QR 코드를 스캔하거나 참여 코드를 입력하여 접속할 수 있습니다. 각 참여자는 자신이 선택한 언어로 실시간 전사 및 번역을 확인합니다. 발표자 모드(Presenter mode)는 호스트의 마이크를 계속 열어두고 청중을 음소거할 수 있어 가이드 투어나 강연에 유용합니다.

또한 빈번하게 쓰이는 여행 표현을 위한 다운로드형 회화집과 오프라인 사진 번역 기능도 포함되어 있습니다. 일반 사용자용 앱은 외부 영화, 동영상 파일 또는 미디어 녹음본의 직접 번역을 지원하지 않으며, 다중 기기 음성 대화 세션은 인터넷 연결이 반드시 필요합니다.

<p align="center"><img src="assets/microsoft-page@2x.webp" alt="Microsoft Translator 공식 기능 소개 페이지" width="640"><br><sub>다중 기기 대화 기능을 강조한 Microsoft Translator 공식 기능 페이지</sub></p>

<a id="papago"></a>
### Papago
한국의 네이버(NAVER)가 개발한 [Papago](https://papago.naver.com/)는 한국어, 영어, 일본어, 중국어를 비롯한 동아시아 언어에 실용적인 기능을 제공합니다. 모바일 기기용 [애플리케이션](https://play.google.com/store/apps/details?hl=en-US&id=com.naver.labs.translator)은 대면 대화, 인쇄된 텍스트로 학습 노트를 만드는 에듀(Edu) 모드, 빠른 단어 확인을 위한 Papago 미니 플로팅 창을 제공하여 한국 내 식당 이용, 대중교통 이용, 어학 학습 등에 편리합니다.

웹페이지 번역의 경우 플랫폼에 따라 접근 방식에 차이가 있습니다. 네이버는 PC 웹 포털의 독립형 웹사이트 번역 도구 서비스를 종료하고 PC 사용자에게 Papago가 탑재된 [웨일(Whale) 브라우저](https://whale.naver.com/) 사용을 안내하고 있는 반면, [Papago 모바일 앱](https://help.naver.com/service/16448/contents/15637?lang=ko&osType=MOBILE)의 사이드 메뉴에는 여전히 웹사이트 번역 기능이 유지되고 있습니다. 시스템 요구 사양을 충족하는 호환 기기에서 언어 팩을 다운로드하면([네이버의 오프라인 관련 안내 문서](https://help.naver.com/service/16448/contents/10663?osType=MOBILE) 기준: 4GB 이상의 RAM 필요, 음성 지원은 Android 14 이상 및 전용 음성 패키지 필요), 한국어, 영어, 일본어, 중국어 간체 간 텍스트 및 음성 오프라인 번역이 가능합니다. 단, 오프라인 모드는 사진 OCR, 대화 모드, 웹페이지, 문서 파일 번역은 지원하지 않습니다.

<p align="center"><img src="assets/papago-page@2x.webp" alt="NAVER Papago 공식 웹 번역 인터페이스" width="640"><br><sub>NAVER Papago 웹 번역 작업 공간</sub></p>

<a id="itranslate"></a>
### iTranslate
[iTranslate](https://itranslate.com/)는 내장된 [키보드 확장 프로그램(Keyboard Extension)](https://itranslate.com/features/keyboard-translations/index.html)으로 잘 알려져 있습니다. WhatsApp, iMessage, 이메일 등에서 메시지를 작성할 때 별도의 앱으로 전환할 필요 없이 키보드 인터페이스 내에서 텍스트를 직접 번역할 수 있습니다.

또한 [오프라인 도구](https://itranslate.com/features/offline-translations/index.html)를 통해 자주 쓰는 여행 표현 팩과 기본 회화집을 다운로드할 수 있어, 여행 전 필수 표현을 익히는 데 유용합니다. 지원 기능은 운영체제마다 상이하며, 오프라인 음성 기능은 일부 주요 언어로 제한됩니다.

<p align="center"><img src="assets/itranslate-page@2x.webp" alt="iTranslate 공식 홈페이지" width="640"><br><sub>모바일 애플리케이션 인터페이스 미리보기를 담은 iTranslate 공식 홈페이지</sub></p>

---

<a id="2-in-context-web-reading--language-learning-reading-without-leaving-the-page"></a>
## 2. 맥락 유지 웹 읽기 및 언어 학습: 페이지를 벗어나지 않는 독해

외국어 기사나 문서를 검토할 때 외부 번역 탭을 수시로 오가다 보면 집중 흐름이 끊기기 쉽습니다. 인컨텍스트(In-context) 번역 도구는 사용자가 읽고 있는 브라우저 환경에 번역을 직접 삽입해 줍니다.

<a id="immersive-translate"></a>
### Immersive Translate
[Immersive Translate](https://immersivetranslate.com/)는 웹 원문 단락 바로 아래에 번역문을 삽입하여 깔끔한 이중 언어 대역 레이아웃을 제공하는 브라우저 확장 프로그램입니다. 이중 언어 EPUB 전자책 제작, PDF 뷰어, 브라우저 입력창 텍스트 번역도 지원합니다.

멀티미디어의 경우, Immersive Translate는 YouTube, Netflix 등의 플랫폼에서 기존 자막 트랙을 번역합니다. 또한 [AI 동영상 번역](https://immersivetranslate.com/video/ai-video-translator/) 기능은 음성 인식을 통해 YouTube 등 지원 플랫폼의 무자막 동영상에 대한 이중 언어 자막 생성을 지원하며, 전용 [YouTube 라이브 번역 포털](https://livetranslate.immersivetranslate.com/zh-CN)도 제공합니다. 무자막 음성 기반의 자막 생성은 브라우저 호환성, 오디오 선명도 및 플랫폼의 스트리밍 상태에 영향을 받습니다.

<p align="center"><img src="assets/immersive-page@2x.webp" alt="Immersive Translate 공식 홈페이지" width="640"><br><sub>Immersive Translate 공식 홈페이지 및 브라우저 확장 프로그램 다운로드 포털</sub></p>

<a id="mate-translate"></a>
### Mate Translate
[Mate Translate](https://matetranslate.com/en)는 macOS, iOS 및 주요 데스크톱 브라우저 환경에 최적화되어 있습니다. 웹 서핑 중 단어를 더블 클릭하면 즉시 팝업 사전이 표시되고, 텍스트를 드래그 선택하면 빠른 문맥 번역이 제공되며, 전체 페이지 번역 시 원문과 번역문 뷰를 전환할 수 있고, 상시 접근 가능한 Mac 메뉴바 유틸리티도 제공합니다.

어학 학습자를 위해 Mate는 웹페이지나 Netflix 자막에서 단어를 클릭해 커스텀 단어장(Phrasebook)에 저장할 수 있는 기능을 제공하며, 맞춤형 분류 및 외부 복습을 위한 CSV 내보내기를 지원합니다. Chrome 등 데스크톱 브라우저에서는 내장 PDF 뷰어 내의 텍스트를 드래그 선택하여 즉시 번역을 실행할 수도 있습니다.

<p align="center"><img src="assets/mate-page@2x.webp" alt="Mate Translate 공식 홈페이지" width="640"><br><sub>다양한 플랫폼의 인터페이스 미리보기를 보여주는 Mate Translate 공식 홈페이지</sub></p>

<a id="reverso"></a>
### Reverso
자연스러운 단어 용례를 확인하려는 작문가와 학습자에게 [Reverso Context](https://context.reverso.net/translation/about)는 영화 대사, 국제 간행물, 다국어 웹사이트 등에서 수집한 이중 언어 예문 쌍을 동사 활용표 및 유의어 추천과 함께 제공합니다. 예문이 공개 다국어 말뭉치(코퍼스)에서 추출되므로, 민감하거나 격식 있는 문서 작성 시 문맥 적합성을 직접 확인할 필요가 있습니다.

문서 번역 포털인 [Reverso Documents](https://www.reverso.net/documents/en)는 PDF, Word, PowerPoint, Excel 및 일부 현지화 파일 형식을 지원합니다. 브라우저 내에서 문장 세그먼트별 검토 인터페이스를 제공하므로, 팀이 함께 번역문을 교정한 뒤 완성된 파일을 다운로드할 수 있습니다.

<p align="center"><img src="assets/reverso-page@2x.webp" alt="Reverso 공식 번역 인터페이스" width="640"><br><sub>Reverso 웹 번역 인터페이스 및 내비게이션 바</sub></p>

<a id="yandex-translate"></a>
### Yandex Translate
[Yandex Translate 웹 포털](https://yandex.com/support/translate-desktop/en/) 및 모바일 앱은 텍스트, 이미지, 웹사이트, 문서를 번역합니다. Android 클라이언트에는 지원 언어에 대해 발음 기호, 단어 정의, 유의어, 형태론적 굴절형을 보여주는 상세 사전이 포함되어 있습니다.

모바일의 경우, Android 앱에는 영어-러시아어 [오프라인 사전](https://yandex.ru/support/translate-app-android/en/offline-mobile)이 기본 내장되어 있으며, 추가 언어 팩을 다운로드하여 오프라인 텍스트 입력 번역을 수행할 수 있습니다. 데스크톱 인터페이스는 표준 Office 및 PDF 파일 업로드를 지원합니다. 단, 독립형 서비스인 Yandex Translate와 독자적인 자동 동영상 음성 더빙 기능이 탑재된 Yandex Browser는 서로 구별되는 제품이라는 점에 유의해야 합니다.

<p align="center"><img src="assets/yandex-page@2x.webp" alt="Yandex Translate 공식 웹 인터페이스" width="640"><br><sub>Yandex Translate 입력 인터페이스 및 사이드 내비게이션</sub></p>

---

<a id="3-complex-document-layouts--enterprise-workflows-preserving-formats-and-assets"></a>
## 3. 복잡한 문서 레이아웃 및 엔터프라이즈 워크플로: 서식과 자산 보존

프레젠테이션 슬라이드, 공급업체 계약서, 기술 매뉴얼 등을 다룰 때 레이아웃이 흐트러지면 많은 수작업 수정이 뒤따릅니다. 이 분야의 도구들은 원본 레이아웃 보존, 전문 용어 통제, 번역 자산 재사용에 초점을 맞춥니다.

<a id="deepl"></a>
### DeepL
[DeepL Translator](https://www.deepl.com/en/features)는 텍스트 및 문서 워크플로를 위한 정교한 설정 옵션을 제공합니다. 사용자는 [용어집(Glossary)](https://www.deepl.com/en/features/glossary)을 생성하여 사내 표준 용어나 기술 번역을 일관되게 적용할 수 있으며, 지원되는 언어에서는 격식체(존댓말)와 비격식체 간의 어조를 전환할 수 있습니다.

[문서 번역 서비스](https://www.deepl.com/en/features/document-translation)는 Word, PDF, PPT, Excel, HTML, SRT 파일을 지원합니다(계정 유형에 따라 지원 형식 상이). 제품 생태계에는 텍스트 윤문을 위한 DeepL Write, Teams 및 Zoom에서 실시간 자막을 제공하는 [온라인 미팅용 DeepL Voice](https://support.deepl.com/hc/en-us/articles/16810100955676-About-DeepL-Voice-for-Online-Meetings)(Voice 라이선스 및 호스트 권한 필요), AI 에이전트를 위한 공식 Model Context Protocol(MCP) 가이드가 포함되어 있습니다.

<p align="center"><img src="assets/deepl-page@2x.webp" alt="DeepL 공식 웹 번역 작업 공간" width="640"><br><sub>DeepL 웹 번역기 인터페이스</sub></p>

<a id="otranslator"></a>
### O.Translator
[O.Translator](https://otranslator.com/en/product-info)는 레이아웃 보존 문서 번역에 특화되어 있습니다. PDF, Word, PPT, Excel 외에도 EPUB 전자책, InDesign(IDML), Illustrator(AI), OpenDocument, 자막 파일(SRT/ASS), 만화 아카이브(CBZ/CBR) 등 출판 및 현지화 형식을 지원하며, 스캔본 페이지를 위한 내장 OCR을 갖추고 있습니다. 레이아웃의 완성도는 폰트 임베딩 및 번역 후 텍스트 길어짐에 따라 달라질 수 있습니다.

전체 파일을 번역하기 전에 일부 레이아웃 미리보기를 확인할 수 있습니다. XLSX나 TBX 형식의 용어집 가져오기를 지원하며, [개발자 API](https://www.otranslator.com/en/developer/v1)도 제공합니다. 미디어 옵션은 브라우저 실시간 스트림 번역이 아닌, 업로드된 오디오 및 비디오 파일을 자막 파일로 전사하는 용도로 설계되었습니다.

<p align="center"><img src="assets/otranslator-page@2x.webp" alt="O.Translator 공식 제품 홈페이지" width="640"><br><sub>O.Translator 공식 홈페이지 및 문서 업로드 섹션</sub></p>

<a id="simplifyai"></a>
### SimplifyAI
SimplifyAI는 두 개의 별도 웹사이트를 운영합니다: AI 기반 [복합 문서 워크벤치](https://simplifyai.cn/zh/translate)(simplifyai.cn/zh)와 [일반 문서 번역 포털](https://translate.simplifyai.cn/)(translate.simplifyai.cn)입니다.

워크벤치에서는 Word, PPTX, InDesign, PDF, EPUB 파일에서 번역 전 고빈도 용어를 추출하여 사용자가 미리 검토할 수 있도록 지원합니다. 또한 Word 및 InDesign용 AI 편집(Word 기본 변경 내용 추적 지원), 이중 언어 데이터 내보내기(Excel/XLIFF), 구조화된 Markdown/JSON 추출, 텍스트 넘침 및 폰트 레이아웃 시각적 검사 기능을 제공하여 프리프레스(인쇄 전 공정) 및 디자인 자산 현지화에 적합합니다. 단순한 일상 파일 번역의 경우 일반 번역 포털에서 보다 직관적이고 간결한 과정을 이용할 수 있습니다.

<p align="center"><img src="assets/simplifyai-page@2x.webp" alt="SimplifyAI 공식 홈페이지" width="640"><br><sub>복합 문서 워크벤치 및 기능 모듈을 보여주는 SimplifyAI 공식 홈페이지</sub></p>

<a id="lingvanex"></a>
### Lingvanex
[Lingvanex](https://lingvanex.com/)는 Windows와 macOS 전반에 걸쳐 데스크톱, 모바일, 브라우저 클라이언트를 제공합니다. [Windows 데스크톱 번역기](https://lingvanex.com/products/windows-translator/)는 시스템 전역 단축키(선택한 텍스트에서 Ctrl+C 두 번 누르기 등)를 지원하며, 언어 팩 다운로드 후 오프라인 텍스트 및 로컬 DOCX/ODT 파일 번역을 지원합니다.

일반 소비자용 애플리케이션 외에도, Lingvanex는 엔터프라이즈 오프라인 환경을 위한 다운로드형 데스크톱 소프트웨어인 [보안 번역 소프트웨어(Secure Translation Software)](https://lingvanex.com/products/secure-translation-software/)와 폐쇄망 환경을 위한 온프레미스 기계 번역 솔루션을 별도로 제공합니다.

<p align="center"><img src="assets/lingvanex-page@2x.webp" alt="Lingvanex 공식 홈페이지" width="640"><br><sub>엔터프라이즈 번역 및 온프레미스 솔루션을 소개하는 Lingvanex 공식 홈페이지</sub></p>

<a id="systran"></a>
### SYSTRAN
SYSTRAN은 기업 및 기관의 전문 현지화 요구를 겨냥합니다. 클라우드 서비스인 [SYSTRAN Translate Pro](https://www.systransoft.com/translation-products/translate-pro/)는 Word, PowerPoint, Excel, PDF 파일 번역을 즉시 지원하며, 맞춤형 용어집 및 번역 메모리(TM)와 더불어 법률, 금융, 제조 등 산업별 사전 구성 도메인 모델을 제공합니다.

데이터 주권 요건이 엄격한 조직을 위해 기업 방화벽 내부 온프레미스 배포가 가능한 [Translate Server](https://www.systransoft.com/translation-products/translate-server/), 전용 프라이빗 클라우드 환경, 문서 파이프라인 처리를 위한 일괄 [API](https://www.systransoft.com/translation-products/translate-api/)를 제공합니다.

<p align="center"><img src="assets/systran-page@2x.webp" alt="SYSTRAN Translate Pro 공식 제품 페이지" width="640"><br><sub>SYSTRAN Translate Pro 공식 제품 소개 인터페이스</sub></p>

<a id="ai-manga-translator"></a>
### AI 만화 번역기
[AI 만화 번역기](https://www.mangatranslate.com/ko/ai-manga-translator/)는 Ficory LLC가 제공하는 기업급 온라인 만화 리더로, 만화 이미지의 대사 번역과 후속 편집을 지원합니다. 개인 사용자는 여러 페이지를 일괄 번역하고 번역 설정을 맞춤 조정할 수 있습니다. 스튜디오 사용자는 완전한 온라인 Photoshop 스타일 편집기에서 텍스트 상자, 글꼴과 배치를 편집합니다. 개발자는 [공식 API 예제](https://www.mangatranslate.com/api-examples/)를 참고해 API를 개인 작업 흐름에 연결할 수 있으며, 서비스는 제품이 지원하는 모든 번역 언어를 지원합니다.

이 도구는 온라인 호스팅 서비스입니다. 제한된 무료 이용과 유료 요금제를 제공하며, API 연동에는 계정과 API 키가 필요하고 사용 가능한 크레딧이 적용됩니다. 사용자는 이미지의 문자 인식과 번역 결과를 검토하고 필요한 대사와 배치를 편집해야 합니다.

---

<a id="4-academic-writing-refinement--human-in-the-loop-collaboration-polishing-the-output"></a>
## 4. 학술 연구, 작문 교정 및 인간-기계 협업: 번역 품질 향상

번역은 대개 더 넓은 글쓰기나 연구 워크플로의 시작 단계에 불과합니다. 사전 정의 대조, 표현 윤문, 인터랙티브한 인간-기계 협업 편집은 결과물이 격식 있는 학술적 기준을 충족하도록 돕습니다.

<a id="youdao-translate-netease-youdao"></a>
### Youdao Translate (NetEase Youdao)
넷이즈 유도(NetEase Youdao)의 사전 생태계와 연계된 [유도 번역(Youdao Translate)](https://fanyi.youdao.com/)은 어휘 검색, 번역, 작문 보조 기능을 하나로 연결합니다. 일반적인 텍스트 및 파일 번역 외에도 웹 포털에서 'arXiv 논문 번역' 및 학술 윤문 전용 메뉴를 제공합니다.

연구 발췌문을 번역한 후 문법 검사를 실행하거나 대체 유의어를 검토하고 학술적 어조를 다듬을 수 있어 학생과 연구자가 외국 문헌을 검토하고 논문 초안을 작성하는 데 유용합니다. 논문 윤문 및 미디어 모듈의 지원 형식과 언어 범위는 일반 사전 검색과 다를 수 있습니다.

<p align="center"><img src="assets/youdao-page@2x.webp" alt="NetEase Youdao 번역 공식 웹 작업 공간" width="640"><br><sub>NetEase Youdao 번역 웹 인터페이스 및 기능 내비게이션</sub></p>

<a id="baidu-translate"></a>
### Baidu Translate
[바이두 번역(Baidu Translate)](https://fanyi.baidu.com/)은 중화권 사용자를 위한 폭넓은 클라이언트 지원을 제공합니다. 데스크톱 소프트웨어는 간편한 플로팅 창과 로컬 데스크톱 앱 내 단축키 드래그 번역을 제공하며, 모바일 앱은 사진 번역, 구두 회화 연습, 사전 검색을 통합하고 있습니다.

또한 바이두는 독립된 [바이두 동영상 번역 포털](https://fanyi-video.baidu.com/)을 운영합니다. 사용자가 미디어 파일을 업로드하면 정렬된 이중 언어 자막 트랙을 생성하고, 온라인 편집기에서 이를 검토 및 수정한 뒤 완성된 자막 파일을 내보낼 수 있습니다. 이 기능은 실시간 웹 재생 통역기가 아닌 업로드 기반 후반 작업용 도구입니다.

<p align="center"><img src="assets/baidu-page@2x.webp" alt="바이두 번역 공식 웹사이트 페이지" width="640"><br><sub>바이두 번역 공식 웹 인터페이스</sub></p>

<a id="transmart-tencent-interactive-translation"></a>
### TranSmart (Tencent Interactive Translation)
텐센트 AI 랩(Tencent AI Lab)이 개발한 [TranSmart(텐센트 인터랙티브 번역)](https://transmart.qq.com/zh-CN/intro)는 인간과 기계의 상호작용적 협업을 중심으로 설계되었습니다. 단순히 복사해 쓸 정적 번역문을 출력하는 데 그치지 않고 단어 및 문장 단위의 예측 완성을 실시간으로 제안하며, 확정된 이중 언어 쌍을 활성 번역 메모리에 통합합니다.

번역가는 번역문 내 원하는 위치에 커서를 두고 내용을 수정할 수 있으며, 시스템은 이에 맞춰 이후 문맥의 추천을 동적으로 새로고침합니다. 이를 통해 용어 선택과 문장 호흡을 사용자가 직접 제어할 수 있으며, 텐센트의 일반 소비자용 독립 사전 모바일 앱과는 지향점이 다른 협업 편집기로 작동합니다.

<p align="center"><img src="assets/transmart-page@2x.webp" alt="Tencent TranSmart 공식 웹페이지" width="640"><br><sub>Tencent TranSmart 공식 웹 인터페이스</sub></p>

<a id="lingocloud-caiyun-xiaoyi"></a>
### LingoCloud (Caiyun Xiaoyi)
[LingoCloud](https://www.caiyunapp.com/?lang=zh)는 중국어, 영어, 일본어 워크플로에서 널리 사용됩니다. 브라우저 확장 프로그램은 공개 공유 용어집 및 개인 용어집을 지원하며 웹페이지 내 이중 언어 대역 읽기를 제공합니다. 모바일 앱 안내를 기준으로 한 [문서 번역 서비스](https://docs.caiyunapp.com/lingocloud-app/lingocloud-introduction/app-files-trans.html)는 PDF, Word, PPT, Excel, EPUB, TXT, SRT 등의 형식을 지원하며, 원본 파일에 따라 주로 PDF 또는 Word 형식으로 다운로드 결과물을 제공합니다.

데스크톱 소프트웨어에는 마이크 음성을 캡처하거나 실행 중인 애플리케이션(예: Windows 환경의 Zoom, Teams, Chrome 등)의 시스템 오디오 출력을 가로채 실시간 이중 언어 자막을 표시하는 [LingoCloud 동시통역(Interpretation)](https://www.caiyunapp.com/interpretation/) 기능도 포함되어 있습니다. 데스크톱 동시통역은 운영체제의 오디오 캡처 제한을 받습니다: Windows에서는 지원되는 화상회의 및 미디어 앱 전반에서 시스템 오디오 캡처가 작동하지만, macOS에서는 OS 업데이트로 인해 내부 시스템 오디오 직접 녹음 경로가 현재 지원되지 않아 마이크를 통한 오디오 수음이 실질적인 작동 경로입니다.

<p align="center"><img src="assets/caiyun-page@2x.webp" alt="LingoCloud 공식 웹사이트 페이지" width="640"><br><sub>LingoCloud 공식 웹 인터페이스</sub></p>

<a id="quillbot-translate"></a>
### QuillBot Translate
[QuillBot Translate](https://quillbot.com/translate)는 QuillBot의 작문 및 교정 생태계 안에서 동작합니다. 텍스트 번역 시 인터페이스에서 격식 수준(formality) 옵션을 제공하며, 지원되는 언어에 대해 단어 정의와 유의어를 표시합니다.

번역된 텍스트는 Paraphraser(문장 패러프레이징) 및 Grammar Checker(문법 검사기)로 자연스럽게 복사하여 문장 흐름을 매끄럽게 다듬을 수 있습니다. 또한 단일 PDF 문서를 업로드하여 검토할 수 있는 전용 [PDF 번역 페이지](https://quillbot.com/translate-pdf)도 제공합니다. 번역, 문법 검사, 패러프레이징 도구 간 지원되는 언어 범위에는 차이가 있습니다.

<p align="center"><img src="assets/quillbot-page@2x.webp" alt="QuillBot 공식 Chrome 웹 스토어 확장 프로그램 페이지" width="640"><br><sub>QuillBot 브라우저 확장 프로그램의 공식 Chrome 웹 스토어 제품 페이지</sub></p>

---

<a id="5-open-source-ecosystem-local-engines-apis-desktop-clients--scientific-pdf-pipelines"></a>
## 5. 오픈소스 생태계: 로컬 엔진, API, 데스크톱 클라이언트 및 학술 PDF 파이프라인

개발자, 개인정보 보호를 중시하는 팀, 학술 연구자는 코드를 직접 검증할 수 있거나 로컬에서 오프라인으로 실행할 수 있는 환경, 또는 맞춤형 자동화 파이프라인을 필요로 하는 경우가 많습니다. 오픈소스 번역 생태계는 다음과 같은 뚜렷한 아키텍처 계층으로 나뉩니다:

- **과학 및 학술 PDF 레이아웃 도구**: 다단 레이아웃, 수식, 도표를 보존하면서 복잡한 학술 논문을 번역합니다.
- **자체 호스팅 가능한 번역 서비스**: 로컬 네트워크 배포를 위한 HTTP REST API 엔드포인트와 웹 UI를 제공합니다.
- **임베디드 오프라인 번역 엔진**: 외부 네트워크 의존성 없이 Python 라이브러리를 통해 로컬에서 신경망 기계 번역을 실행합니다.
- **데스크톱 및 터미널 프론트엔드**: 다중 엔진 조회, 클립보드 감시, OCR, 셸 파이프라인을 통합합니다.

> [!IMPORTANT]
> 오픈소스 코드를 로컬에서 실행한다고 해서 번역이 자동으로 오프라인으로 처리되거나 비공개로 유지되는 것은 아닙니다. 도구 자체는 로컬에서 실행되더라도 기본 설정상 클라우드 API를 호출할 수 있습니다. 진정한 오프라인 번역이 이루어지려면 로컬 모델 자산과 로컬 번역 엔진이 모두 갖추어져야 합니다.

<a id="51-scientific--academic-pdf-pipelines"></a>
### 5.1 과학 및 학술 PDF 파이프라인

<a id="pdfmathtranslate-pdf2zh"></a>
#### PDFMathTranslate (pdf2zh)
[PDFMathTranslate](https://github.com/PDFMathTranslate/PDFMathTranslate)(GNU AGPL v3)는 과학 및 학술 PDF 문서에 특화된 오픈소스 도구입니다. 다단 논문 구조, 수학 표기법, 삽입된 그래픽, 목차 및 주석을 보존합니다.

- **단일 및 대역 출력**: 번역문만 포함된 문서(`-mono.pdf`)와 원문-번역문 대역 비교 문서(`-dual.pdf`)를 모두 생성합니다.
- **인터페이스 및 연동**: 명령줄 도구(CLI), 대화형 WebUI, Docker 컨테이너 배포, Model Context Protocol(MCP)을 지원합니다. 연계 프로젝트로 Zotero 연동 플러그인도 제공됩니다.
- **번역 백엔드**: Google Translate(문서화된 기본값), DeepL, OpenAI 호환 API, 로컬 Ollama 인스턴스를 지원하는 플러그형 아키텍처를 채택하고 있습니다. 클라우드 백엔드가 설정되어 있다면 Docker나 WebUI를 통해 로컬 배포하더라도 오프라인으로 작동하는 것은 아닙니다.
- **OCR 지원**: 흰색 배경의 검은색 텍스트 스캔본 페이지를 위한 실험적 OCR을 포함합니다(최초 사용 시 언어 모델 자산을 다운로드하며, 이후 로컬에서 재사용 가능).

<p align="center"><img src="assets/pdfmathtranslate-page.webp" alt="PDFMathTranslate 공식 GitHub 저장소 페이지" width="640"><br><sub>학술 PDF 레이아웃 번역과 CLI/WebUI 워크플로를 보여주는 공식 PDFMathTranslate 저장소 개요</sub></p>

<a id="babeldoc"></a>
#### BabelDOC
[BabelDOC](https://github.com/funstory-ai/BabelDOC)(GNU AGPL v3)는 문서 수준의 과학 논문 번역 및 이중 언어 대역 비교 라이브러리로, 디버깅용 CLI와 함께 주로 Python 애플리케이션에 임베드하여 사용하도록 설계되었습니다.

- **레이아웃 및 출력 제어**: 단일(mono) 또는 대역(dual) 출력, 동일 페이지 좌우 대역 또는 원문/번역문 페이지 교차 배치, 특정 페이지 선택 번역, 대용량 PDF 분할 및 병합, 사용자 정의 CSV 용어집 입력, 수식 보존을 지원합니다. 표 텍스트 번역은 공식 문서에 실험적 기능으로 명시되어 있습니다.
- **백엔드 아키텍처**: OpenAI 호환 엔드포인트 또는 로컬 Ollama 인스턴스를 통한 번역 백엔드 설정이 필요합니다. PDF 처리 및 레이아웃 엔진 역할을 하므로, 자체적인 범용 번역 엔진을 내장하고 있지는 않습니다.
- **오프라인 자산 및 사용 한계**: 문서 레이아웃 모델과 폰트를 위한 웜업 루틴 및 오프라인 자산 생성/복원 기능을 제공합니다. 완전한 오프라인 실행을 위해서는 사전 캐시된 자산과 로컬에서 실행 중인 번역 백엔드(로컬 Ollama 등)가 모두 필요합니다. 공식 문서에서는 주로 영어-중국어 워크플로에서 검증되었음을 강조하며, 흰색 배경의 검은색 텍스트를 위한 실험적 OCR 우회 기능을 제공합니다.

<p align="center"><img src="assets/babeldoc-page.webp" alt="BabelDOC 공식 GitHub 저장소 페이지" width="640"><br><sub>문서 수준의 과학 PDF 번역 라이브러리 역량을 보여주는 공식 BabelDOC 저장소 개요</sub></p>

<a id="52-self-hostable-engines--apis"></a>
### 5.2 자체 호스팅 가능한 엔진 및 API

<a id="libretranslate"></a>
#### LibreTranslate
[LibreTranslate](https://github.com/LibreTranslate/LibreTranslate)(GNU AGPL v3)는 Argos Translate 엔진을 기반으로 구축된, 웹 UI가 포함된 무료 오픈소스 자체 호스팅 기계 번역 API 서비스입니다.

- **API 및 웹 서비스**: 텍스트 번역, 출발어 감지, HTML/마크업 처리를 위한 REST API 엔드포인트를 제공합니다. 상용 번역 API의 프록시가 아닌 독립적인 서비스 계층으로 작동합니다.
- **로컬 배포 및 프라이버시**: 의존성 패키지와 언어 모델을 설치하고 나면 외부 서드파티로 데이터를 전송하지 않고 로컬 하드웨어에서 완전히 실행할 수 있습니다. 공개 호스팅 인스턴스를 사용하는 경우에는 여전히 네트워크 연결이 필요합니다. 호스트 요구 사항에 따라 API 키 접근 제어를 활성화하거나 비활성화할 수 있습니다.
- **지원 언어 및 파일 형식**: 지원 가능한 언어 쌍은 설치된 언어 모델에 따라 달라집니다. argos-translate-files와 같은 연계 프로젝트를 통해 TXT, ODT, ODP, DOCX, PPTX, EPUB, HTML, SRT, PDF 등의 파일 번역을 지원합니다.

<p align="center"><img src="assets/libretranslate-page.webp" alt="LibreTranslate 공식 GitHub 저장소 페이지" width="640"><br><sub>자체 호스팅 번역 API 및 웹 인터페이스 기능을 보여주는 공식 LibreTranslate 저장소 개요</sub></p>

<a id="argos-translate"></a>
#### Argos Translate
[Argos Translate](https://github.com/argosopentech/argos-translate)(README에 MIT License / CC0 옵션 명시)는 오픈소스 오프라인 Python 번역 라이브러리 및 명령줄 도구이며, 별도로 설치 가능한 GUI 클라이언트도 제공합니다.

- **모듈식 모델 패키지**: `.argosmodel` 확장자를 사용하는 언어 모델 패키지를 다운로드하고 관리합니다. 직접 번역 가능한 언어 쌍이 없는 경우, 설치된 중간 언어 쌍을 거쳐 피벗(pivot) 번역을 수행할 수 있습니다(예: 영어를 거쳐 번역).
- **생태계 엔진**: LibreTranslate의 기반 기계 번역 엔진으로 작동합니다. 연계 프로젝트를 통해 HTML 번역(`translate-html`) 및 파일 처리(`argos-translate-files`)로 기능을 확장할 수 있습니다.
- **오프라인 작동**: 모델 설치가 완료되면 완전히 오프라인으로 실행됩니다. 단, 패키지 색인 및 초기 모델을 다운로드할 때는 인터넷 연결이 필요합니다.

<p align="center"><img src="assets/argos-translate-page.webp" alt="Argos Translate 공식 GitHub 저장소 페이지" width="640"><br><sub>모듈식 오프라인 번역 엔진 및 패키지 시스템을 설명하는 공식 Argos Translate 저장소 개요</sub></p>

<a id="53-desktop--terminal-frontends"></a>
### 5.3 데스크톱 및 터미널 프론트엔드

<a id="pot-pot-desktop"></a>
#### Pot (pot-desktop)
[Pot](https://github.com/pot-app/pot-desktop)(GNU GPL v3)는 Windows, macOS, Linux를 지원하는 크로스 플랫폼 데스크톱 번역 도구로, 단축키 드래그 번역, 텍스트 입력 번역, 클립보드 감시, 스크린샷 OCR, 스크린샷 번역을 지원합니다(공식 GitHub 저장소는 2026-09-07부로 읽기 전용으로 아카이브되었습니다).

- **다중 서비스 집합**: 여러 번역 및 사전 서비스에 동시에 질의하여 결과를 나란히 비교할 수 있습니다. 음성 합성(TTS), Anki 및 Eudic으로의 단어 내보내기, 플러그인 확장을 지원합니다.
- **플러그형 백엔드 및 OCR**: 클라우드 번역 제공업체, OpenAI 호환 API, 로컬 Ollama 엔드포인트를 집합하여 사용할 수 있습니다. OCR의 경우 플랫폼 네이티브 옵션(Windows 시스템 OCR, Apple Vision, Linux Tesseract), Tesseract.js 또는 로컬 플러그인을 선택할 수 있습니다.
- **오프라인 실행 경로**: 드래그 선택 및 입력 텍스트 번역은 로컬 번역 백엔드(로컬 Ollama 인스턴스 등)만 구성되어 있으면 실행 가능하며, 스크린샷 번역은 오프라인 OCR 엔진(플랫폼 네이티브 OCR 또는 Tesseract 등)이 추가로 필요합니다. 클라우드 서비스를 사용할 경우 요청은 네트워크를 통해 전송됩니다.

<p align="center"><img src="assets/pot-desktop-page.webp" alt="Pot 데스크톱 번역 공식 GitHub 저장소 페이지" width="640"><br><sub>다중 인터페이스 번역, OCR, 클립보드 워크플로를 보여주는 공식 Pot 데스크톱 클라이언트 저장소 개요</sub></p>

<a id="translate-shell"></a>
#### Translate Shell
[Translate Shell](https://github.com/soimort/translate-shell)(The Unlicense / 퍼블릭 도메인)은 Unix 계열 터미널 환경을 위한 다기능 명령줄 번역 도구(실행 파일명 `trans`)입니다.

- **CLI 검색 및 사전**: 셸에서 직접 단어 정의, 문구 번역, 간결한 사전 모드, 대화형 REPL 세션, 언어 식별을 지원합니다.
- **Unix 파이프라인**: 표준 입출력(`stdin` / `stdout`)과 원활하게 연동되며, 텍스트 파일을 직접 처리하고, 외부 오디오 플레이어가 설치되어 있으면 음성 합성(TTS)도 지원합니다.
- **엔진 계층**: 공개 번역 서비스(기본값 Google Translate, Bing Translator, Yandex.Translate, Apertium)에 연결하는 경량 클라이언트 프론트엔드로 작동합니다.
- **사용 한계**: 로컬 신경망 번역 모델을 자체 내장하지 않으므로, 일반적인 작동을 위해서는 선택한 엔진 서비스로의 외부 네트워크 연결이 필요합니다. 파일 번역은 서식 있는 문서가 아닌 순수 텍스트 스트림용으로 설계되었습니다.

<p align="center"><img src="assets/translate-shell-page.webp" alt="Translate Shell 공식 GitHub 저장소 페이지" width="640"><br><sub>터미널 명령줄 번역 및 파이프라인 연동을 보여주는 공식 Translate Shell 저장소 개요</sub></p>

---

<a id="6-connected-end-to-end-workflows-equalang"></a>
## 6. 연결된 엔드투엔드 워크플로: [Equalang](https://equalang.com/?utm_source=github)

이상의 도구들을 살펴보면 각 서비스가 특정 작업에 맞춰 명확한 강점을 발전시켜 왔음을 알 수 있습니다. 하지만 실제 일상 업무에서는 이러한 요구 사항들이 서로 교차하는 경우가 빈번합니다:

브라우저에서 온라인 백서를 읽다가 표와 도표가 포함된 첨부 PDF를 다운로드하고, 자막이 없는 강의 영상을 시청한 뒤, 해외 협력 파트너와 직접 소통하며 Word로 요약 보고서를 작성해야 할 수 있습니다. 이때 파편화된 개별 소프트웨어와 파일 변환기를 오가다 보면 작업 흐름이 끊기게 됩니다.

저희는 이러한 작업들을 매끄럽고 연속적인 대역(side-by-side) 번역 워크플로로 연결하여 문서, 웹페이지, 동영상, 현장 실시간 소통 전반에서 조율된 번역 지원을 제공하고자 **[Equalang](https://equalang.com/?utm_source=github)**을 설계했습니다.

<p align="center"><img src="assets/equalang-en-page@2x.webp" alt="Equalang 공식 영문 홈페이지" width="640"><br><sub><a href="https://equalang.com/?utm_source=github">Equalang</a> 공식 영문 웹사이트 홈페이지</sub></p>

<a id="1-whole-file-document-translation-with-layout-preservation"></a>
### 1. 서식과 레이아웃을 보존하는 전체 파일 문서 번역
[Equalang](https://equalang.com/?utm_source=github)은 전체 문서를 번역할 때 구조 보존과 번역 후 활용성에 초점을 맞추며, 연구 문헌, 프레젠테이션, 일상 사무 문서 전반에 맞춤형 워크플로를 제공합니다:

- **PDF 문서 및 독해**: 다단 레이아웃, 머리글, 바닥글, 캡션을 보존하고, 페이지 경계에서 나뉜 문장을 다시 온전하게 연결한 후 번역하며, 표 구조, 인라인 수식, 문서 내부 링크를 그대로 유지합니다. [학술 PDF 읽기 가이드](https://equalang.com/blog/translate-and-read-pdf-documents?utm_source=github)에서 설명하듯, 독자는 원문과 번역본을 나란히 배치한 대역 레이아웃으로 확인하면서 모국어로 핵심 논지를 먼저 파악한 뒤 원본 페이지의 구체적인 용어와 데이터를 교차 검증할 수 있습니다.

- **PowerPoint 프레젠테이션**: [슬라이드 서식 가이드](https://equalang.com/blog/translate-powerpoint-keep-formatting?utm_source=github)에 나와 있듯이, 번역된 PPTX 파일은 표를 정적 이미지로 병합하지 않고 기본 편집 가능한 표 형식 그대로 유지합니다. 한 문장 안의 굵게, 기울임꼴, 글꼴 색상 등 단어 단위 스타일링이 번역된 해당 어구에 정확히 매핑됩니다. 슬라이드 전반에 걸쳐 핵심 용어와 제목의 일관성이 유지되며, 번역문이 길어질 경우 텍스트 상자 내 글꼴 크기가 자동으로 축소되어 텍스트 넘침이나 그래픽 가림을 방지합니다.

- **Word 및 Excel 오피스 파일**: 검증된 [Word 번역 테스트](https://equalang.com/blog/translate-word-document-keep-formatting?utm_source=github)에서 번역된 DOCX 파일은 제목 계층, 글머리 기호 목록, 가격표, 굵은 글씨 서식을 그대로 유지하여 Microsoft Word에서 직접 추가 편집이 가능했습니다. [Excel 단가표 검증](https://equalang.com/blog/translate-excel-file?utm_source=github)에서는 수식과 숫자가 온전히 보존되었으며, 셀 간 중복되는 텍스트 문자열은 단 한 번만 번역 처리되었습니다.

- **전자책 및 포맷 미디어**: EPUB 전자책은 목차 내비게이션과 내부 앵커 링크를 유지합니다. 최대 180분 분량의 녹음 오디오 및 비디오 파일의 경우, 일반 웹 문서 업로드 포털이 아닌 개발자 API 및 Agent Skill/MCP 연동을 통해 번역 및 전사 작업을 제출할 수 있으며, 타임스탬프가 포함된 이중 언어 SRT/VTT 자막 파일이나 원문 전사본을 출력합니다.

<a id="2-in-browser-reading--subtitle-generation"></a>
### 2. 브라우저 내 웹 읽기 및 자막 생성
가벼운 [브라우저 확장 프로그램](https://equalang.com/extension?utm_source=github)(Chrome, Edge, Firefox용 설치 가이드 제공, Safari 18.4+용 임시 Mac Safari 모드 지원)을 통해 일상적인 독해 과정에 번역이 자연스럽게 녹아듭니다:

- **단락 아래 이중 언어 웹 읽기**: 페이지를 스크롤하면 원문 텍스트 바로 아래에 번역 단락이 나란히 표시됩니다. 필요할 때 단어를 찾아볼 수 있도록 설정에서 플로팅 아이콘을 켜고 끌 수 있습니다. 로컬 PDF 파일을 볼 때는 확장 프로그램 관리 페이지에서 '파일 URL에 대한 액세스 허용'을 활성화하여 단어를 선택하고 조회할 수 있습니다.

- **이중 언어 동영상 자막**: [이중 언어 동영상 시청 가이드](https://equalang.com/blog/watch-videos-with-bilingual-subtitles?utm_source=github)에서 소개했듯 YouTube, Netflix, TikTok, Bilibili를 지원합니다. 기존 자막 번역은 물론, 확장 프로그램이 오디오 스트림을 캡처하여 **자막이 없는 영상**에 대해서도 실시간 이중 언어 자막을 생성할 수 있으며(브라우저 환경 및 미디어 암호화 제한의 영향을 받으며, YouTube 라이브 스트림 및 공식 예고편에서 검증 완료), YouTube 실시간 라이브 채팅 댓글도 동시에 번역합니다.

<a id="3-installation-free-spoken-communication--on-site-exchange"></a>
### 3. 별도 설치 없는 현장 음성 소통 및 대화
대화 상대방에게 전용 모바일 앱 설치를 요구하는 것은 특히 여행이나 현장 상황에서 큰 부담이 됩니다. 인터넷에 연결되어 있다면 [Equalang](https://equalang.com/?utm_source=github)은 표준 브라우저 내에서 직접 사진 번역과 음성 통역을 제공합니다(최초 1회 로그인 및 최초 사용 시 기기 카메라/마이크 권한 허용 필요). 자세한 내용은 [해외 파트너 소통 가이드](https://equalang.com/blog/talk-with-overseas-partners?utm_source=github)에서 다루고 있습니다:

- **모바일 사진 번역**: 여행 중 낯선 식당 메뉴판, 길거리 표지판, 안내문을 마주했을 때 모바일 브라우저에서 바로 사진을 촬영할 수 있습니다. 사진의 원래 레이아웃 위에 번역문이 직접 덧씌워지므로, [여행 사진 번역 가이드](https://equalang.com/blog/photo-translation-for-travel?utm_source=github)에 나온 것처럼 원본 이미지를 대조하며 음료를 주문하거나 공지사항을 확인하기 쉽습니다.

- **대면 대화 모드**: 호텔 짐 보관, 길 묻기, 안내 데스크 응대 등 직접 마주 보는 상황을 위해 설계되었습니다. 두 사람이 스마트폰이나 태블릿 한 대를 가운데에 평평하게 두고 상하 반전 분할 화면이나 좌우 대역 뷰를 통해 연속 양방향 전사와 대화 기록 내보내기를 이용할 수 있습니다([여행 대면 대화 가이드](https://equalang.com/blog/talk-face-to-face-while-traveling?utm_source=github) 참조).

- **현장 실시간 듣기(Live Listening)**: 현장 발표나 강연 중 웹 포털을 열면 기기의 물리적 마이크를 통해 수음된 음성을 실시간 이중 언어 자막으로 확인할 수 있으며, 청취 중 선택 가능한 텍스트 음성 변환(TTS) 오디오 재생과 종료 후 전사 기록 내보내기를 지원합니다(브라우저 확장 프로그램의 스트리밍 미디어 오디오 캡처와는 구분됩니다).

- **통역 통화(Translated Calls)**: 호스트가 웹 포털에 로그인하여 보안 통화 링크를 생성한 뒤 메시지 앱으로 공유합니다. **상대방은 계정을 생성하거나 소프트웨어를 설치할 필요 없이 브라우저로 직접 접속**하며, 표시할 이름을 입력하고 호스트가 수락하면 바로 통화가 시작됩니다. 양측 모두 모국어로 말하고 번역된 음성을 들으며 실시간 텍스트를 함께 확인할 수 있습니다.

<a id="4-integration-for-ai-agents-and-developers"></a>
### 4. AI 에이전트 및 개발자를 위한 연동 생태계
개발자와 팀이 번역을 자동화된 워크플로에 손쉽게 통합할 수 있도록 지원합니다:

- **개발자 API**: 텍스트를 위한 즉시 응답 엔드포인트와 함께 Idempotency-Key 재시도 및 콜백 알림을 지원하는 비동기 파일 작업 처리를 제공합니다([파일 번역 API 연동 가이드](https://equalang.com/blog/integrate-file-translation-api?utm_source=github) 참조).

- **Skill 및 MCP 연동**: [equalang-skill](https://github.com/equalang/equalang-skill)을 통한 오픈소스 Agent Skill과 [@equalang/mcp](https://github.com/equalang/equalang-mcp)를 통한 공식 Model Context Protocol 지원을 유지 관리합니다. Claude Code, Codex, WorkBuddy 등의 환경에서 간단한 설치 프롬프트를 실행하고 API 키를 설정하면, [AI 어시스턴트 파일 번역 가이드](https://equalang.com/blog/translate-files-with-ai-assistants?utm_source=github)에 따라 사용자의 AI 어시스턴트가 문서 번역과 미디어 전사 작업을 워크플로 내에서 직접 수행할 수 있습니다.

---

<a id="7-task-based-decision-guide"></a>
## 7. 작업별 도구 선택 가이드

현재 작업에 가장 적합한 도구를 선택하려면 다음 작업 대조표를 참고하세요:

| 주요 작업 | 핵심 요구 사항 | 추천 도구 | 주요 고려 사항 |
| :--- | :--- | :--- | :--- |
| **여행 및 구두 대화** | 사진 OCR, 양방향 대화, 오프라인 팩 및 온라인 여행 도구 | Google Translate, Apple Translate, Papago, [Equalang](https://equalang.com/?utm_source=github) | 신호가 약한 지역에 대비해 Google, Apple 또는 Papago(하드웨어 요구 사양 확인 필요)에서 오프라인 언어 팩을 다운로드하세요. 인터넷이 연결된 환경이라면 [Equalang](https://equalang.com/?utm_source=github)을 통해 앱 설치 없이 브라우저 기반 사진 번역과 대면 대화를 이용할 수 있습니다. |
| **다중 기기 워크숍** | 일대다 발표, 여러 기기 동시 참여 | Microsoft Translator | 호스트는 모바일 앱에서 발표자 모드(Presenter mode)를 실행하고, 참석자는 소프트웨어 설치 없이 표준 브라우저를 통해 접속합니다. |
| **심층 웹 읽기** | 페이지를 벗어나지 않는 단락 아래 대역 읽기 | Immersive Translate, [Equalang](https://equalang.com/?utm_source=github), Mate Translate | 이중 언어 단락 대역에는 Immersive Translate 또는 [Equalang](https://equalang.com/?utm_source=github)을 사용하세요. 전체 페이지 뷰 전환이나 Mac 환경의 단어장 저장이 필요하다면 Mate Translate를 활용하세요. |
| **무자막 영상 및 라이브 스트림** | 실시간 자막 생성, 스트리밍 호환성 | [Equalang](https://equalang.com/?utm_source=github), Immersive Translate | 두 도구 모두 지원되는 플랫폼(YouTube 등)에서 원본 오디오로부터 자막을 생성할 수 있습니다. 라이브 채팅 처리 및 스트림 대응 방식을 비교해 보세요. |
| **학술 논문 및 과학 PDF** | 수식 보존, 다단 구조, 페이지 경계 텍스트 연결 | PDFMathTranslate, BabelDOC, [Equalang](https://equalang.com/?utm_source=github) | PDFMathTranslate와 BabelDOC은 이중 언어 대역 PDF 출력과 로컬/클라우드 LLM 백엔드를 지원하는 오픈소스 파이프라인을 제공합니다. [Equalang](https://equalang.com/?utm_source=github)은 브라우저 기반 대역 읽기 및 레이아웃 보존을 지원합니다. |
| **출판 프리프레스 및 디자인 형식** | InDesign, Illustrator, 만화 아카이브, 프리프레스 QA | SimplifyAI, O.Translator | InDesign(IDML) 및 디자인 자산 프리프레스에는 SimplifyAI와 O.Translator를 사용하세요. SimplifyAI는 기본 Word 변경 내용 추적을 지원하는 AI 편집을 포함합니다. |
| **프레젠테이션 및 오피스 문서** | 네이티브 표, 스타일, 수식 및 편집 가능성 보존 | [Equalang](https://equalang.com/?utm_source=github), DeepL | [Equalang](https://equalang.com/?utm_source=github)은 적응형 폰트 크기 조절을 통해 PPTX의 네이티브 표/스타일을 보존하고 Excel 수식을 유지합니다. 용어집을 활용한 기업용 Word/Office 파일 번역에는 DeepL을 추천합니다. |
| **학술 작문 및 윤문** | 문법적 정확성, 격식 있는 학술적 문체 | Youdao Translate, QuillBot Translate, TranSmart | Youdao와 QuillBot은 번역과 텍스트 윤문을 매끄럽게 연결합니다. TranSmart는 대화형 인간-기계 협업 편집을 제공합니다. |
| **데스크톱 단축키 검색 및 다중 엔진** | 전역 단축키, OCR, 여러 엔진 동시 비교 | Pot, Mate Translate | Pot은 Windows, Mac, Linux에서 다중 엔진 동시 질의와 스크린샷 OCR을 지원합니다. Mate는 네이티브 Mac 메뉴바 유틸리티를 제공합니다. |
| **터미널 스크립트 및 셸 파이프라인** | CLI 검색, stdin/stdout 파이프라인, 일반 텍스트 스크립트 | Translate Shell, Argos Translate | Translate Shell은 원격 엔진을 통한 경량 CLI 번역을 제공합니다. Argos Translate는 로컬 모델을 사용하는 오프라인 Python CLI를 제공합니다. |
| **자체 호스팅 프라이빗 API 및 오프라인 엔진** | 폐쇄망 환경, 제3자 데이터 전송 차단 | LibreTranslate, Argos Translate, SYSTRAN, Lingvanex | LibreTranslate는 자체 호스팅 HTTP API 서비스와 WebUI를 제공합니다. Argos Translate는 모듈식 모델 패키지를 갖춘 오프라인 Python 라이브러리/CLI 엔진으로 이를 구동합니다. SYSTRAN과 Lingvanex는 기업용 온프레미스 배포를 지원합니다. |
| **연결된 엔드투엔드 워크플로** | 문서, 스트리밍 자막, 웹 통화 및 AI 에이전트 연동 | [Equalang](https://equalang.com/?utm_source=github) | 통합 문서 처리, 무자막 미디어 자막 생성, 앱 설치 없는 브라우저 통화, Claude Code 또는 WorkBuddy와의 직접 연동을 지원합니다. |

---

<a id="8-directory-principles--verification-criteria"></a>
## 8. 디렉터리 수록 원칙 및 검증 기준

이 디렉터리의 실용성과 사실적 정확성을 유지하기 위해 모든 항목은 엄격한 수록 및 검토 기준을 따릅니다:

1. **마케팅 주장보다 공식 문서화된 기능 우선**: 모든 설명은 공식 문서, 사용자 매뉴얼, 검증된 저장소 소스 파일에 근거합니다. 완벽한 레이아웃 보존이나 모든 형식의 완벽한 지원과 같은 과장된 주장은 배제합니다.
2. **명확한 아키텍처 경계 구분**: 번역 프론트엔드, 자체 호스팅 가능한 서비스 계층, 오프라인 번역 엔진, 문서 레이아웃 라이브러리를 명확히 구분합니다. 로컬에서 실행되는 오픈소스 코드와 진정한 오프라인 실행은 엄격하게 구분하여 기술합니다.
3. **작업 중심의 수록 범위**: 워크플로별 실제 적합성을 기준으로 도구를 분류합니다. 주관적인 등급표(티어 리스트), 품질 순위, 일시적인 가격 정보는 수록하지 않습니다.
4. **투명한 관리 주체 명시**: 이 카탈로그는 **[Equalang](https://equalang.com/?utm_source=github)** 팀이 선별하고 관리합니다. [Equalang](https://equalang.com/?utm_source=github) 또한 검증 가능한 기능적 한계와 투명한 시스템 요구 사양과 함께 다른 도구들과 나란히 동등하게 소개됩니다.

**키워드**: 번역 도구, 문서 번역, 웹 이중 언어 읽기, 학술 PDF 번역, 오픈소스 번역, 기계 번역 API, 레이아웃 보존, AI 에이전트.

---

<a id="9-sources"></a>
## 9. 참고 자료

1. [Google Translate 고객센터](https://support.google.com/translate)
2. [Google Translate 데스크톱 문서 번역](https://support.google.com/translate/answer/2534559?co=GENIE.Platform%3DDesktop&hl=en)
3. [Apple 고객지원: iPhone 번역 앱 가이드](https://support.apple.com/en-gb/guide/iphone/iphd74cb450f/ios)
4. [Apple 고객지원: 실시간 번역 및 기능 지원 현황](https://support.apple.com/en-us/123720)
5. [Microsoft Translator 모바일 기능 안내](https://www.microsoft.com/en-us/translator/apps/features/)
6. [Microsoft Translator 다중 기기 대화 도움말](https://www.microsoft.com/en-us/translator/help/multi-device-conversation/)
7. [NAVER Papago 공식 포털](https://papago.naver.com/)
8. [iTranslate 키보드 및 오프라인 기능](https://itranslate.com/features/keyboard-translations/index.html)
9. [Reverso Context 사용 정보](https://context.reverso.net/translation/about)
10. [Reverso Documents 포털](https://www.reverso.net/documents/en)
11. [Yandex Translate 데스크톱 및 모바일 도움말](https://yandex.com/support/translate-desktop/en/)
12. [Immersive Translate 공식 문서](https://immersivetranslate.com/)
13. [O.Translator 제품 정보 및 지원 형식](https://otranslator.com/en/product-info)
14. [SimplifyAI 복합 문서 워크벤치](https://simplifyai.cn/zh/translate)
15. [SimplifyAI 일반 문서 번역](https://translate.simplifyai.cn/)
16. [Mate Translate 기능 안내](https://matetranslate.com/en)
17. [Lingvanex Windows 번역기](https://lingvanex.com/products/windows-translator/)
18. [Lingvanex 보안 번역 소프트웨어](https://lingvanex.com/products/secure-translation-software/)
19. [SYSTRAN Translate Pro 및 엔터프라이즈 배포](https://www.systransoft.com/translation-products/translate-pro/)
20. [NetEase Youdao 번역](https://fanyi.youdao.com/)
21. [바이두 번역 및 동영상 번역 포털](https://fanyi.baidu.com/)
22. [Tencent TranSmart 제품 소개](https://transmart.qq.com/zh-CN/intro)
23. [Caiyun Xiaoyi(LingoCloud) 문서 도움말](https://docs.caiyunapp.com/lingocloud-app/lingocloud-introduction/app-files-trans.html)
24. [QuillBot Translate 및 PDF 포털](https://quillbot.com/translate)
25. [Equalang API 사양 및 문서](https://equalang.com/llms-full.txt?utm_source=github)
26. [PDFMathTranslate 공식 GitHub 저장소](https://github.com/PDFMathTranslate/PDFMathTranslate)
27. [PDFMathTranslate 고급 옵션 문서](https://github.com/PDFMathTranslate/PDFMathTranslate/blob/main/docs/ADVANCED.md)
28. [BabelDOC 공식 GitHub 저장소](https://github.com/funstory-ai/BabelDOC)
29. [LibreTranslate 공식 GitHub 저장소](https://github.com/LibreTranslate/LibreTranslate)
30. [LibreTranslate 공식 문서 및 API 가이드](https://docs.libretranslate.com/)
31. [Argos Translate 공식 GitHub 저장소](https://github.com/argosopentech/argos-translate)
32. [Pot 데스크톱 번역 공식 GitHub 저장소](https://github.com/pot-app/pot-desktop)
33. [Translate Shell 공식 GitHub 저장소](https://github.com/soimort/translate-shell)
