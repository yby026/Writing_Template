# Writing template with Quarto as a management system

*[中文说明](https://github.com/yby026/Writing_Template/blob/main/README_ch.md)*

**[Quarto](https://quarto.org/docs/get-started/) is needed for using this template. This template is built entirely with VS Code**

* Extra packages and customised environment are not necessary, but it's always a good practice to do so.
* To enable GitHub for version control, a Git installation and Git related extension are needed; the executables will need to be added to **Path** under **Environmental Variables**, and reload the VS Code terminal

**Markdown is used as the editor, which can be controlled by the Markdown syntax and rules**

## Usage
* Download and install Quarto following the instructions first
* Download or Pull the repository from GitHub to the working directory
* Open with VS Code, .qmd files are markdown files for Quarto, and the article documents will also be in this file type
*It's recommended to use the Quarto extension*

## Citation 
* To insert in-text citation, add the **key** for citation following **@**, something like: @Smith2020
* To avoid manual typing citation (both in-text citation or reference list), it can be achieved with several Zotero extensions available from VS Code Extension Marketplace
* All Zotero extensions are dependent on the **Better BibTeX** plugin installed on Zotero, and mostly need Zotero and Better BibTeX running while using


## Format document structure
* Settings can be customised, including: types of the project, names of the authors, chapters to render (documents that can be formatted or converted to other formats), format details, etc.
* Global settings can be changed from **_quarto.yml**
* Specific settings can be applied to each document by adding format information at the beginning of the document (see [Example.qmd](https://github.com/yby026/Writing_Template/blob/main/Example_chapters/Example.qmd))


## Rendering
* Most rendering can be done using **quarto render**
* Rendering from .docx to Markdown is achieved by using **pandoc**
