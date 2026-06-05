---
title: "Developing with Accessibility"
subtitle: "Resources for Building Baseline Usability Across Platforms"
author: "Jamal Mazrui"
date: "June 2026"
version: "v1.0.0"
lang: en-US
toc: true
toc-depth: 3
abstract: |
  A directory of free, reputable resources for building software with accessibility,
  organized by platform — web, desktop (Windows, macOS, Linux), mobile (iOS and
  Android), cross-platform frameworks, command line, and voice — with cross-cutting
  sections for foundations and standards, the roles involved, and the design, content
  authoring, and auditing that span every platform. It pairs curated text and video
  tutorials carrying reading and watching times with per-platform references, free
  testing and document-checking tools, and a glossary whose abbreviations are linked
  from their first use.
keywords:
  - accessibility
  - assistive technology
  - screen reader
  - WCAG
  - ARIA
  - Section 508
  - WinForms
  - WPF
  - .NET MAUI
  - React
  - Angular
  - Vue
  - Flutter
  - React Native
  - Django
  - Alexa
  - browser extensions
  - testing tools
---

# Developing with Accessibility

Free, reputable resources for building accessible software, organized by platform.

## Introduction {#introduction}

Accessible technology has long struggled to keep pace with how quickly software evolves, and the gap is widest when accessibility is treated as an afterthought rather than built in from the start. This directory supports the opposite: developing applications within each platform's accepted accessibility guidelines, so the result is usable for everyone, including people with disabilities. The shorthand for that goal is *baseline usability* — software that can be operated with the keyboard alone, with a screen reader or other assistive technology ([AT](#at)), at increased zoom or contrast, and without relying on color or sound alone to convey meaning. Building this way also helps people facing temporary or situational barriers.

Accessible development is more than coding. It spans design, development, content authoring, and auditing, and it draws on several roles working together. This directory is organized by platform — web, desktop, mobile, cross-platform frameworks, the command line, and voice — with cross-cutting sections for the foundations and standards, the roles involved, and the design, content-authoring, and auditing work that applies across every platform. The standards that define what to meet — chiefly the Web Content Accessibility Guidelines ([WCAG](#wcag)) from the World Wide Web Consortium ([W3C](#w3c)), with [Section 508](#section-508) in the United States and [EN 301 549](#en-301-549) in Europe — are collected under Foundations. Because the audience is people who build software, the directory favors developer guidance, libraries, built-in platform techniques, and testing tools over end-user instructions.

Each entry follows a common form: a linked title, the publisher, and — for tutorials — an estimated time to read or watch in parentheses, figured at about 200 words per minute. The note *TOC* after a time means the estimate covers only the landing page, which acts as a table of contents to further pages. A leading asterisk (*), echoing the marker for a required form field, flags reading considered essential for an area. Reference documentation, standards, and tools are listed without a time. Within each platform section, resources are grouped under Learning, split into Text and Video so you can choose the medium you prefer, and Tools, which covers programming and design aids as well as testing tools. Section headings act as navigation landmarks; the Table of Contents links to each section, and the Glossary defines recurring terms, with abbreviations linked to their definitions on first use.

## Table of Contents {#table-of-contents}

- [Introduction](#introduction)
- [Foundations and Standards](#foundations-and-standards)
- [Roles in Accessible Development](#roles-in-accessible-development)
- [Web Pages and Web Applications](#web-pages-and-web-applications)
- [Desktop: Windows](#desktop-windows)
- [Desktop: macOS](#desktop-macos)
- [Desktop: Linux and GTK](#desktop-linux-and-gtk)
- [Mobile: Apple iOS and iPadOS](#mobile-apple-ios-and-ipados)
- [Mobile: Google Android](#mobile-google-android)
- [Cross-Platform Frameworks](#cross-platform-frameworks)
- [Editor and Browser Extensions](#editor-and-browser-extensions)
- [Command-Line Interfaces](#command-line-interfaces)
- [Voice and Conversational: Amazon Alexa](#voice-and-conversational-amazon-alexa)
- [Design](#design)
- [Content Authoring](#content-authoring)
- [Auditing and Testing](#auditing-and-testing)
- [Communities and Further Lists](#communities-and-further-lists)
- [Glossary](#glossary)

## Foundations and Standards {#foundations-and-standards}

The cross-cutting standards and reference hubs the rest of the directory builds on, from the W3C Web Accessibility Initiative ([WAI](#wai)) and others. Standards and reference material are listed without a reading time.

- [Accessibility Maturity Model](https://www.w3.org/TR/maturity-model/) by W3C, a framework to assess an organization's policies and procedures for delivering accessible products and to plan improvements.
- [Accessibility on MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/Accessibility) by Mozilla.
- [Accessible Name and Description Computation (accname)](https://www.w3.org/TR/accname-1.1/) by W3C.
- [AccessKit](https://github.com/AccessKit/accesskit) by the AccessKit project, a single cross-platform accessibility layer bridging to UI Automation, the macOS accessibility API, and AT-SPI.
- [Create Accessible Software and Websites](https://www.section508.gov/develop/software-websites/) by Section508.gov.
- [EN 301 549 (European ICT accessibility standard) overview](https://en.wikipedia.org/wiki/EN_301_549) on Wikipedia.
- [How People with Disabilities Use the Web](https://www.w3.org/WAI/people-use-web/) by W3C.
- [How to Meet WCAG (Quick Reference)](https://www.w3.org/WAI/WCAG22/quickref/) by W3C.
- [Section 508 ICT Testing Baseline](https://ictbaseline.access-board.gov/) by U.S. Access Board.
- [Standards and Guidelines Overview](https://www.w3.org/WAI/standards-guidelines/) by W3C.
- [Test for Accessibility](https://www.section508.gov/test/) by Section508.gov.
- [The A11y Project](https://www.a11yproject.com/) by The A11y Project.
- [WAI-ARIA Overview](https://www.w3.org/WAI/standards-guidelines/aria/) by W3C.

## Roles in Accessible Development {#roles-in-accessible-development}

Accessible software involves several roles — manager, designer, developer, author, and auditor. This directory uses *developer* expansively, to include the design, authoring, and auditing tasks involved in developing with accessibility, so those areas have their own cross-cutting sections below. The role-based curricula here, and the Accessibility Maturity Model under Foundations, help a team coordinate across roles.

- [Design and Develop Accessible Products](https://www.section508.gov/develop/) by Section508.gov.
- [Designer Modules](https://www.w3.org/WAI/curricula/designer-modules/) by W3C. (2 min TOC)
- [Developer Modules](https://www.w3.org/WAI/curricula/developer-modules/) by W3C. (3 min TOC)

## Web Pages and Web Applications {#web-pages-and-web-applications}

Building accessible web interfaces centers on the Accessible Rich Internet Applications ([ARIA](#aria)) specifications, semantic HTML, and framework-specific guidance.

### Learning

#### Text

- [Angular Accessibility Best Practices](https://angular.dev/best-practices/a11y) by the Angular team.
- [Angular CDK Accessibility (a11y) Overview](https://material.angular.dev/cdk/a11y/overview) by the Angular team.
- \* [ARIA Authoring Practices Guide (APG)](https://www.w3.org/WAI/ARIA/apg/) by W3C. (2 min TOC)
- [Developing Accessible Web Content](https://www.section508.gov/develop/web-content/) by Section508.gov.
- [Django Accessibility](https://www.djangoproject.com/accessibility/) by Django, whose admin and default form rendering target WCAG 2.2 AA.
- [GitHub Accessibility](https://accessibility.github.com/) by GitHub.
- [HTML Semantics and Accessibility Cheat Sheet](https://webaim.org/resources/htmlcheatsheet/) by WebAIM. (6 min)
- [Learn Web Accessibility](https://developer.mozilla.org/en-US/docs/Learn/Accessibility) by Mozilla. (4 min)
- [Primer: Accessibility](https://primer.style/accessibility/) by GitHub.
- [Teach Access Tutorial](https://teachaccess.github.io/tutorial/) by Teach Access. (3 min TOC)
- [The Accessibility Tree: A Training Guide for Advanced Web Development](https://whatsock.com/training/) by Level Access. (63 min)
- [Vue.js Accessibility Guide](https://vuejs.org/guide/best-practices/accessibility) by Vue.js.
- [WAI Tutorials](https://www.w3.org/WAI/tutorials/) by W3C.
- [WAI-ARIA Basics](https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Accessibility/WAI-ARIA_basics) by Mozilla.
- \* [Web Accessibility for Developers](https://pressbooks.library.torontomu.ca/wafd/) by The Chang School, Toronto Metropolitan University. (189 min)
- [Yes, Accessibility Is Also a Backend Concern](https://ericwbailey.website/published/yes-accessibility-is-also-a-backend-concern/) by Eric Bailey. (6 min)

#### Video

- [A11ycasts](https://www.youtube.com/playlist?list=PLNYkxOF6rcICWx0C9LVWWVqvHlYJyqw7g) by Google. (2 - 14 min each in a series of 14)
- [Inclusive Design 24](https://www.youtube.com/inclusivedesign24) by various presenters. (30 - 50 min each in an annual series of 26)

### Tools

- [Able Player](https://ableplayer.github.io/ableplayer/) by the Able Player project, an accessible HTML5 media player with captions, audio description, and transcripts.
- [Accessibility Insights for Web](https://accessibilityinsights.io/) by Microsoft.
- [ANDI (Accessible Name and Description Inspector)](https://www.ssa.gov/accessibility/andi/help/install.html) by the U.S. Social Security Administration.
- [Axe Linter for Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=deque-systems.vscode-axe-linter) by Deque.
- [axe-core](https://github.com/dequelabs/axe-core) by Deque.
- [axe-core-gems](https://github.com/dequelabs/axe-core-gems) by Deque, the Ruby integration for axe-core in Rails test suites.
- [capybara_accessibility_audit](https://github.com/thoughtbot/capybara_accessibility_audit) by thoughtbot, automatic checks in Rails system tests.
- [Colour Contrast Analyser (CCA)](https://www.tpgi.com/color-contrast-checker/) by TPGi.
- [eslint-plugin-jsx-a11y](https://www.npmjs.com/package/eslint-plugin-jsx-a11y) by the ESLint JSX a11y project.
- [eslint-plugin-vuejs-accessibility](https://www.npmjs.com/package/eslint-plugin-vuejs-accessibility) by the Vue.js a11y project.
- [HTML CodeSniffer](https://github.com/squizlabs/HTML_CodeSniffer) by Squiz Labs.
- [IBM Equal Access Accessibility Checker](https://github.com/IBMa/equal-access) by IBM.
- [Lighthouse](https://developer.chrome.com/docs/lighthouse/accessibility/scoring) by Google.
- [Pa11y](https://github.com/pa11y/pa11y) by the Pa11y project.
- [Radix Primitives: Accessibility](https://www.radix-ui.com/primitives/docs/overview/accessibility) by Radix UI.
- [React Aria](https://react-spectrum.adobe.com/react-aria/) by Adobe.
- [urlCheck](https://github.com/JamalMazrui/urlCheck) by Jamal Mazrui, a command-line scanner that tests web pages with Playwright and axe-core, producing HTML, CSV, XLSX, and JSON reports.
- [WAVE Web Accessibility Evaluation Tools](https://wave.webaim.org/) by WebAIM.
- [WebAIM Contrast Checker](https://webaim.org/resources/contrastchecker/) by WebAIM.

## Desktop: Windows {#desktop-windows}

Windows exposes controls through UI Automation ([UIA](#uia)), which superseded the legacy Microsoft Active Accessibility ([MSAA](#msaa)).

### Learning

#### Text

- [.NET Accessibility Best Practices](https://learn.microsoft.com/en-us/dotnet/framework/ui-automation/accessibility-best-practices) by Microsoft.
- [Accessibility Overview (XAML)](https://learn.microsoft.com/en-us/windows/apps/design/accessibility/accessibility-overview) by Microsoft.
- [Accessible Windows Apps (Win32 hub)](https://learn.microsoft.com/en-us/windows/win32/winauto/accessibility) by Microsoft.
- [Common Approaches for Enhancing Programmatic Accessibility of Win32, WinForms, and WPF Apps (WPF installment)](https://learn.microsoft.com/en-us/archive/blogs/winuiautomation/common-approaches-for-enhancing-the-programmatic-accessibility-of-your-win32-winforms-and-wpf-apps-part-4-wpf) by Microsoft.
- [Develop Accessible Windows Apps](https://learn.microsoft.com/en-us/windows/apps/develop/accessibility) by Microsoft.
- [UI Automation Overview](https://learn.microsoft.com/en-us/windows/win32/winauto/uiauto-uiautomationoverview) by Microsoft.
- [What's New in Accessibility in .NET Framework](https://learn.microsoft.com/en-us/dotnet/framework/whats-new/whats-new-in-accessibility) by Microsoft.

#### Video

No video is curated specifically for Windows; the screen-reader and tooling videos under [Auditing and Testing](#auditing-and-testing) apply.

### Tools

- [Accessibility Insights for Windows](https://accessibilityinsights.io/docs/windows/overview/) by Microsoft.
- [Accessible Event Watcher, AccEvent (Windows SDK)](https://learn.microsoft.com/en-us/windows/win32/winauto/accessible-event-watcher-objects) by Microsoft.
- [Inspect (Windows SDK)](https://learn.microsoft.com/en-us/windows/win32/winauto/inspect-objects) by Microsoft.

## Desktop: macOS {#desktop-macos}

### Learning

#### Text

- [Accessibility Fundamentals for SwiftUI](https://developer.apple.com/documentation/swiftui/accessibility-fundamentals) by Apple, much of which is shared with iOS.
- [Apple Developer: Accessibility](https://developer.apple.com/accessibility/) by Apple.
- [Human Interface Guidelines: Accessibility](https://developer.apple.com/design/human-interface-guidelines/accessibility) by Apple.

#### Video

- [Apple Developer Videos: Accessibility and Inclusion](https://developer.apple.com/videos/all-videos/?q=accessibility) by Apple, conference sessions on building accessible apps across Apple platforms.

### Tools

- [Accessibility Inspector](https://developer.apple.com/documentation/accessibility/accessibility-inspector) by Apple, bundled with Xcode.
- [Performing Accessibility Testing for Your App](https://developer.apple.com/documentation/accessibility/performing-accessibility-testing-for-your-app) by Apple.

## Desktop: Linux and GTK {#desktop-linux-and-gtk}

Linux toolkits bridge to the Assistive Technology Service Provider Interface ([AT-SPI](#at-spi)).

### Learning

#### Text

- [AT-SPI on the Accessibility Wiki](https://www.freedesktop.org/wiki/Accessibility/) by freedesktop.org.
- [GNOME Developer Documentation: Accessibility](https://developer.gnome.org/documentation/guidelines/accessibility.html) by GNOME.

#### Video

No video is curated specifically for Linux; the cross-cutting videos under [Auditing and Testing](#auditing-and-testing) apply.

### Tools

GTK and GNOME applications are inspected with Accerciser, the AT-SPI explorer bundled with GNOME; see the GNOME developer documentation under Text above.

## Mobile: Apple iOS and iPadOS {#mobile-apple-ios-and-ipados}

SwiftUI accessibility, shown under macOS, applies to iOS and iPadOS as well.

### Learning

#### Text

- [Accessibility for UIKit](https://developer.apple.com/documentation/uikit/accessibility-for-uikit) by Apple.
- [Information for Developers](https://applevis.com/developers) by AppleVis, a community hub with VoiceOver testing tips for developers.
- [Integrating Accessibility Into Your App](https://developer.apple.com/documentation/accessibility/integrating_accessibility_into_your_app) by Apple.

#### Video

Apple's accessibility sessions, listed under [Desktop: macOS](#desktop-macos), cover iOS and iPadOS as well.

### Tools

iOS apps are inspected with the Xcode Accessibility Inspector, listed under [Desktop: macOS](#desktop-macos), together with on-device VoiceOver.

## Mobile: Google Android {#mobile-google-android}

### Learning

#### Text

- [Accessibility Design Foundations](https://developer.android.com/design/ui/mobile/guides/foundations/accessibility) by Google.
- [Build Accessible Apps](https://developer.android.com/guide/topics/ui/accessibility) by Google.
- [Jetpack Compose Accessibility](https://developer.android.com/develop/ui/compose/accessibility) by Google.
- [Make Apps More Accessible](https://developer.android.com/guide/topics/ui/accessibility/apps) by Google.
- [Principles for Improving App Accessibility](https://developer.android.com/guide/topics/ui/accessibility/principles) by Google.

#### Video

- [Android Developers: Accessibility on YouTube](https://www.youtube.com/@AndroidDevelopers/search?query=accessibility) by Google, talks and how-tos on building accessible Android apps.

### Tools

- [Accessibility Insights for Android](https://accessibilityinsights.io/docs/android/overview/) by Microsoft.
- [Accessibility Scanner for Android](https://support.google.com/accessibility/android/answer/6376570) by Google.
- [Accessibility Test Framework for Android](https://github.com/google/Accessibility-Test-Framework-for-Android) by Google.
- [Espresso Accessibility Checks](https://developer.android.com/training/testing/espresso/accessibility-checking) by Google.

## Cross-Platform Frameworks {#cross-platform-frameworks}

### Learning

#### Text

- [.NET MAUI: Build Accessible Apps With Semantic Properties](https://learn.microsoft.com/en-us/dotnet/maui/fundamentals/accessibility) by Microsoft.
- [Accessibility in wxWidgets](https://wxwidgets.org/docs/tutorials/accessibility/) by wxWidgets.
- [Electron: Accessibility](https://www.electronjs.org/docs/latest/tutorial/accessibility) by Electron.
- [Flutter Accessibility](https://docs.flutter.dev/accessibility-and-localization/accessibility) by Flutter.
- [Qt Accessibility](https://doc.qt.io/qt-6/accessible.html) by Qt.
- [React Native Accessibility](https://reactnative.dev/docs/accessibility) by React Native.
- [wxAccessible Class Reference](https://docs.wxwidgets.org/latest/classwx_accessible.html) by wxWidgets.

#### Video

No video is curated specifically for these frameworks; the cross-cutting videos under [Auditing and Testing](#auditing-and-testing) apply.

### Tools

Each framework compiles to a native platform, so the platform-specific Tools above and the cross-cutting tools under [Auditing and Testing](#auditing-and-testing) apply.

## Editor and Browser Extensions {#editor-and-browser-extensions}

Extension and editor UIs are HTML, so the web references apply; these add host-specific guidance.

### Learning

#### Text

- [Accessibility Course](https://developer.chrome.com/docs/accessibility) by Google (Chrome for Developers), a structured web-accessibility course that also applies to extension UIs.
- [VS Code Accessibility Documentation](https://code.visualstudio.com/docs/editor/accessibility) by Microsoft.
- [VS Code Extension UX Guidelines](https://code.visualstudio.com/api/ux-guidelines/overview) by Microsoft.
- [VS Code Webview Guide](https://code.visualstudio.com/api/extension-guides/webview) by Microsoft.

#### Video

No video is curated specifically for extensions; the web videos under [Web Pages and Web Applications](#web-pages-and-web-applications) apply.

### Tools

Extension and editor UIs are HTML, so the Web Tools under [Web Pages and Web Applications](#web-pages-and-web-applications) apply, including the Axe Linter for Visual Studio Code.

## Command-Line Interfaces {#command-line-interfaces}

Guidance for the Command-Line Interface ([CLI](#cli)) applies across BASH, PowerShell, and Windows terminals.

### Learning

#### Text

- [Accessibility of Command Line Interfaces](https://dl.acm.org/doi/fullHtml/10.1145/3411764.3445544) by Google researchers (ACM).
- [Building a More Accessible GitHub CLI](https://github.blog/engineering/user-experience/building-a-more-accessible-github-cli/) by GitHub.
- [Command-Line Interface Handbook](https://www.patternfly.org/developer-resources/cli-handbook/) by PatternFly (Red Hat).
- [Using Git and the GitHub CLI With a Screen Reader](https://accessibility.github.com/documentation/guide/cli/) by GitHub.

#### Video

No video is curated specifically for command-line interfaces; the cross-cutting videos under [Auditing and Testing](#auditing-and-testing) apply.

### Tools

Terminal output is text, so a screen reader such as NVDA, under [Auditing and Testing](#auditing-and-testing), is the primary test tool.

## Voice and Conversational: Amazon Alexa {#voice-and-conversational-amazon-alexa}

### Learning

#### Text

- [Alexa Design Guide](https://developer.amazon.com/en-US/docs/alexa/design/design-your-skill.html) by Amazon, voice-first skill design with accessibility treated as a core tenet.
- [Alexa Skills for Everyone: How to Design an Inclusive Voice Experience](https://developer.amazon.com/en-US/blogs/alexa/alexa-skills-kit/2019/01/alexa-skills-for-everyone-how-to-design-an-inclusive-voice-experience) by Amazon.
- [APL (Alexa Presentation Language) Accessibility Guide](https://developer.amazon.com/en-US/docs/alexa/alexa-presentation-language/apl-accessibility-guide.html) by Amazon, on voice-enabling on-screen content for Echo Show and similar devices.

#### Video

No video is curated specifically for Alexa; the design and testing videos in the cross-cutting sections apply.

### Tools

Skills are tested in the Alexa Developer Console simulator and on Echo devices using their built-in screen reader.

## Design {#design}

Cross-cutting resources for the design phase, where interaction, visual, and content decisions either anticipate accessibility or build in barriers.

### Learning

#### Text

- \* [10 Usability Heuristics for User Interface Design](https://www.nngroup.com/articles/ten-usability-heuristics/) by Nielsen Norman Group. (11 min)
- [Chartability Heuristics for Accessible Data Experiences](https://chartability.fizz.studio/) by Fizz Studio. (8 min TOC)
- [Designing for Guidance (.pdf)](https://www.microsoft.com/design/assets/inclusive/InclusiveDesign_DesigningForGuidance.pdf) by Microsoft. (4 min), from the Microsoft Inclusive Design toolkit, on guiding users without relying on sight.
- [Do No Harm Guide: Centering Accessibility in Data Visualization](https://www.urban.org/research/publication/do-no-harm-guide-centering-accessibility-data-visualization) by Urban Institute. (4 min TOC)
- [Learn Accessibility with Figma](https://www.figma.com/resources/learn-design/inclusion/) by Figma. (8 min)
- [Survey Accessibility](https://www.qualtrics.com/support/survey-platform/survey-module/survey-tools/check-survey-accessibility/) by Qualtrics. (8 min), on designing and checking accessible survey forms.
- [Universal Design for Learning (UDL) Guidelines](https://udlguidelines.cast.org/) by CAST. (3 min)

#### Video

- [Accessible States in Design Systems](https://www.youtube.com/watch?v=k_7yqLyHc3U) by Russ Weakley. (44 min)

### Tools

Design relies on the contrast and color tools under [Web Pages and Web Applications](#web-pages-and-web-applications), such as the Colour Contrast Analyser and the WebAIM Contrast Checker.

## Content Authoring {#content-authoring}

Cross-cutting resources for producing accessible documents, media, and copy. Authoring tools themselves are addressed by the Authoring Tool Accessibility Guidelines ([ATAG](#atag)); the Accessibility Checker built into Microsoft Office, listed under Tools, is the most common in-app check.

### Learning

#### Text

- [Accessible Writing Guide](https://www.sigaccess.org/welcome-to-sigaccess/resources/accessible-writing-guide/) by SIGAccess. (10 min)
- [Add Alternative Text to a Shape, Picture, Chart, or Other Object](https://support.microsoft.com/en-us/office/add-alternative-text-to-a-shape-picture-chart-smartart-graphic-or-other-object-44989b2a-903c-4d9a-b742-6a75b451c669) by Microsoft. (7 min)
- \* [Alternative Text](https://webaim.org/techniques/alttext/) by WebAIM. (14 min)
- [Create Accessible PDFs from Microsoft Office](https://support.microsoft.com/en-us/office/create-accessible-pdfs-064625e0-56ea-4e16-ad71-3aa33bb4b7ed) by Microsoft. (3 min)
- [Create and Verify PDF Accessibility with Acrobat](https://helpx.adobe.com/acrobat/using/create-verify-pdf-accessibility.html) by Adobe. (27 min)
- [Disability Language Style Guide](https://ncdj.org/style-guide/) by National Center on Disability and Journalism. (84 min)
- [Federal Plain Language Guidelines](https://www.plainlanguage.gov/guidelines/) by U.S. Government. (2 min TOC)
- [Image Description Guidelines](http://diagramcenter.org/table-of-contents-2.html) by DIAGRAM Center. (5 min TOC)
- [Improving the Accessibility of Markdown](https://www.smashingmagazine.com/2021/09/improving-accessibility-of-markdown/) by Smashing Magazine. (19 min)
- [Make Your Outlook Email Accessible](https://support.microsoft.com/en-us/office/make-your-outlook-email-accessible-to-people-with-disabilities-71ce71f4-7b15-4b7a-a2e3-cf91721bbacb) by Microsoft. (10 min)
- [Rules for the Accessibility Checker](https://support.microsoft.com/en-us/office/rules-for-the-accessibility-checker-651e08f2-0fc3-4e10-aaca-74b4a67101c1) by Microsoft. (7 min)
- [UX Writing](https://www.nngroup.com/articles/ux-writing-study-guide/) by Nielsen Norman Group. (9 min)

#### Video

- [Accessibility Training for Microsoft Office](https://support.microsoft.com/en-us/office/accessibility-video-training-71572a1d-5656-4e01-8fce-53e35c3caaf4) by Microsoft. (1 - 3 min each in a series of 5)
- [Creating Accessible Content in Office 365](https://www.youtube.com/watch?v=Y7MktsGL8-Q) by Microsoft. (57 min)

### Tools

- [Accessibility Checker for Microsoft Office](https://support.microsoft.com/en-us/office/improve-accessibility-with-the-accessibility-checker-a16f6de0-2f39-4a2b-8bd8-5ad801426c7f) by Microsoft, built into Word, Excel, PowerPoint, and Outlook.
- [Accessible Templates for Office](https://support.microsoft.com/en-us/office/get-accessible-templates-for-office-ca086caa-2bd2-4ac8-8c12-4cd495bd4d76) by Microsoft.
- [Ace by DAISY](https://inclusivepublishing.org/toolbox/ace-by-daisy-app/) by the DAISY Consortium, an accessibility checker for EPUB files.
- [extCheck](https://github.com/JamalMazrui/extCheck) by Jamal Mazrui, a checker that audits local Word, Excel, PowerPoint, and Markdown documents against accessibility rules through COM automation.
- [GLOW Accessibility Toolkit](https://glow.bits-acb.org) by Jeff Bishop (Blind Information Technology Solutions), which audits, fixes, and templates Word, Excel, PowerPoint, Markdown, PDF, and ePub documents against the ACB Large Print Guidelines and WCAG 2.2 AA.

## Auditing and Testing {#auditing-and-testing}

Cross-cutting resources for evaluating accessibility. Developers test with screen readers that are free or built into the platform: NVDA on Windows (under Tools), VoiceOver on macOS and iOS, TalkBack on Android, and Narrator on Windows. Vendors document results in an Accessibility Conformance Report ([ACR](#acr)), commonly on the Voluntary Product Accessibility Template ([VPAT](#vpat)) form.

### Learning

#### Text

- [Accessibility Insights for Web (overview)](https://devblogs.microsoft.com/engineering-at-microsoft/accessibility-insights-for-web/) by Microsoft. (5 min)
- \* [Categorization and Comparison of Accessibility Testing Methods for Software Development](https://ebooks.iospress.nl/publication/50637) by the Norwegian Computing Center and OsloMet. (27 min)
- [Involving Users in Evaluating Web Accessibility](https://www.w3.org/WAI/test-evaluate/involving-users/) by W3C. (7 min)
- \* [Professional Web Accessibility Auditing Made Easy](https://pressbooks.library.torontomu.ca/pwaa/) by The Chang School, Toronto Metropolitan University. (238 min)
- [Testing for Accessibility on macOS](https://developer.apple.com/library/archive/documentation/Accessibility/Conceptual/AccessibilityMacOSX/OSXAXTestingApps.html) by Apple. (5 min)
- [Unified Accessibility Requirements for Web, Software, and Documents](https://www.ibm.com/able/requirements/requirements/) by IBM. (2 min TOC)
- [Using Narrator to Evaluate Web Accessibility](https://webaim.org/articles/narrator/) by WebAIM. (6 min)
- \* [Using NVDA to Evaluate Web Accessibility](https://webaim.org/articles/nvda/) by WebAIM. (7 min)
- [Using VoiceOver to Evaluate Web Accessibility](https://webaim.org/articles/voiceover/) by WebAIM. (8 min)
- [Verification through Manual Testing](https://www.ibm.com/able/toolkit/verify/manual/) by IBM. (3 min TOC), the manual-testing stage of the IBM Equal Access toolkit.
- [WCAG 2 Checklist](https://webaim.org/standards/wcag/checklist/) by WebAIM. (17 min)

#### Video

- [A11yTalks](https://www.youtube.com/c/accessibilitytalks) by A11yTalks. (28 - 60 min each in a series of 28)
- \* [Digital Accessibility Foundations](https://www.youtube.com/playlist?list=PLhDEeYUfW02RX4xw1pZPsspzT30_Zl8qq) by W3C. (1 - 4 min each in a series of 5)
- [Get Started with Assessment in Accessibility Insights for Web](https://www.youtube.com/watch?v=m1l7ghxOKF0) by Microsoft. (7 min)
- [Intro to Accessibility Insights](https://www.youtube.com/watch?v=UWlsZ-WUpVU) by Microsoft. (24 min)

### Tools

- [NVDA (NonVisual Desktop Access)](https://www.nvaccess.org/download/) by NV Access, the free, open-source Windows screen reader used for development testing; its [source repository](https://github.com/nvaccess/nvda/) is public.

## Communities and Further Lists {#communities-and-further-lists}

- [AppleVis](https://applevis.com/) by AppleVis.
- [Awesome Accessibility (brunopulis/awesome-a11y)](https://github.com/brunopulis/awesome-a11y), a community-maintained list that excludes overlay tools.
- [Awesome Web Accessibility (awesomelistsio)](https://github.com/awesomelistsio/awesome-web-accessibility), a community-maintained list focused on the web.
- [GNOME Accessibility Mailing Lists and Channels](https://wiki.gnome.org/Accessibility) by GNOME.
- [ICT Accessibility Testing Symposium](https://www.ictaccessibilitytesting.org/) by Chris Law.
- [Web Accessibility Email Discussion List](https://webaim.org/discussion/) by WebAIM.

## Glossary {#glossary}

Key terms used throughout this directory, in alphabetical order. Abbreviations link here from their first use.

- [**Accessibility (a11y)**]{#a11y} — The practice of designing software so that people with disabilities can use it on an equal basis with everyone else; "a11y" abbreviates the word (the letter a, eleven letters, the letter y).
- [**Accessibility API**]{#accessibility-api} — The platform service through which applications expose user-interface information to assistive technology; examples include UI Automation, the macOS and iOS accessibility APIs, and AT-SPI.
- [**Accessibility Conformance Report (ACR)**]{#acr} — A completed report, commonly on the VPAT form, in which a vendor documents how a product meets accessibility standards such as WCAG and Section 508.
- [**Accessibility tree**]{#accessibility-tree} — The structured representation of a user interface, derived from the running UI, that assistive technologies read; each node carries a name, a role, and often a value and a state.
- [**Accessible name**]{#accessible-name} — The label an assistive technology announces for a control, computed from markup or properties such as a visible label, an aria-label, or a content description.
- [**Alternative text (alt text)**]{#alt-text} — A short text description of an image that conveys its meaning to people who cannot see it; purely decorative images are instead hidden from assistive technology.
- [**API (Application Programming Interface)**]{#api} — A defined way for one piece of software to call another; an accessibility API lets applications expose interface details to assistive technology.
- [**ARIA (WAI-ARIA)**]{#aria} — A W3C set of roles, states, and properties for conveying the meaning and behavior of custom web widgets to assistive technology when native HTML semantics are not enough.
- [**Assistive technology (AT)**]{#at} — Software or hardware that helps a person with a disability use a computer, such as a screen reader, a screen magnifier, or a switch device.
- [**AT-SPI**]{#at-spi} — The Assistive Technology Service Provider Interface, the toolkit-neutral accessibility API used on Linux.
- [**ATAG**]{#atag} — The Authoring Tool Accessibility Guidelines, the W3C standard for making authoring tools both accessible to use and supportive of producing accessible content.
- [**Audio description**]{#audio-description} — A spoken narration track that describes important visual information in video for people who cannot see it.
- **Bookmarklet** — A small piece of JavaScript saved as a browser bookmark that performs a task, such as an accessibility check on the current page, when run.
- **Captions** — Synchronized on-screen text of speech and meaningful sound in video, for people who are deaf or hard of hearing.
- [**Command-Line Interface (CLI)**]{#cli} — A text-based interface in which the user types commands and reads textual output, as in a terminal or shell.
- **Conformance level** — WCAG's grading of success criteria as A, AA, or AAA; AA is the common legal and practical target.
- **Contrast ratio** — A measure of the difference in luminance between text and its background; WCAG sets minimum ratios so text stays legible for people with low vision.
- [**EN 301 549**]{#en-301-549} — The European standard for accessibility of information and communications technology, referenced by the European Accessibility Act, which incorporates WCAG.
- **Focus management** — Deliberately controlling which control holds keyboard focus, for example moving focus into a dialog when it opens and returning it to the trigger when it closes.
- **Keyboard trap** — A defect in which focus enters a component and cannot be moved out with the keyboard, blocking keyboard and screen-reader users.
- **Landmark** — A region of a page, such as main or navigation, that lets assistive-technology users understand the layout and jump between areas quickly.
- **Linter** — A tool that flags problems in source code as it is written or built; accessibility linters catch common markup and ARIA mistakes early.
- **Manual testing** — Human evaluation of accessibility, typically with the keyboard and a screen reader, needed for the many issues automated tools cannot detect.
- [**MSAA**]{#msaa} — Microsoft Active Accessibility, the legacy Windows accessibility API that preceded UI Automation.
- **Overlay (accessibility overlay)** — A third-party widget that claims to fix a site's accessibility automatically; widely regarded as ineffective.
- [**POUR**]{#pour} — The four WCAG principles: content should be perceivable, operable, understandable, and robust.
- **Role** — The type of a control as exposed to assistive technology, such as button, link, or checkbox.
- **Screen reader** — Assistive technology that conveys on-screen content as speech or braille; common ones are JAWS, NVDA, VoiceOver, TalkBack, and Narrator.
- [**Section 508**]{#section-508} — The United States law requiring federal information technology to be accessible; its Revised Standards incorporate WCAG.
- **Semantic HTML** — Using HTML elements for their intended meaning, such as button, nav, and heading elements, so that accessibility and structure come for free.
- **State** — A changeable condition of a control exposed to assistive technology, such as checked, expanded, or disabled.
- **Success criterion** — An individual, testable requirement within WCAG.
- [**UI Automation (UIA)**]{#uia} — The modern Windows accessibility framework that exposes user-interface elements to assistive technology and to test tools.
- [**VPAT (Voluntary Product Accessibility Template)**]{#vpat} — A standard form, published by the Information Technology Industry Council, used to produce an Accessibility Conformance Report for a product.
- [**W3C (World Wide Web Consortium)**]{#w3c} — The international standards body that develops web technologies and, through its Web Accessibility Initiative, the accessibility guidelines.
- [**WAI (Web Accessibility Initiative)**]{#wai} — The part of the W3C that produces accessibility guidelines, supporting technical material, curricula, and educational resources.
- [**WCAG**]{#wcag} — The Web Content Accessibility Guidelines, the W3C's widely adopted standard for digital accessibility.
