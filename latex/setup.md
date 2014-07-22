Ubuntu Setup
============

Install texmaker editor which can produce PDF previews.
```
sudo apt-get install texmaker
```

Install recommended fonts.
```
sudo apt-get install texlive-fonts-recommended
```

Optionally, install aditional fonts.
```
sudo apt-get install texlive-fonts-extra
```

Missing .sty files
------------------
If building the PDF fails due to missing .sty files, you may need to install another
more specialized package.  For example, when using the acmsiggraph template I found
lineno.sty was missing.  Find out what package has it as follows:
```
apt-cache search lineno
```

This returned:
```
texlive-humanities - TeX Live: Humanities packages
```

So install the package:
```
sudo apt-get install texlive-humanities
```
