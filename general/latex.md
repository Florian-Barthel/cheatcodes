# [Home](../README.md)

### Text style

```tex
Italic \emph{text}
Bold \textbf{text}
```

### Spacing

```tex
\vspace{1.5cm}
\newpage
```

### Table

```tex
\begin{table}[htbp]
    \centering
    \begin{tabular}{l c c c c}
        \hline
        Method & FID & Depth & Pose  & ID $ \\ 
        \hline
        GIRAFFE & 31.5 & 0.94 & 0.089 & 0.64 \\
        \hline
    \end{tabular}

    \caption[Caption Heading]{Caption Text}
    \label{tab:label}
\end{table}

```

### Iterating

```tex
% description
\begin{description}    
    \item[FID] text1
    \item[ID] text2
\end{description}

% dots
\begin{itemize}    
    \item text1
    \item text2
\end{itemize}
```

### Images

```tex
\begin{figure}[htbp]
    \centering
    \includegraphics[width=1.0\textwidth]{Chapters/3_eg3d/img/tri-plane.png}
    \caption[caption title]{caption text}
    \label{fig:tri-plane}
\end{figure}
```

### Ref / Cite

```tex
% nur nummer (1.1)
\ref{}

% nummer + text (Figure 1.1)
\autoref{}

% zitieren
\cite{}

% autor
\citeauthor{}
```

### Use multiple tex files
```tex
\input{Chapters/1_introduction/index}
```