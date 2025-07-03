# PowerShell command to convert a Word document to Markdown with media extraction
pandoc "input/chapter1.docx" `
>>   -f docx -t markdown_strict `
>>   --extract-media="chapter1/media" `
>>   -o "output/chapter1.md"
# change .md to .qmd if needed

# render markdown file to latex
quarto render chapter1\chapter1.qmd --to latex

# render markdown to docx
 * quarto can't specify a path when it comes to "path", so to bypass this have to use "*cd*" point to the directory first 
 * cd "target_directory\" quarto render chapter1.qmd --to docx --output chapter1.docx

# render latex to docx
pandoc _book\book-latex\chapters.tex -o chap1.docx