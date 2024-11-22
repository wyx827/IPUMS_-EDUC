# Estimating State Populations Using the 2022 ACS Data

## Overview

This repo leverages data from the 2022 American Community Survey (ACS), obtained through IPUMS USA, to estimate the total number of respondents in each state. The focus is on respondents whose highest educational attainment is a doctoral degree. Using the ratio estimator approach, California is taken as the reference state to calculate proportional estimates for other states.

\section*{Key Components}

\subsection*{Data}
\begin{itemize}
    \item The dataset includes educational attainment levels, focusing on individuals holding doctoral degrees (using the \texttt{EDUCD} variable, where \texttt{EDUCD = 116} indicates a doctoral degree).
    \item State-level data is extracted using the \texttt{STATEICP} variable, which represents state codes.
\end{itemize}

\subsection*{Method}
\begin{itemize}
    \item \textbf{Ratio Estimator Approach:}
    \begin{itemize}
        \item California serves as the reference state, where both the total number of respondents and the number of doctoral degree holders are known.
        \item The ratio of doctoral degree holders to total respondents in California is used to estimate the total population for other states based on their number of doctoral degree holders.
    \end{itemize}
\end{itemize}

\subsection*{Comparison}
\begin{itemize}
    \item The estimated total number of respondents is compared to the actual respondent counts for each state.
    \item The comparison reveals discrepancies, analyzed to understand the impact of regional differences in education and demographics.
\end{itemize}


## Statement on LLM usage

LLMs such as ChatGPT were not used for this paper. 
