# PowerShell command to convert a Word document to Markdown with media extraction
pandoc "C:\Users\fcy5609\OneDrive - AUT University\Thesis\Chapter1 - commentary on deep learning\challenges in deep learning in forest ecology.docx" `
>>   -f docx -t markdown_strict `
>>   --extract-media="chapter1/media" `
>>   -o "C:\Users\fcy5609\OneDrive - AUT University\Thesis\Chapter1 - commentary on deep learning/chapter1.md"
# change .md to .qmd if needed

# render the markdown file to latex
quarto render chapter1\chapter1.qmd --to latex

# render latex to docx
pandoc _book\book-latex\Beech-Thesis.tex -o chap1.docx