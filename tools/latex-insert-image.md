# Image in latex

Images in latex the way i like them.

~~~tex
\begin{figure}[H]
    \centering
    \includegraphics[width=1\linewidth]{image-file-name}
    \caption{image-text}
    \label{fig:image-label}
\end{figure}
~~~

the float package is needed to use the "H" specifier

~~~tex
\usepackage{float}
~~~
