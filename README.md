
# 德语词卡网页 (Vokabel-Web)

一个基于浏览器的德语单词学习网页，支持翻转卡片、复习计划、导入导出词库等功能。  
网页使用 **HTML + CSS + JavaScript** 编写，可直接在 GitHub Pages 上运行。

---

## 📘 词汇来源
本项目中的单词主要来自以下教材：

> 《当代大学德语（学生用书）第1册》，外语教学与研究出版社提供的 PDF 版本。

所有词汇均由我手动从教材中整理为 CSV/JSON 格式，仅用于个人学习与交流目的。  
若涉及版权问题，请联系我删除相关内容。

---

## 💡 功能介绍

### 📂 导入与管理
- 支持导入 CSV 或 JSON 文件（表头为 `de,zh,example,image,hint`）。
- 点击 **导入Deck** 可上传现有的单词表。
- 点击 **导出Deck** 可保存当前的单词和学习进度为 `.json` 文件。
- **批量编辑** 功能可以直接粘贴 CSV/JSON 文本进行导入（目前功能简单，后续可能优化）。
- **清空单词** 会删除本地保存的所有词汇和进度数据（localStorage）。

### 🧠 学习与复习
- 点击或按 **Space** 键可翻转卡片。
- 按 **F** 或点击“熟悉”记录为已掌握。
- 按 **J** 或点击“不熟悉”记录为需复习。
- 卡片下方会显示“下次复习时间”，根据简单的间隔重复算法自动计算。
- “只看到期”选项目前无明显作用，未来版本可能优化或移除。

### 🔢 显示与统计
- 页面顶部会显示当前总单词数、到期单词数及当前索引。
- 支持课次筛选（如 Lektion 1, 2...）。
- 左右方向键（← / →）切换卡片。
- 页面下方按钮也可实现翻页操作。

---

## ⚙️ 技术说明
- 数据保存在浏览器的 `localStorage` 中，不需要服务器。
- 复习算法基于简化的 SM-2 模型（Anki 同类算法的简易版）。
- 可朗读德语单词与例句（使用 Web Speech API）。

---

## ⚠️ 说明
- 当前版本的“复习计划”算法与“只看到期”功能尚未完善。
- 批量编辑器导入功能部分浏览器可能无响应，建议通过“导入Deck”上传。
- “熟悉/不熟悉”按钮目前不会隐藏卡片，仅记录时间数据（后续可优化）。

---

## 🌐 访问网页
你可以直接访问：

👉 [https://yooyii.github.io/vokabel-web/](https://yooyii.github.io/vokabel-web/)

---

## 🗣 English Version

### Overview
This is a German vocabulary learning web app built with HTML, TailwindCSS, and JavaScript.  
It supports flip cards, spaced repetition (localStorage-based), CSV/JSON import & export, and progress tracking.

### Vocabulary Source
The words come from:
> *Contemporary College German – Textbook Vol. 1* (Foreign Language Teaching and Research Press).

All vocabulary data were manually extracted for **educational use only**.  
If any copyright concerns arise, I will remove the material immediately.

### Main Features
- **Import/Export Decks**: Upload `.csv` or `.json` files or export your current deck.
- **Flip Cards**: Front = German, Back = Chinese + Example Sentence.
- **Keyboard Shortcuts**:  
  - `Space` = Flip,  
  - `F` = Mark as familiar,  
  - `J` = Mark as unfamiliar,  
  - `← / →` = Switch card.
- **Statistics & Filters**: View total count, due count, lesson filter.
- **Local Storage**: Progress and deck are saved locally in your browser.

---

## ⚠ Notes
- The spaced-repetition system is a simplified SM-2 model and still experimental.
- “Show only due” currently has limited functionality.
- “Bulk Edit” allows manual import but may not respond in all browsers.

---

## 🌍 Deutsche Version

### Überblick
Dies ist eine browserbasierte Lernseite für deutschen Wortschatz, entwickelt mit HTML, TailwindCSS und JavaScript.  
Sie unterstützt Karteikarten, Wiederholungspläne und das Importieren/Exportieren von Wortlisten (CSV/JSON).

### Wortquelle
Die Vokabeln stammen aus:
> *当代大学德语（学生用书）Band 1*, herausgegeben vom FLTRP.

Alle Daten wurden manuell für Lernzwecke extrahiert.  
Bei Urheberrechtsbedenken werden die Inhalte auf Anfrage entfernt.

### Hauptfunktionen
- **Import/Export**: CSV oder JSON-Dateien hochladen oder exportieren.  
- **Karteikarten**: Vorderseite = Deutsch, Rückseite = Chinesisch + Beispielsatz.  
- **Tastenkürzel**:  
  - `Leertaste` = umdrehen  
  - `F` = vertraut  
  - `J` = nicht vertraut  
  - `← / →` = Karte wechseln  
- **Statistiken**: Gesamtzahl, fällige Karten, Lektionenfilter.  
- **Lokale Speicherung**: Fortschritt wird im Browser gespeichert.

---

📧 *Für Rückfragen oder Hinweise zu Urheberrecht: bitte kontaktieren Sie mich direkt über GitHub.*
