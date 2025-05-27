# UOK-LaTeX-Thesis

A XeLaTeX-based thesis prepared according to the official formatting guidelines of the University of Kurdistan (UOK). This repository provides a complete and approved sample thesis that other students can reference to structure and format their own work correctly.

---

## 📁 LaTeX File Structure

This project is organized into several folders and key files as follows:

---

### 📁 **Bibs**

Contains the bibliography file:

* `Ref.bib`: Stores all your citation entries. Add your references here using BibTeX format.

---

### 📁 **Chapters**

Includes the main body content of your thesis, organized by topic:

* `Introduction.tex`
* `RelatedWork.tex`
* `ProposedMethod.tex`
* `Experimental.tex`
* `Conclusion.tex`

➤ You should place your thesis content into the appropriate file. For example, write your introduction in `Introduction.tex`, your methodology in `ProposedMethod.tex`, and so on.

➤ To add additional chapters (e.g., a pre-introduction), create a new `.tex` file in this folder and include it in the main file using:

```latex
\include{chapters/pre-intro}
```

---

### 📁 **Figures**

Place all your figures and images here. Subfolders are supported.

➤ To include an image in your document, use the following command:

```latex
\mysubfig{figures/Subfolder/your-figure.pdf}{Your image caption}
```

---

### 📁 **STR-Files**

Contains structured front matter and official university pages:

* `abstract-en.tex`: Write your abstract in English.
* `abstract-fa.tex`: Write your abstract in Persian.
* `acknowledgements.tex`: A page to thank those who supported you during the thesis.
* `submission-en.tex`: Fill in the English score and signature page.
* `submission-fa.tex`: Fill in the Persian score and signature page.
* `evaluation.tex`: Undertaking/commitment declaration.
* `TASVIR-en.tex`: Insert the English cover page with the green background.
* `TASVIR-fa.tex`: Insert the Persian cover page with the green background.

⚠️ *Most users won't need to modify the TASVIR files unless required for submission or printing.*

---

## 📄 Main LaTeX Files

* **`Mohammad.tex`**
  The main file to compile the full thesis. Use this to include all chapters and structure your document.

* **`preamble.tex`**
  Loads all necessary packages, commands, and global configurations. Typically does not require editing.

* **`glossaries.tex`**
  Add glossary terms, abbreviations, or technical definitions here.

---

## 📦 Compilation Notes

➤ Recommended to compile using **XeLaTeX** for best font and language support (especially for Persian/Unicode text).
You can compile via TeX editors like **TeXstudio**, **Overleaf**, or the command line.

---

🙏 **If you found this thesis example helpful, please consider giving the repository a ⭐ to support the project.**
