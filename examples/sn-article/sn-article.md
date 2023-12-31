---
title: Article Title
short_title: Short Title
authors:
  - name: First Author
    affiliations:
      - aff1
      - aff2
    corresponding: true
    email: iauthor@gmail.com
  - name: Second Author
    affiliations:
      - aff2
      - aff3
    email: iiauthor@gmail.com
  - name: Third Author
    affiliations:
      - aff1
      - aff3
    #email: iiiauthor@gmail.com

affiliations:
  - id: aff1
    name: 'Affiliation 1,  '
    department: 'Department 1, '
    address: 'Street 1, '
    city: 'City 1, '
    postal_code: ' 100190, '
    state: 'State 1, '
    country: 'Country 1'
    collaboration: false
  - id: aff2
    department: 'Department 2, '
    institution: 'Organization 2, '
    address: 'Street 2, '
    city: 'City 2, '
    postal_code: 'EA10587, '
    state: 'State 2, '
    country: 'Country 2'
    collaboration: false
  - id: aff3
    name: 'Affiliation 3, '
    department: 'Department 3, '
    address: 'Street 3, '
    city: 'City 3, '
    postal_code: 'EA10587, '
    state: 'State 3, '
    country: 'Country 3'
    collaboration: false

keywords:
  - Keyword1
  - Keyword2
  - Keyword3
  - Keyword4
bibliography:
  - sn-bibliography.bib
export:
  - format: pdf+tex
    template: ../../.
    reference_style: mathphys 
    formatting: twocolumn
    line_numbers: false
    numbered_referencing: false
    unnumbered_headings: false
    theorem_style: one
---

%%==================================%%
%% sample for unstructured abstract %%
%%==================================%%

+++ {"part": "abstract"}
The abstract serves both as a general introduction to the topic and as a brief, non-technical summary of the main results and their implications. Authors are advised to check the author instructions for the journal they are submitting to for word limits and if structural elements like subheadings, citations, or equations are permitted.
+++

%%================================%%
%% Sample for structured abstract %%
%%================================%%

% \abstract{\textbf{Purpose:} The abstract serves both as a general introduction to the topic and as a brief, non-technical summary of the main results and their implications. The abstract must not include subheadings (unless expressly permitted in the journal's Instructions to Authors), equations or citations. As a guide the abstract should not exceed 200 words. Most journals do not set a hard limit however authors are advised to check the author instructions for the journal they are submitting to.
% 
% \textbf{Methods:} The abstract serves both as a general introduction to the topic and as a brief, non-technical summary of the main results and their implications. The abstract must not include subheadings (unless expressly permitted in the journal's Instructions to Authors), equations or citations. As a guide the abstract should not exceed 200 words. Most journals do not set a hard limit however authors are advised to check the author instructions for the journal they are submitting to.
% 
% \textbf{Results:} The abstract serves both as a general introduction to the topic and as a brief, non-technical summary of the main results and their implications. The abstract must not include subheadings (unless expressly permitted in the journal's Instructions to Authors), equations or citations. As a guide the abstract should not exceed 200 words. Most journals do not set a hard limit however authors are advised to check the author instructions for the journal they are submitting to.
% 
% \textbf{Conclusion:} The abstract serves both as a general introduction to the topic and as a brief, non-technical summary of the main results and their implications. The abstract must not include subheadings (unless expressly permitted in the journal's Instructions to Authors), equations or citations. As a guide the abstract should not exceed 200 words. Most journals do not set a hard limit however authors are advised to check the author instructions for the journal they are submitting to.}


(sec1)=
# Introduction 

The Introduction section, of referenced text {cite:t}`bib1` expands on the background of the work (some overlap with the Abstract is acceptable). The introduction should not include subheadings.

Springer Nature does not impose a strict layout as standard however authors are advised to check the individual requirements for the journal they are planning to submit to as there may be journal-level preferences. When preparing your text please also be aware that some stylistic choices are not supported in full text XML (publication version), including coloured font. These will not be replicated in the typeset article if it is accepted. 

(sec2)=
# Results

Sample body text. Sample body text. Sample body text. Sample body text. Sample body text. Sample body text. Sample body text. Sample body text.

(sec3)=
# This is an example for first level head---section head

(subsec2)=
## This is an example for second level head---subsection head

(subsubsec2)=
### This is an example for third level head---subsubsection head

Sample body text. Sample body text. Sample body text. Sample body text. Sample body text. Sample body text. Sample body text. Sample body text. 

(sec4)=
# Equations

Equations in LaTex can either be inline or on-a-line by itself (``display equations''). For inline equations use the ```$...$``` commands. E.g.: The equation $H\psi = E \psi$ is written via the command ```$H\psi = E\psi$```.

For display equations (with auto generated equation numbers)
one can use the equation or align environments:
```{math}
:label: eq1
\|\tilde{X}(k)\|^2 \leq\frac{\sum\limits_{i=1}^{p}\left\|\tilde{Y}_i(k)\right\|^2+\sum\limits_{j=1}^{q}\left\|\tilde{Z}_j(k)\right\|^2 }{p+q}.
```
where,
%%```{math}
%%:label: eq2
%%D_\mu &=  \partial_\mu - ig \frac{\lambda^a}{2} A^a_\mu \nonumber \\
%%F^a_{\mu\nu} &= \partial_\mu A^a_\nu - \partial_\nu A^a_\mu + g f^{abc} A^b_\mu A^a_\nu
%%```
Notice the use of ```\nonumber``` in the align environment at the end
of each line, except the last, so as not to produce equation numbers on
lines where no equation numbers are required. The ```\label{}``` command
should only be used at the last line of an align environment where
```\nonumber``` is not used.
```{math}
Y_\infty = \left( \frac{m}{\textrm{GeV}} \right)^{-3}
    \left[ 1 + \frac{3 \ln(m/\textrm{GeV})}{15}
    + \frac{\ln(c_2/5)}{15} \right]
```
The class file also supports the use of ```\mathbb{}```, ```\mathscr{}``` and
```\mathcal{}``` commands. As such ```\mathbb{R}```, ```\mathscr{R}```
and ```\mathcal{R}``` produces $\mathbb{R}$, $\mathscr{R}$ and $\mathcal{R}$
respectively (refer [Subsubsection](#subsubsec2)).

(sec5)=
# Tables

Tables can be inserted via the normal table and tabular environment. To put
footnotes inside tables you should use ```\footnotetext[]{...}``` tag.
The footnote appears just below the table itself (refer [Tables](#tab1) and [](#tab2)). 
For the corresponding footnotemark use ```\footnotemark[...]```

\begin{table}[h]
\caption{Caption text}\label{tab1}%
\begin{tabular}{@{}llll@{}}
\toprule
Column 1 & Column 2  & Column 3 & Column 4\\
\midrule
row 1    & data 1   & data 2  & data 3  \\
row 2    & data 4   & data 5\footnotemark[1]  & data 6  \\
row 3    & data 7   & data 8  & data 9\footnotemark[2]  \\
\botrule
\end{tabular}
\footnotetext{Source: This is an example of table footnote. This is an example of table footnote.}
\footnotetext[1]{Example for a first table footnote. This is an example of table footnote.}
\footnotetext[2]{Example for a second table footnote. This is an example of table footnote.}
\end{table}

The input format for the above table is as follows:

```{code-block} tex
\begin{table}[<placement-specifier>]
\caption{<table-caption>}\label{<table-label>}%
\begin{tabular}{@{}llll@{}}
\toprule
Column 1 & Column 2 & Column 3 & Column 4\\
\midrule
row 1 & data 1 & data 2	 & data 3 \\
row 2 & data 4 & data 5\footnotemark[1] & data 6 \\
row 3 & data 7 & data 8	 & data 9\footnotemark[2]\\
\botrule
\end{tabular}
\footnotetext{Source: This is an example of table footnote. 
This is an example of table footnote.}
\footnotetext[1]{Example for a first table footnote.
This is an example of table footnote.}
\footnotetext[2]{Example for a second table footnote. 
This is an example of table footnote.}
\end{table}
```

%%\begin{table}[h]
%%\caption{Example of a lengthy table which is set to full textwidth}\label{tab2}
%%\begin{tabular*}{\textwidth}{@{\extracolsep\fill}lcccccc}
%%\toprule%
%%& \multicolumn{3}{@{}c@{}}{Element 1\footnotemark[1]} & \multicolumn{3}{@{}c@{}}{Element 2\footnotemark[2]} \\\cmidrule{2-4}\cmidrule{5-7}%
%%Project & Energy & $\sigma_{calc}$ & $\sigma_{expt}$ & Energy & $\sigma_{calc}$ & $\sigma_{expt}$ \\
%%\midrule
%%Element 3  & 990 A & 1168 & $1547\pm12$ & 780 A & 1166 & $1239\pm100$\\
%%Element 4  & 500 A & 961  & $922\pm10$  & 900 A & 1268 & $1092\pm40$\\
%%\botrule
%%\end{tabular*}
%%\footnotetext{Note: This is an example of table footnote. This is an example of table footnote this is an example of table footnote this is an example of~table footnote this is an example of table footnote.}
%%\footnotetext[1]{Example for a first table footnote.}
%%\footnotetext[2]{Example for a second table footnote.}
%%\end{table}


In case of double column layout, tables which do not fit in single column width should be set to full text width. For this, you need to use ```\begin{table*}...+ \end{table*}``` instead of ```begin{table}...\end{table}``` environment. Lengthy tables which do not fit in textwidth should be set as rotated table. For this, you need to use ```\begin{sidewaystable}...\end{sidewaystable}``` instead of ```\begin{table*}...\end{table*}``` environment. This environment puts tables rotated to single column width. For tables rotated to double column width, use ```\begin{sidewaystable*}...\end{sidewaystable*}```.

%%\begin{sidewaystable}
%%\caption{Tables which are too long to fit, should be written using the ``sidewaystable'' environment as shown here}\label{tab3}
%%\begin{tabular*}{\textheight}{@{\extracolsep\fill}lcccccc}
%%\toprule%
%%& \multicolumn{3}{@{}c@{}}{Element 1\footnotemark[1]}& \multicolumn{3}{@{}c@{}}{Element\footnotemark[2]} \\\cmidrule{2-4}\cmidrule{5-7}%
%%Projectile & Energy	& $\sigma_{calc}$ & $\sigma_{expt}$ & Energy & $\sigma_{calc}$ & $\sigma_{expt}$ \\
%%\midrule
%%Element 3 & 990 A & 1168 & $1547\pm12$ & 780 A & 1166 & $1239\pm100$ \\
%%Element 4 & 500 A & 961  & $922\pm10$  & 900 A & 1268 & $1092\pm40$ \\
%%Element 5 & 990 A & 1168 & $1547\pm12$ & 780 A & 1166 & $1239\pm100$ \\
%%Element 6 & 500 A & 961  & $922\pm10$  & 900 A & 1268 & $1092\pm40$ \\
%%\botrule
%%\end{tabular*}
%%\footnotetext{Note: This is an example of table footnote this is an example of table footnote this is an example of table footnote this is an example of~table footnote this is an example of table footnote.}
%%\footnotetext[1]{This is an example of table footnote.}
%%\end{sidewaystable}

(sec6)=
# Figures

As per the LaTeX standards you need to use eps images for LaTeX compilation and ```pdf/jpg/png``` images for ```PDFLaTeX``` compilation. This is one of the major difference between LaTeX and ```PDFLaTeX```. Each image should be from a single input .eps/vector image file. Avoid using subfigures. The command for inserting images for LaTeX and ```PDFLaTeX``` can be generalized. The package used to insert images in LaTeX/```PDFLaTeX``` is the graphicx package. Figures can be inserted via the normal figure environment as shown in the below example:

```{code-block} tex
\begin{figure}[<placement-specifier>]
\centering
\includegraphics{<eps-file>}
\caption{<figure-caption>}\label{<figure-label>}
\end{figure}
```

```{figure} fig.pdf
:name: fig1

This is a widefig. This is an example of long caption this is an example of long caption  this is an example of long caption this is an example of long caption
```

In case of double column layout, the above format puts figure captions/images to single column width. To get spanned images, we need to provide ```\begin{figure*}...\end{figure*}```.

For sample purpose, we have included the width of images in the optional argument of ```\includegraphics``` tag. Please ignore this. 

(sec7)=
# Algorithms, Program codes and Listings

Packages ```algorithm```, ```algorithmicx``` and ```algpseudocode``` are used for setting algorithms in LaTeX using the format:

```{code-block} tex
\begin{algorithm}
\caption{<alg-caption>}\label{<alg-label>}
\begin{algorithmic}[1]
. . .
\end{algorithmic}
\end{algorithm}
```

You may refer above listed package documentations for more details before setting ```algorithm``` environment. For program codes, the ``verbatim'' package is required and the command to be used is ```\begin{verbatim}...\end{verbatim}```. 

Similarly, for ```listings```, use the ```listings``` package. ```\begin{lstlisting}...\end{lstlisting}``` is used to set environments similar to ```\verbatim``` environment. Refer to the ```lstlisting``` package documentation for more details.

A fast exponentiation procedure:

%\lstset{texcl=true,basicstyle=\small\sf,commentstyle=\small\rm,mathescape=true,escapeinside={(*}{*)}}
%\begin{lstlisting}
```{code-block} pascal
begin
  for $i:=1$ to $10$ step $1$ do
      expt($2,i$);  
      newline() od                (*\textrm{Comments will be set flush to the right margin}*)
where
proc expt($x,n$) $\equiv$
  $z:=1$;
  do if $n=0$ then exit fi;
     do if odd($n$) then exit fi;                 
        comment: (*\textrm{This is a comment statement;}*)
        $n:=n/2$; $x:=x*x$ od;
     { $n>0$ };
     $n:=n-1$; $z:=z*x$ od;
  print($z$). 
end
```

%%\begin{algorithm}
%%\caption{Calculate $y = x^n$}\label{algo1}
%%\begin{algorithmic}[1]
%%\Require $n \geq 0 \vee x \neq 0$
%%\Ensure $y = x^n$ 
%%\State $y \Leftarrow 1$
%%\If{$n < 0$}\label{algln2}
%%        \State $X \Leftarrow 1 / x$
%%        \State $N \Leftarrow -n$
%%\Else
%%        \State $X \Leftarrow x$
%%        \State $N \Leftarrow n$
%%\EndIf
%%\While{$N \neq 0$}
%%        \If{$N$ is even}
%%            \State $X \Leftarrow X \times X$
%%            \State $N \Leftarrow N / 2$
%%        \Else[$N$ is odd]
%%            \State $y \Leftarrow y \times X$
%%            \State $N \Leftarrow N - 1$
%%        \EndIf
%%\EndWhile
%%\end{algorithmic}
%%\end{algorithm}



%%\lstset{frame=single,framexleftmargin=-1pt,framexrightmargin=-17pt,framesep=12pt,linewidth=0.98\textwidth,language=pascal}% Set your language (you can change the language for each code-block optionally)
%%% Start your code-block
```{code-block} pascal
for i:=maxint to 0 do
begin
{ do nothing }
end;
Write('Case insensitive ');
Write('Pascal keywords.');
\end{lstlisting}
\end{minipage}
```
(sec8)=
# Cross referencing

Environments such as figure, table, equation and align can have a label
declared via the ```\label{#label}``` command. For figures and table
environments use the ```\label{}``` command inside or just
below the ```\caption{}``` command. You can then use the
```\ref{#label}``` command to cross-reference them. As an example, consider
the label declared for [](#fig1) which is
```\label{fig1}```. To cross-reference it, use the command 
```Figure \ref{fig1}```, for which it comes up as
[](#fig1). 

To reference line numbers in an algorithm, consider the label declared for the line number 2 of [Algorithm](#algo1) is ```\label{algln2}```. To cross-reference it, use the command ```\ref{algln2}``` for which it comes up as line~[](#algln2) of [Algorithm](#algo1).

(subsec7)=
## Details on reference citations

Standard LaTeX permits only numerical citations. To support both numerical and author-year citations this template uses ```natbib```-LaTeX package. For style guidance please refer to the template user manual.

Here is an example for ```\cite{...}```: \cite{bib1}. Another example for ```\citep{...}```: \citep{bib2}. For author-year citation mode, ```\cite{...}``` prints Jones et al. (1990) and ```\citep{...}``` prints (Jones et al., 1990).

All cited bib entries are printed at the end of this article: {cite:t}`bib3`, {cite:t}`bib4`, {cite:t}`bib5`, {cite:t}`bib6`, {cite:t}`bib7`, {cite:t}`bib8`, {cite:t}`bib9`, {cite:t}`bib10`, {cite:t}`bib11`, {cite:t}`bib12` and {cite:t}`bib13`.

(sec10)=
# Examples for theorem like environments

For theorem like environments, we require ```amsthm``` package. There are three types of predefined theorem styles exists---```thmstyleone```, ```thmstyletwo``` and ```thmstylethree```.

%%=============================================%%
%% For presentation purpose, we have included  %%
%% \bigskip command. please ignore this.       %%
%%=============================================%%
%%\bigskip
%%\begin{tabular}{|l|p{19pc}|}
%%\hline
%%\verb+thmstyleone+ & Numbered, theorem head in bold font and theorem text in italic style \\\hline
%%\verb+thmstyletwo+ & Numbered, theorem head in roman font and theorem text in italic style \\\hline
%%\verb+thmstylethree+ & Numbered, theorem head in bold font and theorem text in roman style \\\hline
%%\end{tabular}
%%\bigskip
%%=============================================%%
%% For presentation purpose, we have included  %%
%% \bigskip command. please ignore this.       %%
%%=============================================%%

For mathematics journals, theorem styles can be included as shown in the following examples:

%%\begin{theorem}[Theorem subhead]\label{thm1}
%%Example theorem text. Example theorem text. Example theorem text. Example theorem text. Example theorem text. 
%%Example theorem text. Example theorem text. Example theorem text. Example theorem text. Example theorem text. 
%%Example theorem text. 
%%\end{theorem}

%%:::{prf:theorem} Theorem subhead
%%:label: thm1
%%Example theorem text. Example theorem text. Example theorem text. Example theorem text. Example theorem text. 
%%Example theorem text. Example theorem text. Example theorem text. Example theorem text. Example theorem text. 
%%Example theorem text. 
%%:::

Sample body text. Sample body text. Sample body text. Sample body text. Sample body text. Sample body text. Sample body text. Sample body text.

%%\begin{proposition}
%%Example proposition text. Example proposition text. Example proposition text. Example proposition text. Example proposition text. 
%%Example proposition text. Example proposition text. Example proposition text. Example proposition text. Example proposition text. 
%%\end{proposition}

%%:::{prf:proposition}
%%:label: prop1
%%Example proposition text. Example proposition text. Example proposition text. Example proposition text. Example proposition text. 
%%Example proposition text. Example proposition text. Example proposition text. Example proposition text. Example proposition text.
%%:::

Sample body text. Sample body text. Sample body text. Sample body text. Sample body text. Sample body text. Sample body text. Sample body text.

%%\begin{example}
%%Phasellus adipiscing semper elit. Proin fermentum massa
%%ac quam. Sed diam turpis, molestie vitae, placerat a, molestie nec, leo. Maecenas lacinia. Nam ipsum ligula, eleifend
%%at, accumsan nec, suscipit a, ipsum. Morbi blandit ligula feugiat magna. Nunc eleifend consequat lorem. 
%%\end{example}

%%:::{prf:example}
%%Phasellus adipiscing semper elit. Proin fermentum massa
%%ac quam. Sed diam turpis, molestie vitae, placerat a, molestie nec, leo. Maecenas lacinia. Nam ipsum ligula, eleifend
%%at, accumsan nec, suscipit a, ipsum. Morbi blandit ligula feugiat magna. Nunc eleifend consequat lorem. 
%%:::

Sample body text. Sample body text. Sample body text. Sample body text. Sample body text. Sample body text. Sample body text. Sample body text.

%%\begin{remark}
%%Phasellus adipiscing semper elit. Proin fermentum massa
%%ac quam. Sed diam turpis, molestie vitae, placerat a, molestie nec, leo. Maecenas lacinia. Nam ipsum ligula, eleifend
%%at, accumsan nec, suscipit a, ipsum. Morbi blandit ligula feugiat magna. Nunc eleifend consequat lorem. 
%%\end{remark}

%%:::{prf:remark}
%%Phasellus adipiscing semper elit. Proin fermentum massa
%%ac quam. Sed diam turpis, molestie vitae, placerat a, molestie nec, leo. Maecenas lacinia. Nam ipsum ligula, eleifend
%%at, accumsan nec, suscipit a, ipsum. Morbi blandit ligula feugiat magna. Nunc eleifend consequat lorem.
%%:::

Sample body text. Sample body text. Sample body text. Sample body text. Sample body text. Sample body text. Sample body text. Sample body text.

%%\begin{definition}[Definition sub head]
%%Example definition text. Example definition text. Example definition text. Example definition text. Example definition text. Example definition text. Example definition text. Example definition text. 
%%\end{definition}

%%:::{prf:definition} Definition sub head
%%Example definition text. Example definition text. Example definition text. Example definition text. Example definition text. Example definition text. Example definition text. Example definition text.
%%:::

Additionally a predefined `proof` environment is available: ```\begin{proof}...\end{proof}```. This prints a `Proof` head in italic font style and the `body text` in roman font style with an open square at the end of each proof environment. 

%%\begin{proof}
%%Example for proof text. Example for proof text. Example for proof text. Example for proof text. Example for proof text. Example for proof text. Example for proof text. Example for proof text. Example for proof text. Example for proof text. 
%%\end{proof}

%%:::{prf:proof}
%%Example for proof text. Example for proof text. Example for proof text. Example for proof text. Example for proof text. Example for proof text. Example for proof text. Example for proof text. Example for proof text. Example for proof text. 
%%:::

Sample body text. Sample body text. Sample body text. Sample body text. Sample body text. Sample body text. Sample body text. Sample body text.

%%\begin{proof}[Proof of Theorem~{\upshape\ref{thm1}}]
%%Example for proof text. Example for proof text. Example for proof text. Example for proof text. Example for proof text. Example for proof text. Example for proof text. Example for proof text. Example for proof text. Example for proof text. 
%%\end{proof}

%%:::{prf:proof} Proof of [](#thm1)
%%Example for proof text. Example for proof text. Example for proof text. Example for proof text. Example for proof text. Example for proof text. Example for proof text. Example for proof text. Example for proof text. Example for proof text. 
%%:::

For a quote environment, use `\begin{quote}...\end{quote}`
%%\begin{quote}
%%Quoted text example. Aliquam porttitor quam a lacus. Praesent vel arcu ut tortor cursus volutpat. In vitae pede quis diam bibendum placerat. Fusce elementum
%%convallis neque. Sed dolor orci, scelerisque ac, dapibus nec, ultricies ut, mi. Duis nec dui quis leo sagittis commodo.
%%\end{quote}

> Quoted text example. Aliquam porttitor quam a lacus. Praesent vel arcu ut tortor cursus volutpat. In vitae pede quis diam bibendum placerat. Fusce elementum convallis neque. Sed dolor orci, scelerisque ac, dapibus nec, ultricies ut, mi. Duis nec dui quis leo sagittis commodo.

Sample body text. Sample body text. Sample body text. Sample body text. Sample body text (refer [](#fig1)). Sample body text. Sample body text. Sample body text (refer Table [](#tab3)). 

(sec11)=
# Methods

Topical subheadings are allowed. Authors must ensure that their Methods section includes adequate experimental and characterization data necessary for others in the field to reproduce their work. Authors are encouraged to include RIIDs where appropriate. 

__Ethical approval declarations__ (only required where applicable) Any article reporting experiment/s carried out on (i) live vertebrate (or higher invertebrates), (ii) humans or (iii) human samples must include an unambiguous statement within the methods section that meets the following requirements: 


1. Approval: a statement which confirms that all experimental protocols were approved by a named institutional and/or licensing committee. Please identify the approving body in the methods section

2. Accordance: a statement explicitly saying that the methods were carried out in accordance with the relevant guidelines and regulations

3. Informed consent (for experiments involving humans or human tissue samples): include a statement confirming that informed consent was obtained from all participants and/or their legal guardian/s


If your manuscript includes potentially identifying patient/participant information, or if it describes human transplantation research, or if it reports results of a clinical trial then  additional information will be required. Please visit ([https://www.nature.com/nature-research/editorial-policies](https://www.nature.com/nature-research/editorial-policies)) for Nature Portfolio journals, ([https://www.springer.com/gp/authors-editors/journal-author/journal-author-helpdesk/publishing-ethics/14214](https://www.springer.com/gp/authors-editors/journal-author/journal-author-helpdesk/publishing-ethics/14214)) for Springer Nature journals, or ([https://www.biomedcentral.com/getpublished/editorial-policies\#ethics+and+consent](https://www.biomedcentral.com/getpublished/editorial-policies\#ethics+and+consent)) for BMC.

(sec12)=
# Discussion

Discussions should be brief and focused. In some disciplines use of Discussion or `Conclusion` is interchangeable. It is not mandatory to use both. Some journals prefer a section `Results and Discussion` followed by a section `Conclusion`. Please refer to Journal-level guidance for any specific requirements. 

(sec13)=
# Conclusion

Conclusions may be used to restate your hypothesis or research question, restate your major findings, explain the relevance and the added value of your work, highlight any limitations of your study, describe future directions for research and recommendations. 

In some disciplines use of Discussion or `Conclusion` is interchangeable. It is not mandatory to use both. Please refer to Journal-level guidance for any specific requirements. 


+++ {"part": "supplementary_information"}

If your article has accompanying supplementary file/s please state so here. 

Authors reporting data from electrophoretic gels and blots should supply the full unprocessed scans for key as part of their Supplementary information. This may be requested by the editorial team/s if it is missing.

Please refer to Journal-level guidance for any specific requirements.
+++

+++ {"part": "acknowledgments"}

Acknowledgments are not compulsory. Where included they should be brief. Grant or contribution numbers may be acknowledged.

Please refer to Journal-level guidance for any specific requirements.
+++

+++ {"part": "declarations"}

Some journals require declarations to be submitted in a standardised format. Please check the Instructions for Authors of the journal to which you are submitting to see if you need to complete this section. If yes, your manuscript must contain the following sections under the heading `Declarations':

- Funding
- Conflict of interest/Competing interests (check journal-specific guidelines for which heading to use)
- Ethics approval 
- Consent to participate
- Consent for publication
- Availability of data and materials
- Code availability 
- Authors' contributions

If any of the sections are not relevant to your manuscript, please include the heading and write `Not applicable' for that section. 
+++

%%===================================================%%
%% For presentation purpose, we have included        %%
%% \bigskip command. please ignore this.             %%
%%===================================================%%
%%\bigskip
%%\begin{flushleft}%
Editorial Policies for:

%%\bigskip\noindent
Springer journals and proceedings: [https://www.springer.com/gp/editorial-policie](https://www.springer.com/gp/editorial-policies)

%%\bigskip\noindent
Nature Portfolio journals: [https://www.nature.com/nature-research/editorial-policies](https://www.nature.com/nature-research/editorial-policies)

%%\bigskip\noindent
_Scientific Reports_: [https://www.nature.com/srep/journal-policies/editorial-policies](https://www.nature.com/srep/journal-policies/editorial-policies)

%\bigskip\noindent
BMC journals: [https://www.biomedcentral.com/getpublished/editorial-policies](https://www.biomedcentral.com/getpublished/editorial-policies)
%%\end{flushleft}

+++ {"part": "appendix"}

(secA1)= 
# Section title of first appendix

An appendix contains supplementary information that is not an essential part of the text itself but which may be helpful in providing a more comprehensive understanding of the research problem or it is information that is too cumbersome to be included in the body of the paper.


For submissions to Nature Portfolio Journals please use the heading `Extended Data`.


%%=============================================================%%
%% Sample for another appendix section			       %%
%%=============================================================%%
(secA2)=
# Example of another appendix section

Appendices may be used for helpful, supporting or essential material that would otherwise 
clutter, break up or be distracting to the text. Appendices can consist of sections, figures, tables and equations etc.

+++


 If you are submitting to one of the Nature Portfolio journals, using the eJP submission   
 system, please include the references within the manuscript file itself. You may do this  
by copying the reference list from your .bbl file, paste it into the main manuscript `.tex`
file, and delete the associated `bibliography` commands.                            %%


`\bibliography{sn-bibliography}` common bib file, if required, the content of .bbl file can be included here once bbl is generated `\input sn-article.bbl`.
