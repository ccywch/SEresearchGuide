# The guide of paper writing in Latex

This document record my experience in writing a paper with LaTex. So if you'd like to collaborate with me in writing some research papers, please have a look at this guide.

## Overall:
- Use the latex template downloaded from the official sites of the conference or journal.
- Please write each sentence in one row so that readers (actually I) can easily understand.
- Please separate each section as a file, and add them into the main file.
- For each section, figure, table, please attach a label to it with the command `\label{}`. Please name it with semantically e.g., `\label{sec:introduction}`, `\label{fig:comparisonResult}`, `\label{tab:goodExample}`. When referring the `figure/table/section` in the main text, please use `\ref` command e.g., `Fig. \ref{fig: comparisonResult}`. Note that please come up with a **semantic/meaningful** name for the label.
- If multiple users are working on the latex, please make everyone write text in different colors. You can define a macro in the main file like \newcommand{\chunyang}[1]{\textcolor{blue}{\textbf{Chunyang}:#1}}. 
- Please put all your references into a file (e.g., called `refercen.bib`), and import it using the latex command. Note that all bibtex can be copied-pasted from Google Scholar.
![bibtex](googleScholar.png)
- Do not add URL in the main text, but put your URL with command `\url{}` in the footnote.
- When the overall draft is done, please try to adjust the figure/table position to make it align with the corresponding text.



## Figures
- When showing results in the figure, please make the font size of the axis labels large enough so that reader can understand it.
- Please store your figure in pdf format as pdf figure is a vector figure. It will not collapse when zooming in.
- Please put all figure files into one folder and refer to it in the latex with relative path, e.g., `\includegraphics[width=1.0\textwidth]{figures/autoencoder.pdf}`


## Table
- When using the table to show examples, especially with many rows, please color alternative rows in [white and gray](https://tex.stackexchange.com/questions/5365) with command `\rowcolors{2}{gray!25}{white}` to color every alternate table row. 
- When we want to save space, you can use `\vspace{-2mm}` between the caption and the table, or between the caption and the main text.
- If there are too many rows within the table, you can use command `\rowcolors{2}{gray!25}{white}` to color every alternate table row.
- `\setlength{\tabcolsep}{0.7em}` can be used to squeeze the padding space between columns.


## Macro
- When there are multiple collaborators for paper writing, please use the macro command to highlight different color for each user like `\newcommand{\chen}[1]{\textcolor{red}{\textbf{Chen}: #1}}`.
- If you have a tool to mention within the whole paper, you can give it a name with a macro like `\newcommand{\tool}{{\texttt{TOOL}}\xspace}`.


## Metainfo
Before paper submission (not camera-ready), you may need to remove the meta-info (e.g., copyright) to save space. For example, you can remove the copyright info in ACM template with command lines: 
```
\setcopyright{none}
\settopmatter{printacmref=false} % Removes citation information below abstract
\renewcommand\footnotetextcopyrightpermission[1]{} % removes footnote with conference information in first column
```


## Contact
More examples can be seen at my [slides](FIT4003-paperDiscussion_short.pdf).
I will keep maintaining this guideline list, and feel free to clone or submit new suggestions to it. If you have further questions, please create an issue or drop me an email wchccy@gmail.com.
