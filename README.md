# UOK-LaTeX-Thesis

A XeLaTeX template for writing theses according to the official style guidelines of the University of Kurdistan (UOK).

## Repository Structure

This template is organized into several directories and files as follows:

### 📁 Folders

* **Bibs**
  Contains `resources.bib`, which stores all citation entries used throughout the thesis.

* **Chapters**
  Includes the main content of your thesis, such as:

  * `Introduction.tex`
  * `RelatedWork.tex`
  * `ProposedMethod.tex`
  * `Experimental.tex`
  * `Conclusion.tex`

  You can add additional chapters (e.g., a pre-introduction) by creating a new `.tex` file here and including it in your main file using:

  ```latex
  \include{chapters/pre-intro}
  ```

* **Figures**
  Store all your image files here. Subfolders are supported. To include a figure in your document, use:

  ```latex
  \mysubfig{figures/your-file.pdf}{Your image caption}
  ```

* **STR-Files**
  Contains structured template files for front matter and official pages:

  * `abstract-en.tex`: Abstract in English
  * `abstract-fa.tex`: Abstract in Persian
  * `acknowledgements.tex`
  * `submission-en.tex`: Score and signatures page (English)
  * `submission-fa.tex`: Score and signatures page (Persian)
  * `evaluation.tex`: Undertaking page
  * `TASVIR-en.tex`: English cover page with green background
  * `TASVIR-fa.tex`: Persian cover page with green background

  ⚠️ Most users won't need to edit the TASVIR files.

### 📄 Main LaTeX Files

* **Mohammad.tex**
  The primary file to compile. Update this file to include your chapters and structure the thesis.

* **preamble.tex**
  Loads all required packages and configurations. You typically don't need to modify this.

* **glossaries.tex**
  Add your glossary terms here if your thesis includes a list of abbreviations or definitions.
