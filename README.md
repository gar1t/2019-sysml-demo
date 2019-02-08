# Paper submission for SysML 2019

## Requirements

- latex
- letexmk
- xzdec (required by tlmgr)

Latex packages:

- subfigure

On Ubuntu:

``` shell
apt install -y \
  texlive-latex-base \
  texlive-latex-recommended \
  latexmk \
  xzdec
tlmgr init-usertree
tlmgr option repository ftp://tug.org/historic/systems/texlive/2017/tlnet-final
tlmgr install \
  subfigure
```
