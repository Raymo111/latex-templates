# LaTeX formatting for STEM Schoolwork
Overleaf settings:
- Compiler: PDFLatex
- TeX Live version: 2019 (latest)
- Spell check: English (use whatever lang you want)
- Auto-complete: On
- Auto-close Brackets: On
- Code check: On
- Editor theme: monokai (it's the best)
- Overall theme: Default (eww to light mode, I wish there was a black mode)
- Keybindings: None (I'm a vim user but I don't like it in Overleaf)
- Font Size: 14px (I have a massive monitor)
- Font Family: Monaco/Menlo/Consolas
- Line Height: Compact
- PDF Viewer: Built-In
- Recompile:
    - Auto-recompile: On
    - Compile Mode: Normal (I'm scared of using draft and there's not much latency reduction for my usage)
    - Check Syntax: On

Texlive packages required: mathtools xcolor enumitem ncctools pgf forest

Additional packages required for minted (code with syntax highlighting in latex): minted fvextra fancyvrb upquote lineno catchfile xstring framed float

Additional config for minted for Sharelatex (Overleaf Community Edition):
```bash
alias sharelatex='/path/to/overleaf/bin/docker-compose exec sharelatex'
sharelatex apt update
sharelatex apt inst python-pygments
sharelatex sed -ie '$ashell_escape = t' /usr/local/texlive/2021/texmf.cnf
```
