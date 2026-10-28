# Awesome Translation Tools

> A curated directory of translation tools and workflows across travel, web reading, formatted documents, academic research, open-source local engines, and developer pipelines.

[English](README.md) | [简体中文](README.zh-CN.md) | [日本語](README.ja.md) | [한국어](README.ko.md) | [Deutsch](README.de.md) | [Français](README.fr.md) | [Español](README.es.md) | [Português (Brasil)](README.pt-BR.md) | [Italiano](README.it.md) | [Русский](README.ru.md) | [العربية](README.ar.md) | [हिन्दी](README.hi.md) | [Bahasa Indonesia](README.id.md) | [Türkçe](README.tr.md)

---

Translation tasks differ fundamentally by context: deciphering a street sign or menu on a mobile phone, reading foreign documentation inside a browser, translating complex slide decks and contracts without breaking layouts, preserving mathematical formulas in academic papers, running private batch translations in a terminal, or following uncaptioned video streams.

We are the **[Equalang](https://equalang.com/?utm_source=github)** team. This directory provides a practical, task-oriented catalog of established translation products and prominent open-source projects. For each tool, we summarize documented capabilities, entry points, deployment modes, and operational constraints to help you identify the right solution for your workflow.

---

## Contents

- [1. On-the-Go Travel & Spoken Exchange: Multi-Modal and Spoken Inputs](#1-on-the-go-travel--spoken-exchange-multi-modal-and-spoken-inputs)
  - [Google Translate](#google-translate)
  - [Apple Translate](#apple-translate)
  - [Microsoft Translator](#microsoft-translator)
  - [Papago](#papago)
  - [iTranslate](#itranslate)
- [2. In-Context Web Reading & Language Learning: Reading Without Leaving the Page](#2-in-context-web-reading--language-learning-reading-without-leaving-the-page)
  - [Immersive Translate](#immersive-translate)
  - [Mate Translate](#mate-translate)
  - [Reverso](#reverso)
  - [Yandex Translate](#yandex-translate)
- [3. Complex Document Layouts & Enterprise Workflows: Preserving Formats and Assets](#3-complex-document-layouts--enterprise-workflows-preserving-formats-and-assets)
  - [DeepL](#deepl)
  - [O.Translator](#otranslator)
  - [SimplifyAI](#simplifyai)
  - [Lingvanex](#lingvanex)
  - [SYSTRAN](#systran)
- [4. Academic Writing, Refinement & Human-in-the-Loop Collaboration: Polishing the Output](#4-academic-writing-refinement--human-in-the-loop-collaboration-polishing-the-output)
  - [Youdao Translate (NetEase Youdao)](#youdao-translate-netease-youdao)
  - [Baidu Translate](#baidu-translate)
  - [TranSmart (Tencent Interactive Translation)](#transmart-tencent-interactive-translation)
  - [LingoCloud (Caiyun Xiaoyi)](#lingocloud-caiyun-xiaoyi)
  - [QuillBot Translate](#quillbot-translate)
- [5. Open-Source Ecosystem: Local Engines, APIs, Desktop Clients & Scientific PDF Pipelines](#5-open-source-ecosystem-local-engines-apis-desktop-clients--scientific-pdf-pipelines)
  - [5.1 Scientific & Academic PDF Pipelines](#51-scientific--academic-pdf-pipelines)
    - [PDFMathTranslate (pdf2zh)](#pdfmathtranslate-pdf2zh)
    - [BabelDOC](#babeldoc)
  - [5.2 Self-Hostable Engines & APIs](#52-self-hostable-engines--apis)
    - [LibreTranslate](#libretranslate)
    - [Argos Translate](#argos-translate)
  - [5.3 Desktop & Terminal Frontends](#53-desktop--terminal-frontends)
    - [Pot (pot-desktop)](#pot-pot-desktop)
    - [Translate Shell](#translate-shell)
- [6. Connected End-to-End Workflows:](#6-connected-end-to-end-workflows-equalang) [Equalang](https://equalang.com/?utm_source=github)
  - [1. Whole-File Document Translation with Layout Preservation](#1-whole-file-document-translation-with-layout-preservation)
  - [2. In-Browser Reading & Subtitle Generation](#2-in-browser-reading--subtitle-generation)
  - [3. Installation-Free Spoken Communication & On-Site Exchange](#3-installation-free-spoken-communication--on-site-exchange)
  - [4. Integration for AI Agents and Developers](#4-integration-for-ai-agents-and-developers)
- [7. Task-Based Decision Guide](#7-task-based-decision-guide)
- [8. Directory Principles & Verification Criteria](#8-directory-principles--verification-criteria)
- [9. Sources](#9-sources)

---

## 1. On-the-Go Travel & Spoken Exchange: Multi-Modal and Spoken Inputs

Travel and fieldwork demand quick activation, reliable multi-modal recognition, and offline readiness when network connectivity is limited.

### Google Translate
[Google Translate on mobile](https://support.google.com/translate) integrates instant camera OCR, photo imports, handwriting input, and split-screen face-to-face conversation. Travelers can download language packs in advance for offline text and offline camera translation. Spoken conversational translation includes multiple display layouts, though offline live speech interpretation is limited to specific Pixel devices and selected language pairs.

On desktop browsers, Google Translate provides a dedicated [document translation portal](https://support.google.com/translate/answer/2534559?co=GENIE.Platform%3DDesktop&hl=en) that accepts DOCX, PDF, PPTX, and XLSX files. This desktop tool is designed for digital files; scanned PDF pages containing pure images are preserved in the downloaded file without OCR translation.

<p align="center"><img src="assets/google-page@2x.webp" alt="Google Translate official product overview page" width="640"><br><sub>Official Google Translate product overview page and mobile app download section</sub></p>

### Apple Translate
For iPhone and iPad users, the system-level [Apple Translate app](https://support.apple.com/en-gb/guide/iphone/iphd74cb450f/ios) requires no separate installation. It handles typed text, voice input, camera text detection, and split-screen face-to-face conversation. Its conversational mode can automatically detect which language is being spoken, eliminating the need to manually toggle the microphone between speakers. Downloaded language packs enable on-device text lookups without a cellular connection.

Within the Apple operating system, [live translation features](https://support.apple.com/en-us/123720) also extend to Messages, Phone, and FaceTime. Live phone call translation is part of Apple Intelligence, requiring compatible hardware and system versions, and is subject to regional eligibility rules (for example, devices purchased in mainland China currently do not support these advanced Apple Intelligence call features).

<p align="center"><img src="assets/apple-page@2x.webp" alt="Apple Support guide for translating on iPhone" width="640"><br><sub>Apple Support guide page for translating words and phrases on iPhone</sub></p>

### Microsoft Translator
The [Microsoft Translator mobile app](https://www.microsoft.com/en-us/translator/apps/features/) provides text translation in 100+ languages, real-time speech translation, and image translation. Its multi-device conversation feature (including Presenter mode, room codes, and browser joining) has been retired, as documented in the [iOS App Store release notes](https://apps.apple.com/us/app/microsoft-translator/id1018949559) and the [Microsoft Speech SDK release notes](https://learn.microsoft.com/en-us/azure/ai-services/speech-service/releasenotes).

The consumer app does not support translating external movies, video files, or media recordings directly. While [Microsoft's feature overview](https://www.microsoft.com/en-us/translator/apps/features/) lists single-device split-screen translation, offline language packs, and a phrasebook, the current App Store description lists text, speech, and image translation, so check inside the app before relying on offline packs or the phrasebook.

<p align="center"><img src="assets/microsoft-page@2x.webp" alt="Microsoft Translator official features page" width="640"><br><sub>The screenshot shows Microsoft's features page as captured in October 2026, and the page still describes the multi-device conversation feature, which Microsoft has retired.</sub></p>

### Papago
Developed by NAVER in South Korea, [Papago](https://papago.naver.com/) provides practical features for East Asian languages including Korean, English, Japanese, and Chinese. On mobile devices, its [application](https://play.google.com/store/apps/details?hl=en-US&id=com.naver.labs.translator) offers face-to-face dialogue, an Edu mode for creating study notes from printed text, and the Papago Mini floating window, making it handy for dining, transit queries, and study in Korea.

For web page translation, available entry points differ between platforms: NAVER has discontinued the standalone website translation tool on the desktop web portal, directing PC users to its Papago-powered [Whale browser](https://whale.naver.com/), while the [Papago mobile app](https://help.naver.com/service/16448/contents/15637?lang=ko&osType=MOBILE) still retains a website translation option within its side menu. When language packs are downloaded on compatible devices meeting system prerequisites (as outlined in [NAVER's offline documentation](https://help.naver.com/service/16448/contents/10663?osType=MOBILE), requiring at least 4GB RAM, and Android 14+ with dedicated voice packages for speech), offline translation supports text and voice between Korean, English, Japanese, and Simplified Chinese. Note that offline mode does not cover photo OCR, conversation mode, web pages, or document files.

<p align="center"><img src="assets/papago-page@2x.webp" alt="NAVER Papago official web translation interface" width="640"><br><sub>NAVER Papago web translation workspace</sub></p>

### iTranslate
[iTranslate](https://itranslate.com/) is recognized for its integrated [Keyboard Extension](https://itranslate.com/features/keyboard-translations/index.html). When drafting messages in WhatsApp, iMessage, or email, users can translate text directly within the keyboard interface, avoiding constant switching between separate apps.

It also provides downloadable packs for common travel expressions and basic phrasebooks through its [offline tools](https://itranslate.com/features/offline-translations/index.html), making it practical to review essential phrases before traveling. Feature availability varies across operating systems, and offline voice capabilities are restricted to a select list of major languages.

<p align="center"><img src="assets/itranslate-page@2x.webp" alt="iTranslate official homepage" width="640"><br><sub>iTranslate homepage featuring mobile application interface previews</sub></p>

---

## 2. In-Context Web Reading & Language Learning: Reading Without Leaving the Page

When reviewing foreign articles or documentation, jumping back and forth to an external translation tab interrupts focus. In-context tools embed translation directly into the active reading environment.

### Immersive Translate
[Immersive Translate](https://immersivetranslate.com/) is a browser extension that inserts translated paragraphs directly beneath the original web text, presenting a clean bilingual layout. It also supports creating bilingual EPUB e-books, viewing PDFs, and translating text inside browser input fields.

For multimedia, Immersive Translate translates existing subtitle tracks across platforms like YouTube and Netflix. In addition, its [AI video translation](https://immersivetranslate.com/video/ai-video-translator/) features speech recognition to generate bilingual subtitles for uncaptioned videos on supported platforms like YouTube, alongside a dedicated [YouTube live translation portal](https://livetranslate.immersivetranslate.com/zh-CN). Subtitle generation from uncaptioned audio depends on browser compatibility, audio clarity, and platform streaming conditions.

<p align="center"><img src="assets/immersive-page@2x.webp" alt="Immersive Translate official homepage" width="640"><br><sub>Immersive Translate homepage and browser extension download portal</sub></p>

### Mate Translate
[Mate Translate](https://matetranslate.com/en) is tailored for macOS, iOS, and mainstream desktop browsers. While browsing, double-clicking any word displays an immediate pop-up definition, selecting text brings up quick contextual translations, full-page translation switches between original and translated views, and a persistent Mac menu-bar utility is provided.

For language learners, Mate allows users to click words on web pages or within Netflix subtitles to save them to a custom Phrasebook, which supports custom categorization and CSV export for external review. In desktop browsers like Chrome, its extension also allows users to select text within the built-in PDF viewer to trigger translations directly.

<p align="center"><img src="assets/mate-page@2x.webp" alt="Mate Translate official homepage" width="640"><br><sub>Mate Translate homepage showing multi-platform interface previews</sub></p>

### Reverso
For writers and learners seeking to verify natural word usage, [Reverso Context](https://context.reverso.net/translation/about) provides bilingual sentence pairs drawn from films, international publications, and multilingual websites, accompanied by verb conjugation tables and synonym recommendations. Because example sentences originate from public multilingual corpora, users should assess context suitability for sensitive or formal drafts.

Its document portal, [Reverso Documents](https://www.reverso.net/documents/en), accepts PDF, Word, PowerPoint, Excel, and select localization files. It provides an in-browser segment-by-segment review interface where teams can collaborate on edits before downloading the completed file.

<p align="center"><img src="assets/reverso-page@2x.webp" alt="Reverso official translation interface" width="640"><br><sub>Reverso web translation interface and navigation bar</sub></p>

### Yandex Translate
The [Yandex Translate web portal](https://yandex.com/support/translate-desktop/en/) and mobile apps handle text, images, websites, and documents. Its Android client includes a detailed dictionary that displays phonetic transcriptions, definitions, synonyms, and morphological inflections for supported languages.

On mobile, the Android app comes with a pre-installed English-Russian [offline dictionary](https://yandex.ru/support/translate-app-android/en/offline-mobile), while additional language packs can be downloaded for offline typed text translation. The desktop interface accommodates standard Office and PDF uploads. Note the distinction between Yandex Translate as a standalone service and Yandex Browser, which houses proprietary automatic video voiceover features.

<p align="center"><img src="assets/yandex-page@2x.webp" alt="Yandex Translate official web interface" width="640"><br><sub>Yandex Translate input interface and side navigation</sub></p>

---

## 3. Complex Document Layouts & Enterprise Workflows: Preserving Formats and Assets

When handling presentation decks, supplier contracts, or technical manuals, distorted layouts require significant manual correction. These tools prioritize layout preservation, terminology control, and asset reuse.

### DeepL
[DeepL Translator](https://www.deepl.com/en/features) offers detailed configuration options for text and document workflows. Users can build [Glossaries](https://www.deepl.com/en/features/glossary) to enforce preferred company or technical translations, and toggle between formal and informal tone registers in supported languages.

Its [document translation service](https://www.deepl.com/en/features/document-translation) accepts Word, PDF, PPT, Excel, HTML, and SRT files (with format access varying by account type). The product ecosystem also includes DeepL Write for text polishing, [DeepL Voice for Online Meetings](https://support.deepl.com/hc/en-us/articles/16810100955676-About-DeepL-Voice-for-Online-Meetings) for real-time captions on Teams and Zoom (requiring Voice licensing and host permissions), and an official Model Context Protocol (MCP) guide for AI agents.

<p align="center"><img src="assets/deepl-page@2x.webp" alt="DeepL official web translation workspace" width="640"><br><sub>DeepL web translator interface</sub></p>

### O.Translator
[O.Translator](https://otranslator.com/en/product-info) focuses on layout-preserving document translation. In addition to PDF, Word, PPT, and Excel, it supports publishing and localization formats such as EPUB e-books, InDesign (IDML), Illustrator (AI), OpenDocument, subtitle files (SRT/ASS), and comic archives (CBZ/CBR), with built-in OCR for scanned pages. Layout accuracy depends on font embedding and target text expansion.

Before translating an entire file, O.Translator allows users to inspect a partial layout preview. It supports importing glossaries via XLSX or TBX, and provides a [developer API](https://www.otranslator.com/en/developer/v1). Its media option is designed for transcribing uploaded audio and video files into subtitle files, rather than real-time browser stream translation.

<p align="center"><img src="assets/otranslator-page@2x.webp" alt="O.Translator official product homepage" width="640"><br><sub>O.Translator homepage and document upload section</sub></p>

### SimplifyAI
SimplifyAI operates two distinct websites: an AI-driven [Complex Document Workbench](https://simplifyai.cn/zh/translate) (simplifyai.cn/zh) and a [General Document Translation portal](https://translate.simplifyai.cn/) (translate.simplifyai.cn).

Within the workbench, the system can extract high-frequency terms prior to translation for user review across Word, PPTX, InDesign, PDF, and EPUB files. The workbench also provides AI Editing for Word and InDesign (supporting native Word track changes), bilingual data export (Excel/XLIFF), structured Markdown/JSON extraction, and visual checks for text overflow and font layout, making it well-suited for prepress and design asset localization. For straightforward everyday file translation, the general translation portal offers a simpler direct flow.

<p align="center"><img src="assets/simplifyai-page@2x.webp" alt="SimplifyAI official homepage" width="640"><br><sub>SimplifyAI homepage showing its complex document workbench and modules</sub></p>

### Lingvanex
[Lingvanex](https://lingvanex.com/) provides desktop, mobile, and browser clients across Windows and macOS. Its [Windows desktop translator](https://lingvanex.com/products/windows-translator/) supports system-wide shortcuts (such as double-tapping Ctrl+C on highlighted text) and allows offline text and local DOCX/ODT file translation after downloading language packs.

Beyond consumer applications, Lingvanex offers downloadable [Secure Translation Software](https://lingvanex.com/products/secure-translation-software/) desktop software for offline enterprise use, as well as separate On-premise Machine Translation solutions for private network environments.

<p align="center"><img src="assets/lingvanex-page@2x.webp" alt="Lingvanex official homepage" width="640"><br><sub>Lingvanex homepage featuring enterprise translation and on-premise solutions</sub></p>

### SYSTRAN
SYSTRAN targets enterprise and institutional localization requirements. Its cloud service, [SYSTRAN Translate Pro](https://www.systransoft.com/translation-products/translate-pro/), is available immediately for Word, PowerPoint, Excel, and PDF files, offering pre-configured domain models for legal, financial, and industrial documentation alongside custom glossaries and translation memory (TM).

For organizations with data sovereignty requirements, SYSTRAN provides [Translate Server](https://www.systransoft.com/translation-products/translate-server/) for on-premise deployment behind corporate firewalls, dedicated Private Cloud environments, and batch [APIs](https://www.systransoft.com/translation-products/translate-api/) for document pipelines.

<p align="center"><img src="assets/systran-page@2x.webp" alt="SYSTRAN Translate Pro official product page" width="640"><br><sub>SYSTRAN Translate Pro official product overview interface</sub></p>

---

## 4. Academic Writing, Refinement & Human-in-the-Loop Collaboration: Polishing the Output

Translation is often the initial phase of a broader writing or research workflow. Checking dictionary definitions, polishing phrasing, and interactive human-machine editing help ensure formal scholarly standards.

### Youdao Translate (NetEase Youdao)
Connecting with NetEase Youdao's dictionary ecosystem, [Youdao Translate](https://fanyi.youdao.com/) links vocabulary lookup, translation, and writing assistance. In addition to standard text and file translation, its web portal offers dedicated entries for "arXiv Paper Translation" and academic text polishing.

After translating research excerpts, users can run grammar checks, evaluate synonym choices, or adjust academic tone, helping students and researchers review foreign literature and draft manuscripts. Format and language scopes for paper polishing and media modules differ from the general dictionary lookup.

<p align="center"><img src="assets/youdao-page@2x.webp" alt="NetEase Youdao Translate official web workspace" width="640"><br><sub>NetEase Youdao Translate web interface and feature navigation</sub></p>

### Baidu Translate
[Baidu Translate](https://fanyi.baidu.com/) provides broad client coverage for Chinese-speaking users. Its desktop software features a compact floating window and shortcut text selection across local desktop apps, while its mobile app combines photo translation, spoken practice, and dictionary references.

In addition, Baidu hosts a standalone [Baidu Video Translation portal](https://fanyi-video.baidu.com/). Users upload media files to generate aligned bilingual subtitle tracks, review and edit them in an online editor, and export finalized subtitle files. This is an upload-based post-production tool rather than an automatic interpreter for live web playback.

<p align="center"><img src="assets/baidu-page@2x.webp" alt="Baidu Translate official website page" width="640"><br><sub>Baidu Translate official web interface</sub></p>

### TranSmart (Tencent Interactive Translation)
Developed by Tencent AI Lab, [TranSmart](https://transmart.qq.com/zh-CN/intro) is designed around interactive human-machine collaboration. Rather than generating a static output for copying, TranSmart suggests word-level and sentence-level predictive completions in real time, integrating confirmed bilingual pairs into active translation memory.

Translators can place their cursor anywhere in the translated text to make adjustments, prompting the system to refresh downstream suggestions dynamically. This keeps terminology decisions and sentence pacing in the hands of the user, operating as a collaborative editor distinct in focus from Tencent's standalone consumer dictionary mobile apps.

<p align="center"><img src="assets/transmart-page@2x.webp" alt="Tencent TranSmart official webpage" width="640"><br><sub>Tencent TranSmart official web interface</sub></p>

### LingoCloud (Caiyun Xiaoyi)
[LingoCloud](https://www.caiyunapp.com/?lang=zh) is widely used for Chinese, English, and Japanese workflows. Its browser extension delivers bilingual in-page web reading with shared public and personal glossary support. Its [document translation service](https://docs.caiyunapp.com/lingocloud-app/lingocloud-introduction/app-files-trans.html) (referencing mobile app guidelines) accepts formats like PDF, Word, PPT, Excel, EPUB, TXT, and SRT, delivering downloaded outputs primarily in PDF or Word format depending on the source file.

Its desktop software also features [LingoCloud Interpretation](https://www.caiyunapp.com/interpretation/), which can capture microphone audio or intercept system audio output from running applications (such as Zoom, Teams, or Chrome on Windows) to render live dual-language subtitles. Desktop interpretation is subject to operating system audio capture boundaries: on Windows, system audio capture works across supported conference and media apps; on macOS, internal system audio recording routes are currently unsupported due to macOS system updates, leaving microphone capture as the operational route.

<p align="center"><img src="assets/caiyun-page@2x.webp" alt="LingoCloud official website page" width="640"><br><sub>LingoCloud official web interface</sub></p>

### QuillBot Translate
[QuillBot Translate](https://quillbot.com/translate) operates within QuillBot's writing and editing ecosystem. When translating text, the interface provides formality options and displays definitions and synonyms in supported languages.

Translated text can be copied smoothly into its Paraphraser and Grammar Checker to refine sentence flow. The platform also maintains a dedicated [Translate PDF page](https://quillbot.com/translate-pdf) for uploading and reviewing single PDF documents. Supported languages vary between the translation, grammar, and paraphrasing tools.

<p align="center"><img src="assets/quillbot-page@2x.webp" alt="QuillBot official Chrome Web Store extension page" width="640"><br><sub>Official Chrome Web Store product page for the QuillBot browser extension</sub></p>

---

## 5. Open-Source Ecosystem: Local Engines, APIs, Desktop Clients & Scientific PDF Pipelines

Developers, privacy-conscious teams, and academic researchers often need inspectable code, local offline execution, or custom automation pipelines. The open-source translation ecosystem spans several distinct architectural layers:

- **Scientific PDF layout tools**: Translate complex academic papers while preserving multi-column layouts, formulas, and figures.
- **Self-hostable translation services**: Provide HTTP REST API endpoints and web UIs for local network deployment.
- **Embedded offline translation engines**: Run neural machine translation locally via Python libraries without external network dependencies.
- **Desktop & terminal frontends**: Integrate multi-engine lookups, clipboard monitoring, OCR, and shell pipelines.

> [!IMPORTANT]
> Running open-source code locally does not automatically mean translations are offline or private. A tool may run locally while querying cloud APIs by default. Truly offline translation requires both local model assets and a local translation engine.

### 5.1 Scientific & Academic PDF Pipelines

#### PDFMathTranslate (pdf2zh)
[PDFMathTranslate](https://github.com/PDFMathTranslate/PDFMathTranslate) (GNU AGPL v3) is an open-source tool tailored for scientific and academic PDF documents. It preserves multi-column paper structures, mathematical notation, embedded graphics, tables of contents, and annotations.

- **Dual and Mono Outputs**: Generates both translated-only (`-mono.pdf`) and bilingual comparison (`-dual.pdf`) documents.
- **Interfaces & Integrations**: Provides command-line tools (CLI), an interactive WebUI, Docker container deployment, and Model Context Protocol (MCP) support. A linked Zotero integration plugin is available as a companion project.
- **Translation Backends**: Employs a pluggable architecture supporting Google Translate (documented default), DeepL, OpenAI-compatible APIs, and local Ollama instances. Local deployment via Docker or WebUI does not imply offline operation if cloud backends are configured.
- **OCR Support**: Includes experimental OCR for black-text on white-background scanned pages (downloads language model assets on first use, which can then be reused locally).

<p align="center"><img src="assets/pdfmathtranslate-page.webp" alt="PDFMathTranslate official GitHub repository page" width="640"><br><sub>Official PDFMathTranslate repository overview illustrating academic PDF layout translation and CLI/WebUI workflows</sub></p>

#### BabelDOC
[BabelDOC](https://github.com/funstory-ai/BabelDOC) (GNU AGPL v3) is a document-level scientific paper translation and bilingual comparison library, designed primarily to be embedded into Python applications, accompanied by a debugging CLI.

- **Layout & Output Control**: Supports mono or dual outputs, same-page side-by-side or alternating original/translated pages, selective page translation, splitting and merging large PDFs, custom glossary CSV input, and formula preservation. Table text translation is explicitly documented as experimental.
- **Backend Architecture**: Requires a configured translation backend via OpenAI-compatible endpoints or a local Ollama instance. As a PDF processing and layout engine, it does not bundle a universal translation engine itself.
- **Offline Assets & Boundaries**: Provides warmup routines and offline asset generation/restoration for document layout models and fonts. Fully offline execution requires both pre-cached assets and a locally running translation backend (such as local Ollama). Documentation highlights primary validation on English-to-Chinese workflows, with an experimental OCR workaround for black text on white backgrounds.

<p align="center"><img src="assets/babeldoc-page.webp" alt="BabelDOC official GitHub repository page" width="640"><br><sub>Official BabelDOC repository overview demonstrating document-level scientific PDF translation library capabilities</sub></p>

### 5.2 Self-Hostable Engines & APIs

#### LibreTranslate
[LibreTranslate](https://github.com/LibreTranslate/LibreTranslate) (GNU AGPL v3) is a free and open-source self-hostable machine translation API service with an included web UI, built on top of the Argos Translate engine.

- **API & Web Service**: Exposes REST API endpoints for text translation, source language detection, and HTML/markup handling. It functions as an independent service layer rather than a proxy to commercial translation APIs.
- **Local Deployment & Privacy**: Can run completely on local hardware without sending data to external third parties once dependencies and language models are installed. Using a public hosted instance remains network-dependent. API key access control can be enabled or disabled according to host requirements.
- **Language Coverage & File Formats**: Available language pairs depend on installed language models. Through companion projects like argos-translate-files, file translation supports formats including TXT, ODT, ODP, DOCX, PPTX, EPUB, HTML, SRT, and PDF.

<p align="center"><img src="assets/libretranslate-page.webp" alt="LibreTranslate official GitHub repository page" width="640"><br><sub>Official LibreTranslate repository overview showing self-hosted translation API and web interface features</sub></p>

#### Argos Translate
[Argos Translate](https://github.com/argosopentech/argos-translate) (MIT License / CC0 option declared in README) is an open-source offline Python translation library and command-line tool, with a separately installable GUI client.

- **Modular Model Packages**: Downloads and manages language model packages using the `.argosmodel` extension. When a direct language pair is unavailable, it can pivot through installed intermediate pairs (e.g., translating through English).
- **Ecosystem Engine**: Serves as the underlying machine translation engine for LibreTranslate. Companion projects extend its capabilities to HTML translation (`translate-html`) and file processing (`argos-translate-files`).
- **Offline Operation**: Runs fully offline once models are installed; downloading package indices and initial models requires internet connectivity.

<p align="center"><img src="assets/argos-translate-page.webp" alt="Argos Translate official GitHub repository page" width="640"><br><sub>Official Argos Translate repository overview detailing the modular offline translation engine and package system</sub></p>

### 5.3 Desktop & Terminal Frontends

#### Pot (pot-desktop)
[Pot](https://github.com/pot-app/pot-desktop) (GNU GPL v3) is a cross-platform desktop translation tool for Windows, macOS, and Linux, supporting selection translation via hotkeys, typed input, clipboard monitoring, screenshot OCR, and screenshot translation. The upstream repository was archived by the owner on September 7, 2026, and is now read-only.

- **Multi-Service Aggregation**: Allows querying multiple translation and dictionary services simultaneously to compare results side-by-side. Supports text-to-speech (TTS), vocabulary export to Anki and Eudic, and plugin extensions.
- **Pluggable Backends & OCR**: Aggregates cloud translation providers, OpenAI-compatible APIs, and local Ollama endpoints. OCR choices include platform-native options (Windows system OCR, Apple Vision, Linux Tesseract), Tesseract.js, or local plugins.
- **Offline Execution Routes**: Selection and typed text translation require only a configured local translation backend (such as a local Ollama instance); screenshot translation additionally requires an offline OCR engine (such as platform-native OCR or Tesseract). Cloud services route requests over the network.

<p align="center"><img src="assets/pot-desktop-page.webp" alt="Pot desktop translation official GitHub repository page" width="640"><br><sub>Official Pot desktop client repository overview highlighting multi-interface translation, OCR, and clipboard workflows</sub></p>

#### SoloPup Subtitle Studio
[SoloPup Subtitle Studio](https://github.com/OakcoderX/solopup-subtitle-studio) (MIT) is a local browser workspace for reviewing English subtitles against Chinese-language audio, with separate source/translation tracks and SRT/ITT export. Version 2.0.0-rc.5 is a public preview.

- **Review workflow**: Imports corresponding Chinese and English SRT screens, compares text and timing against the video, and preserves edits and review decisions. Also offers an ordinary/SDH accessibility-caption workflow.
- **Local versus cloud**: Reviewing an existing subtitle pair requires no AI account. Optional Qwen cloud processing uses the user's provider account, may incur charges, and sends required task inputs to that provider. Optional local ASR requires separate dependencies and model weights; the application is not itself a bundled offline translation engine.
- **Boundaries**: Automatic production targets English US/UK; bilingual controls use Chinese. Syllable estimates and format checks do not replace human audiovisual review. macOS has been tested locally; Windows/Linux manual acceptance is incomplete.

#### Translate Shell
[Translate Shell](https://github.com/soimort/translate-shell) (The Unlicense / Public Domain) is a versatile command-line translation tool (executable `trans`) for Unix-like terminal environments.

- **CLI Lookup & Dictionary**: Supports word definitions, phrase translation, concise dictionary mode, interactive REPL sessions, and language identification directly in the shell.
- **Unix Pipelines**: Integrates with standard input/output (`stdin` / `stdout`), processes text files directly, and supports speech synthesis when an external audio player is installed.
- **Engine Layer**: Operates as a lightweight client front end connecting to public translation services (Google Translate by default, Bing Translator, Yandex.Translate, and Apertium).
- **Boundaries**: Does not bundle local neural translation models; standard operation depends on external network connectivity to selected engine services. File translation is designed for plain text streams, not formatted documents.

<p align="center"><img src="assets/translate-shell-page.webp" alt="Translate Shell official GitHub repository page" width="640"><br><sub>Official Translate Shell repository overview showing terminal command-line translation and pipeline integration</sub></p>

---

## 6. Connected End-to-End Workflows: [Equalang](https://equalang.com/?utm_source=github)

Reviewing these tools demonstrates that each service has developed clear capabilities for specific tasks. In everyday work, however, requirements frequently intersect:

You might read an online white paper in your browser, download an accompanying PDF with tables and diagrams, watch a video lecture without captions, and then prepare an executive summary in Word while coordinating directly with international collaborators. Switching between isolated software tools and file converters fragments the workflow.

We designed **[Equalang](https://equalang.com/?utm_source=github)** to connect these tasks into a continuous, side-by-side translation workflow, delivering coordinated translation support across documents, web pages, videos, and live communication.

<p align="center"><img src="assets/equalang-en-page@2x.webp" alt="Equalang official English homepage" width="640"><br><sub><a href="https://equalang.com/?utm_source=github">Equalang</a> official English website homepage</sub></p>

### 1. Whole-File Document Translation with Layout Preservation
When translating full documents, [Equalang](https://equalang.com/?utm_source=github) focuses on structural preservation and post-translation usability, providing tailored workflows across research literature, presentations, and everyday office files:

- **PDF Documents & Reading**: [Equalang](https://equalang.com/?utm_source=github) preserves multi-column layouts, headers, footers, and captions, reconnecting sentences split across page breaks before translating, while maintaining table structures, inline formulas, and internal document links. As outlined in our [academic PDF reading walkthrough](https://equalang.com/blog/translate-and-read-pdf-documents?utm_source=github), readers can view the translated file alongside the original in a side-by-side layout, grasping core arguments in their primary language first before cross-referencing specific terminology and data on the original page.

- **PowerPoint Presentations**: In our [slide deck formatting guide](https://equalang.com/blog/translate-powerpoint-keep-formatting?utm_source=github), translated PPTX files preserve native editable tables rather than flattening them into static images. Word-level styling—such as bolding, italics, and font colors within a single sentence—is accurately mapped to corresponding translated phrases. Key terms and headings remain consistent across slides, and text boxes automatically scale down font sizes when translations expand to prevent text overflow or covering graphics.

- **Word & Excel Office Files**: In our verified [Word translation test](https://equalang.com/blog/translate-word-document-keep-formatting?utm_source=github), translated DOCX files retained headings, bulleted lists, pricing tables, and bold formatting, allowing direct editing in Microsoft Word. In our [Excel price sheet validation](https://equalang.com/blog/translate-excel-file?utm_source=github), formulas and numbers remained untouched while duplicate text strings across cells were translated only once.

- **E-Books & Formatted Media**: EPUB e-books retain table-of-contents navigation and internal anchor links. For recorded audio and video files up to 180 minutes, translation and transcription tasks are submitted via our Developer API and Agent Skill/MCP integration (rather than a general web document upload portal), outputting timestamped bilingual SRT/VTT subtitle files or source transcripts.

### 2. In-Browser Reading & Subtitle Generation
Through our lightweight [browser extension](https://equalang.com/extension?utm_source=github) (with installation guides for Chrome, Edge, and Firefox, plus a temporary Mac Safari mode for Safari 18.4+), translation integrates directly into your daily reading:

- **Under-Paragraph Bilingual Web Reading**: Translated paragraphs appear directly beneath the original text as you scroll. A floating icon can be toggled in settings for on-demand word lookups. When viewing local PDFs, users can enable "Allow access to file URLs" in extension management to select words for lookup.

- **Bilingual Video Subtitles**: Compatible with YouTube, Netflix, TikTok, and Bilibili, as explored in our [bilingual video viewing guide](https://equalang.com/blog/watch-videos-with-bilingual-subtitles?utm_source=github). Beyond translating existing subtitles, the extension can capture audio streams to generate real-time bilingual subtitles for **uncaptioned videos** (subject to browser environment and media encryption limits, verified on YouTube live streams and official trailers), while simultaneously translating live chat comments on YouTube.

### 3. Installation-Free Spoken Communication & On-Site Exchange
Requiring conversational partners to install dedicated mobile applications creates friction, especially while traveling. When connected to the internet, [Equalang](https://equalang.com/?utm_source=github) delivers on-the-go photo translation and spoken interpretation directly inside standard browsers (requiring only an initial sign-in and device camera/microphone permission on first use), as outlined in our [international communication guide](https://equalang.com/blog/talk-with-overseas-partners?utm_source=github):

- **Mobile Photo Translation**: When encountering unfamiliar restaurant menus, signs, or public notices while traveling, users can snap a picture in their mobile browser. Translations overlay directly onto the photo layout, making it easy to order drinks or review notices against the original image, as illustrated in our [travel photo translation guide](https://equalang.com/blog/photo-translation-for-travel?utm_source=github).

- **Face-to-Face Mode**: Designed for in-person situations such as hotel luggage storage, asking directions, or front-desk interactions. Two speakers can place a single phone or tablet flat between them, using an inverted split-screen or side-by-side view with continuous two-way transcription and transcript export, as shown in our [travel face-to-face guide](https://equalang.com/blog/talk-face-to-face-while-traveling?utm_source=github).

- **Live Listening**: Open the web portal during an in-person presentation or lecture to receive real-time bilingual subtitles captured via the device's physical microphone, with optional text-to-speech audio and transcript export when finished (distinguished from the browser extension's streaming media audio capture).

- **Translated Calls**: Hosts log in on the web portal to generate a secure call link and share it via any messaging app. **Guests join directly through their browser without creating an account or installing any software**—they simply enter a display name and the host admits them to begin the call. Both parties speak their native language, hear translated audio, and view real-time text.

### 4. Integration for AI Agents and Developers
To help developers and teams embed translation into automated workflows:

- **Developer API**: Features instant endpoints for text alongside asynchronous file jobs supporting Idempotency-Key retries and callback notifications, as detailed in our [file translation API integration guide](https://equalang.com/blog/integrate-file-translation-api?utm_source=github).

- **Skill & MCP Integration**: We maintain open-source Agent Skills via [equalang-skill](https://github.com/equalang/equalang-skill) and official Model Context Protocol support via [@equalang/mcp](https://github.com/equalang/equalang-mcp). In environments such as Claude Code, Codex, or WorkBuddy, running a single installation prompt and configuring your API key equips your AI assistant to handle document translation and media transcription directly within your workflow, following our [AI assistant file translation guide](https://equalang.com/blog/translate-files-with-ai-assistants?utm_source=github).

---

## 7. Task-Based Decision Guide

To help you choose the right tool for your current task, refer to this task matrix:

| Primary Task | Core Requirement | Recommended Tools to Try | Key Considerations |
| :--- | :--- | :--- | :--- |
| **Travel & Spoken Dialogue** | Photo OCR, two-way dialogue, offline packs & connected travel tools | Google Translate, Apple Translate, Papago, [Equalang](https://equalang.com/?utm_source=github) | Download offline language packs in Google, Apple, or Papago (noting hardware requirements) for weak-signal areas; when connected, [Equalang](https://equalang.com/?utm_source=github) provides browser-based photo translation and face-to-face dialogue without installing apps. |
| **Multi-Device Workshops** | One-to-many presentations, multi-device participation | The directory currently lists no tool for this scenario. | Microsoft retired its multi-device conversation feature and Presenter mode in 2026 (see the Microsoft Translator section above for details), and this is why the directory lists no tool here now. |
| **In-Depth Web Reading** | Under-paragraph reading without leaving the page | Immersive Translate, [Equalang](https://equalang.com/?utm_source=github), Mate Translate | Use Immersive Translate or [Equalang](https://equalang.com/?utm_source=github) for bilingual paragraphs; use Mate Translate for switching full-page views or saving words to Phrasebooks on Mac. |
| **Uncaptioned Video & Live Streams** | Real-time subtitle generation, streaming compatibility | [Equalang](https://equalang.com/?utm_source=github), Immersive Translate | Both tools can generate subtitles from raw audio on supported platforms (like YouTube); compare browser extension workflows for live chat and stream handling. |
| **Academic Papers & Scientific PDFs** | Formula preservation, column structures, cross-page text | PDFMathTranslate, BabelDOC, [Equalang](https://equalang.com/?utm_source=github) | PDFMathTranslate and BabelDOC provide open-source pipelines with dual-PDF output and local/cloud LLM backends; [Equalang](https://equalang.com/?utm_source=github) provides browser-based side-by-side reading and layout preservation. |
| **Publishing Prepress & Design Formats** | InDesign, Illustrator, comic archives, prepress QA | SimplifyAI, O.Translator | Use SimplifyAI and O.Translator for InDesign (IDML) and design asset prepress; SimplifyAI includes AI Editing with native Word track changes. |
| **Presentations & Office Documents** | Preserving native tables, styles, formulas, and editability | [Equalang](https://equalang.com/?utm_source=github), DeepL | [Equalang](https://equalang.com/?utm_source=github) preserves PPTX native tables/styling with adaptive font sizing and Excel formula retention; use DeepL for corporate Word/Office files with glossaries. |
| **Academic Writing & Polishing** | Grammatical accuracy, formal scholarly register | Youdao Translate, QuillBot Translate, TranSmart | Youdao and QuillBot streamline translation into text refinement; TranSmart provides interactive human-in-the-loop editing. |
| **Desktop Hotkey Lookup & Multi-Engine** | Global shortcuts, OCR, comparing multiple engines | Pot, Mate Translate | Pot allows simultaneous multi-engine queries and screenshot OCR across Windows, Mac, and Linux; Mate offers a native Mac menu-bar utility. |
| **Terminal Scripting & Shell Pipelines** | CLI lookup, stdin/stdout pipelines, plain text scripts | Translate Shell, Argos Translate | Translate Shell provides lightweight CLI translation via remote engines; Argos Translate provides an offline Python CLI with local models. |
| **Self-Hosted Private API & Offline Engines** | Air-gapped networks, no third-party data transmission | LibreTranslate, Argos Translate, SYSTRAN, Lingvanex | LibreTranslate provides a self-hosted HTTP API service and WebUI; Argos Translate powers it as an offline Python library/CLI engine with modular model packages; SYSTRAN and Lingvanex offer enterprise on-premise deployments. |
| **Connected End-to-End Workflows** | Documents, streaming subtitles, web calls, and AI Agents | [Equalang](https://equalang.com/?utm_source=github) | Unified document processing, uncaptioned media subtitles, browser-based calls without app installation, and direct integration with Claude Code or WorkBuddy. |

---

## 8. Directory Principles & Verification Criteria

To maintain the practical utility and factual accuracy of this directory, entries follow strict inclusion and review criteria:

1. **Documented Features Over Marketing Claims**: Descriptions are derived from official documentation, user manuals, and confirmed repository source files. We do not claim perfect layout retention or universal format support.
2. **Clear Architectural Boundaries**: We distinguish between translation frontends, self-hostable service layers, offline translation engines, and document layout libraries. Open-source code running locally is explicitly separated from true offline execution.
3. **Task-Oriented Coverage**: Tools are grouped by practical suitability across workflows. We do not maintain subjective tier lists, quality rankings, or transient pricing figures.
4. **Transparent Maintainer Identity**: This catalog is curated and maintained by the **[Equalang](https://equalang.com/?utm_source=github)** team. [Equalang](https://equalang.com/?utm_source=github) is presented alongside other tools with verifiable feature boundaries and transparent system requirements.

**Keywords**: translation tools, document translation, bilingual web reading, academic PDF translation, open-source translation, machine translation API, layout preservation, AI agents.

---

## 9. Sources

1. [Google Translate Help Center](https://support.google.com/translate)
2. [Google Translate Desktop Document Translation](https://support.google.com/translate/answer/2534559?co=GENIE.Platform%3DDesktop&hl=en)
3. [Apple Support: Translate App Guide for iPhone](https://support.apple.com/en-gb/guide/iphone/iphd74cb450f/ios)
4. [Apple Support: Live Translation & Feature Availability](https://support.apple.com/en-us/123720)
5. [Microsoft Translator Mobile Features](https://www.microsoft.com/en-us/translator/apps/features/)
6. [Microsoft Translator on the iOS App Store](https://apps.apple.com/us/app/microsoft-translator/id1018949559)
7. [Microsoft Speech SDK Release Notes](https://learn.microsoft.com/en-us/azure/ai-services/speech-service/releasenotes)
8. [NAVER Papago Official Portal](https://papago.naver.com/)
9. [iTranslate Keyboard & Offline Features](https://itranslate.com/features/keyboard-translations/index.html)
10. [Reverso Context Usage Information](https://context.reverso.net/translation/about)
11. [Reverso Documents Portal](https://www.reverso.net/documents/en)
12. [Yandex Translate Help for Desktop & Mobile](https://yandex.com/support/translate-desktop/en/)
13. [Immersive Translate Documentation](https://immersivetranslate.com/)
14. [O.Translator Product Information & Formats](https://otranslator.com/en/product-info)
15. [SimplifyAI Complex Document Workbench](https://simplifyai.cn/zh/translate)
16. [SimplifyAI General Document Translation](https://translate.simplifyai.cn/)
17. [Mate Translate Features](https://matetranslate.com/en)
18. [Lingvanex Windows Translator](https://lingvanex.com/products/windows-translator/)
19. [Lingvanex Secure Translation Software](https://lingvanex.com/products/secure-translation-software/)
20. [SYSTRAN Translate Pro & Enterprise Deployments](https://www.systransoft.com/translation-products/translate-pro/)
21. [NetEase Youdao Translate](https://fanyi.youdao.com/)
22. [Baidu Translate & Video Translation Portal](https://fanyi.baidu.com/)
23. [Tencent TranSmart Product Introduction](https://transmart.qq.com/zh-CN/intro)
24. [Caiyun Xiaoyi (LingoCloud) Document Help](https://docs.caiyunapp.com/lingocloud-app/lingocloud-introduction/app-files-trans.html)
25. [QuillBot Translate & PDF Portal](https://quillbot.com/translate)
26. [Equalang API Specifications & Documentation](https://equalang.com/llms-full.txt?utm_source=github)
27. [PDFMathTranslate Official GitHub Repository](https://github.com/PDFMathTranslate/PDFMathTranslate)
28. [PDFMathTranslate Advanced Options Documentation](https://github.com/PDFMathTranslate/PDFMathTranslate/blob/main/docs/ADVANCED.md)
29. [BabelDOC Official GitHub Repository](https://github.com/funstory-ai/BabelDOC)
30. [LibreTranslate Official GitHub Repository](https://github.com/LibreTranslate/LibreTranslate)
31. [LibreTranslate Documentation & API Guide](https://docs.libretranslate.com/)
32. [Argos Translate Official GitHub Repository](https://github.com/argosopentech/argos-translate)
33. [Pot Desktop Translation Official GitHub Repository](https://github.com/pot-app/pot-desktop)
34. [Translate Shell Official GitHub Repository](https://github.com/soimort/translate-shell)
