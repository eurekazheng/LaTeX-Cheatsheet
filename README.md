# LaTeX Cheatsheet

- Don't hesitate to read all sentences \& code of this doc. It answers most of the puzzles.
- $\LaTeX{}$ is a good regularization scheme to write academic works compared to MS Word and the de facto standard in academia. However, typesetting in $\LaTeX{}$ is also terribly unrobust, highly mysterious, stubbornly unreasonable, confusing, counter-intuitive, complicated, hard-to-memorize, buggy yet undebuggable, packages-dependent, restrictive, and involves many obsolete programming fashions.
- Therefore, this cheat sheet serves as a collection of common snippets in a common article (for a book you may need extra features such as indices \& glossaries etc.) and it would be a terrible typesetting experience if you don't have something similar in hand. It tries to support both aesthetics from designers' perspective and workflow conveniences from engineers' perspective while being as least hacky as possible. Most of them are self-explanatory for basic users.
- However, it's still far from capturing all the subtleties of $\LaTeX{}$, e.g. hyperlinks. It will be frequently updated after I discovered more in everyday usages. To explore more of $\LaTeX{}$, I recommend the following resources:
  - Documentation of packages: [CTAN](https://ctan.org/)
  - Topics-organized tutorials: [Overleaf](https://www.overleaf.com/learn)
  - General docs: [$\LaTeX{}e$ unofficial reference manual](https://latexref.xyz/)
- Note that some of the usage (such as the geometry package) are only in the preamble. Please refer to the code with comments.
- I recommend using $Lua\LaTeX{}$ + $\TeX{}$ Live + $\TeX{}$ Studio (Windows), $\TeX$ Pad (macOS), or Overleaf (for collab). 
  - You might think that a more lightweight bundle such as [$Tiny\TeX{}$](https://yihui.org/tinytex/) is preferrable, but you end up having to install packages every time you use a new template. 
  - Compared to popular versatile editor such as Visual Studio Code or IDEs, $\TeX{}$ Studio, though ugly in interface, is dedicated to $\TeX{}$ and contains many shortcuts.
  - $Lua\LaTeX$ is the newest $\TeX{}$ engine. It provides a new programming framework which some new features require.
- When a .sty file is missing (especially if you're using $Tiny\TeX{}$), use `tlmgr search --global --file XX.sty` to find the package name. Then, use `tlmgr install YY.sty` (though YY is usually the same with XX). 对于国内用户，请换用清华源：`tlmgr option repository https://mirrors.tuna.tsinghua.edu.cn/CTAN/systems/texlive/tlnet`