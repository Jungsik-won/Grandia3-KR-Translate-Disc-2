# Grandia3-KR-Translate-Disc-2<div align="center">

<img src="https://raw.githubusercontent.com/Jungsik-won/Grandia3-KR-Translate-Disc-1/main/docs/assets/grandia3-korean-banner.svg" alt="Grandia III Korean Translation Project" width="860">

# Grandia III 한국어 패치 — Disc 2

**PlayStation 2 일본판 『그란디아 III』 비공식 한국어화 프로젝트**

[![Latest Release](https://img.shields.io/github/v/release/Jungsik-won/Grandia3-KR-Translate-Disc-2?display_name=tag&label=Latest%20Release&color=6f42c1)](https://github.com/Jungsik-won/Grandia3-KR-Translate-Disc-2/releases)
[![Disc 2](https://img.shields.io/badge/Target-Disc%202-2ea44f)](https://github.com/Jungsik-won/Grandia3-KR-Translate-Disc-2/releases/tag/disc2-20260914)
[![Download Xdelta](https://img.shields.io/badge/Download-Xdelta%20Patch-0969da)](https://github.com/Jungsik-won/Grandia3-KR-Translate-Disc-2/releases/download/disc2-20260914/Grandia3_KR_Disc2_20260914.xdelta)

</div>

> Disc 2의 시스템·아이템·전투·시나리오·비행·동영상 이벤트를 한국어로 즐길 수 있도록 다듬는 팬 번역 프로젝트입니다.

## 언어 선택

[🇰🇷 한국어](#한국어) · [🇺🇸 English](#english) · [🇯🇵 日本語](#日本語)

---

## 🇰🇷 한국어

### 프로젝트 소개

이 저장소는 **Grandia III 일본판 Disc 2**를 대상으로 하는 비공식 한국어 패치의 배포 공간입니다. 게임 원본을 배포하지 않고, 합법적으로 보유한 원본 ISO에 적용하는 차분 패치와 검증 자료만 제공합니다.

Disc 1 패치와 분리해 관리하므로, Disc 2를 패치할 때는 반드시 Disc 2용 원본 ISO와 이 저장소의 패치를 사용하세요.

### 최신 배포판

| 항목 | 내용 |
| --- | --- |
| 릴리스 | [disc2-20260914](https://github.com/Jungsik-won/Grandia3-KR-Translate-Disc-2/releases/tag/disc2-20260914) |
| 패치 파일 | `Grandia3_KR_Disc2_20260914.xdelta` |
| 패치 크기 | 1,930,316,788 bytes |
| 원본 | `Grandia III (Japan) (Disc 2).iso` |
| 원본 크기 | 4,449,107,968 bytes |
| 원본 SHA-256 | `68d2eb9dc03288c91fcd943c437390f41b10ecff7f61558665695dc5140a057d` |
| 결과 ISO SHA-256 | `e8565a7b35a939c9a0be653dc4c71fecaede95ee05bd29e98a5b75eba77a5cd8` |

### 다운로드

<div align="center">

### [⬇️ Disc 2 Xdelta 패치 다운로드](https://github.com/Jungsik-won/Grandia3-KR-Translate-Disc-2/releases/download/disc2-20260914/Grandia3_KR_Disc2_20260914.xdelta)

[릴리스 페이지에서 README·체크섬·매니페스트 받기](https://github.com/Jungsik-won/Grandia3-KR-Translate-Disc-2/releases/tag/disc2-20260914)

</div>

릴리스에는 다음 파일만 포함됩니다.

- Xdelta 차분 패치
- `README_KO.md` 적용 안내서
- `SHA256SUMS.txt` 체크섬
- `release-manifest.json` 배포 매니페스트

원본 ISO, 패치 완료 ISO, MOV·MDZ·MDT·BIN 및 추출 게임 데이터는 배포하지 않습니다.

### 적용 방법

1. 위 릴리스에서 Xdelta 패치와 안내 파일을 받습니다.
2. 아래 SHA-256과 일치하는 일본판 Disc 2 원본 ISO를 준비합니다.
3. `xdelta3`가 설치된 폴더에서 다음 명령을 실행합니다.

<pre><code>xdelta3 -d -s "Grandia III (Japan) (Disc 2).iso" "Grandia3_KR_Disc2_20260914.xdelta" "Grandia3_KR_Disc2_Final_20260914.iso"</code></pre>

생성된 결과 ISO의 SHA-256은 다음과 같아야 합니다.

<code>e8565a7b35a939c9a0be653dc4c71fecaede95ee05bd29e98a5b75eba77a5cd8</code>

### 왜 5GB 이상의 여유 공간이 필요한가요?

패치 적용 후 ISO가 5GB 이상으로 커지는 것은 아닙니다. 결과 ISO는 원본과 거의 같은 **4,449,394,688 bytes**입니다. 다만 작업 중에는 원본 ISO, 약 1.93GB 패치, 새로 생성되는 결과 ISO와 임시 파일이 함께 필요할 수 있으므로 **최소 5GB 이상, 가능하면 10GB 이상의 여유 공간**을 권장합니다. FAT32 저장 장치는 4GB 제한 때문에 결과 ISO를 저장할 수 없습니다.

### 반영 범위

- Disc 2 한국어화 최종 교체 항목 379개 재병합
- 아이템 알림·공용 폰트·비행 선택지 및 전환 데이터 수정
- GRM51~GRM69 동영상 자막과 GRM56 수정 반영
- 90개 음성 이벤트와 997개 논리 자막 큐를 사용하는 외부 자막 렌더러
- ISO9660/UDF 파일 주소·크기 정합성 검증

### 검증 상태

- 379개 교체 파일 역추출 및 해시 검증 통과
- 원본 파일 1,265개 전체 payload 대조 통과
- 원본 파일 전체 ISO9660/UDF 주소·크기 대조 통과
- Xdelta 적용 결과와 최종 ISO의 바이트 단위 일치 확인
- 일부 비행 전환·이벤트 자막·GRM56 재생은 사용자 PCSX2 실기 확인이 남아 있습니다.

### 주의사항

- 반드시 정확한 일본판 Disc 2 원본 ISO에만 적용하세요.
- 다른 지역판·다른 리비전·이미 수정된 ISO에는 적용하지 마세요.
- 원본 ISO는 별도로 보존하고, 처음 실행할 때는 PCSX2를 완전히 종료한 뒤 새 ISO로 cold boot하세요.
- 게임명·로고·캐릭터·게임 데이터의 권리는 각 권리자에게 있으며, 이 프로젝트는 비공식·비상업적 팬 번역 프로젝트입니다.

---

## 🇺🇸 English

This repository distributes an unofficial Korean fan translation patch for the Japanese PlayStation 2 release of **Grandia III — Disc 2**. It provides an Xdelta difference patch and verification documents only; no original or patched ISO and no extracted game assets are distributed.

Download the latest [Disc 2 release](https://github.com/Jungsik-won/Grandia3-KR-Translate-Disc-2/releases/tag/disc2-20260914). Use only the matching Japanese Disc 2 source ISO and verify the SHA-256 values listed above. The output ISO remains approximately the same size as the source; extra free space is needed because the source, patch, output, and temporary files may coexist during patching.

---

## 🇯🇵 日本語

このリポジトリは、PlayStation 2版『グランディアIII』日本版 **Disc 2** を対象とした非公式韓国語ファン翻訳パッチを配布します。配布物はXdelta差分パッチと検証資料のみで、元ISO・パッチ済みISO・抽出ゲーム素材は含みません。

最新版は [Disc 2 リリース](https://github.com/Jungsik-won/Grandia3-KR-Translate-Disc-2/releases/tag/disc2-20260914) からダウンロードしてください。記載されたSHA-256と一致する日本版Disc 2の元ISOだけを使用し、適用前に元ISOをバックアップしてください。

---

<div align="center">

[⬅️ Disc 1 Repository](https://github.com/Jungsik-won/Grandia3-KR-Translate-Disc-1) · [📦 Disc 2 Releases](https://github.com/Jungsik-won/Grandia3-KR-Translate-Disc-2/releases) · [🐛 Issues](https://github.com/Jungsik-won/Grandia3-KR-Translate-Disc-2/issues)

**Grandia III Korean Translation Project**

</div>
