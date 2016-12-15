# Computer Science College Resume Template

This is a LuaLaTeX resume template catered specifically to college students in Computer Science, although it can be adapted to any major or non-students.

## Getting Started

### Using TeX

Download a TeX distribution from the table below:

| Windows | Mac | *nix |
| ------------------------------------------------------------------------------- |:-------------:|:-------------:|
| [TeX Live](http://mirror.ctan.org/systems/texlive/tlnet/install-tl-windows.exe) | [MacTex](http://tug.org/cgi-bin/mactex-download/MacTeX.pkg) | [TeX Live](http://mirror.ctan.org/systems/texlive/tlnet/install-tl-unx.tar.gz) |

TeX is very modular, and depending on the distribution you download, you may or may not have all of the packages needed to typeset the template. TeX Live Utility is a great package manager for Mac. For other systems, you may need to use the command line to install new packages.

It is important to typeset this template using LuaLaTeX rather than LaTeX, XeTeX, etc.

### Template Usage

To use the template, begin a new TeX document and paste the contents of Resume.tex into your TeX document. Set the typesetting to LuaLaTeX and hit typeset.

When in doubt, look for the raw text within the TeX document of the text you are trying to change in the PDF. Changing this text will typically change what you want within the PDF.

#### Heading

To change the heading, look for the following block of code within the document:
```latex
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
%%%%%      HEADING      %%%%%
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
```

Directly below this, you can change the 7 values associated with the heading.

#### Leadership/Education/Work Experience

An experience block, which includes bullet points, is of the form:

```latex
\begin{itemize}
\item[]
	\ressubheading{Name of Organization}{City, State}{Position, Degree, etc.}{Start Date - End Date}
	\begin{itemize}
		\resitem{Item 1}
		\resitem{Item 2}
    \resitem{Item 3}
	\end{itemize}
\end{itemize}
```

#### Projects

A project block, which includes bullet points, is of the form:

```latex
\begin{itemize}
\item[]
	\project{Project Name}{\textbf{GitHub Link or Date}}
	\begin{itemize}
		\projitem{Item 1}
		\projitem{Item 2}
	\end{itemize}
\end{itemize}
```

#### Software Skills

The software skills section is relatively straightforward, and the block shouldn't change much:

```latex
\begin{changemargin}{0cm}{0.475cm}
\begin{itemize}
\item[]
	\textbf{Languages and Software}: List of programming languages
	\vspace{-1mm}

\item[]
	\textbf{IDEs and Frameworks}: List of IDEs, Frameworks, Databases, etc.
	\vspace{-1mm}
	
\item[]
	\textbf{Operating Systems}: List of Operating Systems
	\vspace{-1mm}
	
\end{itemize}
\end{changemargin}
```

#### Activities

An activities block is simple and of the form:

```latex
\begin{itemize}
\item[]
	\activity{Item 1}{Year}
	\activity{Item 2}{Year}
	\activity{Item 3}{Year}
\end{itemize}
```

#### Coursework

A coursework block is simple and is of the form:

```latex
\item[]
	\coursework{Class 1}{Class 2}{Class 3}
	\coursework{Class 4}{Class 5}{Class 6}
	\coursework{Class 7}{Class 8}{Class 9}
\end{itemize}
```

## Contributing

I am open to adding more types of blocks or making changes to current block types. If you have a suggestion, don't be afraid to open a pull request with your change!
