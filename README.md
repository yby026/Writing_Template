# Writing template with Quarto as management system

**本模板使用Quarto作为管理系统， 需要安装[Quarto](https://quarto.org/docs/get-started/)，之后可以在VS Code, R Studio, 或者Jupyter上使用。本模板时完全建立在VS Code之上的**

* 推荐使用Conda来进行环境管理
* 如需使用GitHub进行版本控制，则需要额外安装Git和GitHub插件，并将相关文件添加至**环境变量** > **Path**中 （推荐安装的时候直接选添加到Path）
* 同理，如果VS code terminal说找不到命令，则需要将相关文件添加至**环境变量** > **Path**中

**本模板使用Markdown，语法和符号和Jupyter Notebook这种基于Markdown的IDE相同**

## 常用Markdown符号
标题分级用#，## 或者###，一级标题用#，二级标题用##，三级标题用###，依次类推 （#后面要加空格）
斜体用*斜体*，粗体用**粗体**，斜粗体用 ***斜粗体***，删除线用~~删除线~~。
bullet list用*，+ 或者-开头，后面加空格

如果要加代码块， 用三个反引号包裹起来：
```python
print("Hello, World!")
```
如果要加行内代码， 用一个反引号包裹起来：`print("Hello, World!")`

如果要加链接， 用方括号包裹链接文本，后面跟上圆括号包裹链接地址：[链接文本](https://example.com)

如果要加citations， 用@后面跟上引用的key，例如：@Smith2020，用插件Zetero Cite可以自动生成引用，可以自己添加快捷键，但必须要有zetero和better-bibtex插件

## 快捷键列表：
* ctrl+shift+P 打开命令面板
* ctrl+shift+C 打开代码块
* ctrl+. 直接打开拼写检查


## 文章结构设置和format
从_quarto.yml里面设置全局

每篇文章（每个.qmd文件）都可以有自己的设置

## 插件
* python
* LTeX+ 拼写检查
* Zotero Cite 引用管理
* Quarto
* 别的按需添加


## 其他
Notes_some_simple_lines.md 里有我添加的一点quarto和pandoc代码行笔记