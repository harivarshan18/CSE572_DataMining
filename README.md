\documentclass[11pt]{article}
\usepackage[margin=1in]{geometry}
\usepackage[hidelinks]{hyperref}
\usepackage{enumitem}
\usepackage{parskip}
\usepackage{titlesec}
\titleformat{\section}{\large\bfseries}{}{0em}{}

\begin{document}

\begin{center}
{\LARGE \textbf{CSE 572: Data Mining -- Homework Repository}}\\
\vspace{0.25em}
{\small Author: \textbf{<Your Name>} \quad | \quad Term: \textbf{Spring 2026} \quad | \quad University: \textbf{UCF}}
\end{center}

\vspace{0.5em}

\section*{Overview}
This GitHub repository contains my homework submissions for \textbf{CSE 572 (Data Mining)}.
It includes code, notebooks, reports, and supporting files. The repository will be continuously updated to include all future homework assignments for this course.

\section*{Repository Structure}
\begin{verbatim}
cse572-data-mining/
├── HW1/
│   ├── report/
│   ├── code/
│   └── data/
├── HW2/
│   ├── report/
│   ├── code/
│   └── data/
├── HW3/
│   ├── report/
│   ├── code/
│   └── data/
└── README.tex
\end{verbatim}

\section*{Current Contents}
\subsection*{Homework: Titanic Classification (Kaggle-style)}
This homework explores multiple classification models on the Titanic dataset with a focus on preprocessing and model comparison.

\textbf{Files included:}
\begin{itemize}[leftmargin=1.2em]
    \item \texttt{titanic-data-original.ipynb}: Original baseline notebook.
    \item \texttt{titanic-kaggle.ipynb}: Updated notebook with improved preprocessing and evaluation.
    \item \texttt{train.csv}, \texttt{test.csv}: Titanic dataset files.
\end{itemize}

\textbf{Models evaluated:}
\begin{itemize}[leftmargin=1.2em]
    \item Support Vector Machines
    \item KNN
    \item Logistic Regression
    \item Random Forest
    \item Naive Bayes
    \item Perceptron
    \item Stochastic Gradient Descent
    \item Linear SVC
    \item Decision Tree
\end{itemize}

\textbf{Key preprocessing changes used in the updated version:}
\begin{itemize}[leftmargin=1.2em]
    \item Added \texttt{Age\_missing} indicator and kept \texttt{Age} continuous (no binning).
    \item Log-transformed \texttt{Fare} using \texttt{log(1 + Fare)} to reduce outlier impact.
    \item Extracted \texttt{Deck} from \texttt{Cabin} and encoded it.
    \item Used one-hot encoding for categorical features where appropriate (e.g., Title, Embarked, Deck).
    \item Added cross-validation at the end to check generalization and detect overfitting.
\end{itemize}

\section*{How to Run}
\subsection*{Environment}
Recommended: Python 3.9+ with the following packages:
\begin{itemize}[leftmargin=1.2em]
    \item \texttt{numpy}
    \item \texttt{pandas}
    \item \texttt{scikit-learn}
    \item \texttt{matplotlib} (optional)
    \item \texttt{seaborn} (optional)
\end{itemize}

\subsection*{Running Notebooks}
Open the notebooks using Jupyter:
\begin{verbatim}
jupyter notebook
\end{verbatim}
Then run cells in order:
\begin{itemize}[leftmargin=1.2em]
    \item \texttt{titanic-data-original.ipynb} for baseline results
    \item \texttt{titanic-kaggle.ipynb} for improved preprocessing and updated results
\end{itemize}

\section*{Notes}
\begin{itemize}[leftmargin=1.2em]
    \item Some models (Decision Tree, Random Forest) may show very high \textbf{training} accuracy due to overfitting.
    \item Cross-validation is included in the updated notebook to provide a more realistic estimate of performance.
\end{itemize}

\section*{Future Homeworks}
This repository will be updated throughout the semester. Each homework will include:
\begin{itemize}[leftmargin=1.2em]
    \item Problem statement or prompt (when allowed)
    \item Code and experiments
    \item Report or writeup
    \item Any required datasets or links (as permitted by course policy)
\end{itemize}

\vspace{0.5em}
\noindent\textbf{Course:} CSE 572 Data Mining \\
\textbf{Instructor:} \texttt{<Instructor Name>} \\
\textbf{Repository:} \texttt{<GitHub Repo Link>}

\end{document}
