# 🌸 言叶之栞----日本语歌词假名标注网页

**[简体中文](README.md) |English| [日本语](README_JA.md) |**


**Japanese Lyrics Kana Annotation and Formatting Tool**
### Extract lyrics with a single click using a 🎵NetEase Cloud Music🎵 URL
### Generate a 🛍️Word document with a single click
##
 **Kotoba no Shiori** is a single-file front-end web application designed specifically for Japanese music enthusiasts, Japanese language learners, and lyric translators.
The project supports automatic furigana annotation on kanji in Japanese lyrics, one-click extraction of lyrics from web URLs (NetEase Cloud Music), and one-click export of **Word (`.doc`)** files and standalone web documents with native furigana.


## ✨ Core Features

### 1. Ming typeface and bilingual typesetting system
### 2. Intelligent word segmentation and interactive phonetic annotation
### 3. 🔗 One-click lyric extraction from URLs
- **Multi-Source Web Parsing**: Supports directly pasting URLs from **Uta-Net (歌ネット)**, **Utaten**, **J-Lyric**, **NetEase Cloud Music**, and general Japanese lyrics websites to instantly retrieve song titles, artists, and lyrics.
- **Tag Restoration and Automatic Bilingual Separation**: Automatically converts the `<ruby>` tags embedded in web pages into editable `Kanji (Kana)` format, intelligently removes `.lrc` timeline tags (such as `[00:12.34] ) and composer/lyricist metadata, and automatically identifies “One Chinese a Day” alternating text, splitting it into two columns: the original Japanese lyrics and the Chinese translation.
### 4. Multi-Format Export and Responsive User Experience
- **One-Click Generation of Word Documents (`.doc`)**
- **HTML and Plain Text Export**
- **Mobile-optimized**

## 🚀 Quick Start

### Download and Run Locally (Zero Configuration)
This project uses a single-file, pure front-end HTML architecture, requiring no installation of `Node.js` or execution of bundling commands:

Simply visit `http://localhost:8080/mincho-lyrics.html` in your browser.

## 📖 User Guide

1. **Import or Enter Lyrics**
   - **Blank Customization (Default)**: Paste Japanese lyrics and Chinese translations directly into the input fields on the left; the system automatically aligns the two languages by line number. Click the `✕` button to the right of any input field to quickly clear its contents.
   - **URL Extraction**: Paste the URL of a lyrics webpage into the “🔗 Extract Lyrics from URL” field (or click the sample links “花の塔” or “夜に駆ける” in the top-right corner of the field), then click **⚡ Extract Lyrics** to automatically populate the content.
   - **Pre-set Song Experience**: Click the `🎵 夜に駆ける` or `🌺 花の塔` capsule at the top of the workspace to load a complete bilingual formatting example with a single click.

2. **Customizing Special Pronunciations (Ateji)**
   - **Inline Syntax Annotation**: Enter `未来(あした)` in the Japanese lyrics box or click the shortcut label at the bottom of the input box; the preview area will immediately render the specified pronunciation.
   - **Stage Click Correction**: Directly click any kanji with phonetic annotations on the preview stage on the right, enter the new pronunciation in the pop-up window, and select either “Apply to all instances of this term” or “Apply only to this line.” Click **Apply Phonetic Annotations** to apply the changes in real time.

3. **Customize Ming-style Layout and Colors**
   - In the 2×4 layout workspace at the top, adjust the **Japanese font**, **translation font**, **font size**, **character spacing**, **line height and font weight**, and **pronunciation annotation scale**.
   - Click the circular color dots under “Free Color Selection” to choose any RGB/HEX color for the Japanese text, phonetic annotations, and translation, or use the drop-down menu on the right to switch between 5 anime-style color palettes with a single click.

4. **Export Your Work**
   - Click **One-Click Word Generation** in the top-right corner of the navigation bar to download a `.doc` document, or use the **Copy HTML**, **Copy Text**, and **Export Webpage** buttons in the top bar of the preview pane to share your layout.

Translated with DeepL.com (free version)
