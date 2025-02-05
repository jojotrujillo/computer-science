<!-- "'In that day I will restore the fallen house of David. I will repair its damaged walls. From the ruins
I will rebuild it and restore its former glory. And Israel will possess what is left of Edom and all the
nations I have called to be mine.' The Lord has spoken, and he will do these things." Amos 9:11-12 (NLT) -->

# statistics

Two major parts of statistics: descriptive statistics and statistical inference.
Descriptive statistics includes all of the definitions, concepts, and formulas required to create graphical
displays like frequency distributions, graphs, location of data, spread of data, and variability.

Statistical inference leverages probability and includes different methods used to achieve point estimation,
interval estimates, confidence intervals, and hypothesis tests.

Professor Leonard's video lectures on stats I used: [Statistics (Full Length Videos)](https://youtube.com/playlist?list=PL5102DFDC6790F3D0&si=Q4Ixn8DS6f9mt71Z)

Stats textbook I used: [Essentials of Modern Business Statistics with Microsoft Excel, Loose-leaf Version, 7th
Edition](https://www.amazon.com/Essentials-Business-Statistics-Microsoft-Loose-leaf/dp/1337298301)

I decided to use the R programming language to show mastery in this course since R is the de facto programming
language to use for programming statistics. I used the standalone version of R, outside of RStudio, because
I'm using Neovim as my editor of choice. More specifically, I'm using the 'rmarkdown' package out of R that
enables you to parse .Rmd files and mix in regular markdown syntax with R 'code chunks.' You can find more
info on R Markdown here: https://rmarkdown.rstudio.com/index.html.

Once you have `r` and `pandoc` installed into your distro via `apt`, open a terminal and run `R` to open a R
prompt.

Make sure you `cd` into the directory you need to that has your .Rmd files in it. Once inside the R prompt,
run `rmarkdown::render(<.Rmd file>)` to have it generate the parsed .md file along with any images you
might've included.

