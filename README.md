\documentclass[Journal,letterpaper]{ascelike-new}
\WarningFilter{caption}{Unknown document class}
%% Please choose the appropriate document class option:
% "Journal" produces double-spaced manuscripts for ASCE journals.
% "NewProceedings" produces single-spaced manuscripts for ASCE conference proceedings.
% "Proceedings" produces older-style single-spaced manuscripts for ASCE conference proceedings. 
%
%% For more details and options, please see the notes in the ascelike-new.cls file.

% Some useful packages...
\usepackage{float}
\usepackage{placeins}
\usepackage{multirow}
\usepackage{booktabs}

\usepackage[utf8]{inputenc}
\usepackage[T1]{fontenc}
\usepackage{lmodern}
\usepackage{graphicx}
\usepackage[style=base,figurename=Fig.,labelfont=bf,labelsep=period]{caption}
\usepackage{subcaption}
\usepackage{amsmath}
\usepackage{amsthm,amssymb}
%\usepackage{amsfonts}
%\usepackage{amssymb}
%\usepackage{amsbsy}
\usepackage{newtxtext,newtxmath}
\usepackage[colorlinks=true,citecolor=red,linkcolor=black]{hyperref}

\usepackage[ruled,vlined,linesnumbered]{algorithm2e} %

\newtheorem{theorem}{Theorem}
\newtheorem{assumption}{Assumption}
\usepackage{hyperref}
\hypersetup{
colorlinks=true,
linkcolor=blue,
anchorcolor=blue,
citecolor=blue}
%
% Please add the first author's last name here for the footer:
\NameTag{Tang, \today}
% Note that this is not displayed if the NoPageNumbers option is used
% in the documentclass declaration.
%
\begin{document}

% You will need to make the title all-caps
\title{Supplementary materials}




\section{Appendixes}
\subsection{Expected payoffs}

\begin{table}[hb]\rmfamily 
   % \Large   %tiny,scriptsize,footnotesize, normalsize ,large,Large,LARGE,huge,Huge
    % \centering    % 设置表格是否居中
    \begin{center}   %  作用同 `\centering`,不同：设置表格和标题之间的间隔
        \caption{Payoff matrix of the three game participants}  % 插入图表标题
        \label{tab:payoff}
        \resizebox{\linewidth}{!}{  % 表格宽度设置为文本宽度
        \begin{tabular}{cccc}  % {l:左对齐,C:居中,r:右对齐} 有多少列设置多少个
        \toprule    % \toprule、\midrule 和 \bottomrule，可分别对表格顶部、中部和底部使用不同粗细的水平线
        \multirow{2}{*}{\begin{tabular}[c]{@{}l@{}}Supplier \end{tabular}} 
        &  \multirow{2}{*}{\begin{tabular}[c]{@{}l@{}} Platform \end{tabular}} 
        &\multicolumn{2}{c}{Buyer} \\ \cline{3-4}  
        % \multirow:合并行; \multicolumn:合并列 ; \cline{x-y}：第x列到第y列插入线条;表格文字过长可嵌入`\begin{tabular}'环境换行
                              &                       &  Honest strategy ($\varGamma_{z}^{+}$)                                                                                                  & Dishonest strategy ($\varGamma_{z}^{-}$)                                                                          \\ \midrule  % 中部水平线
                              &  Honest               & $(1-\xi) \pi + \upsilon R_{S} - \frac{1}{2} \delta \varphi^2$                                                                          & $\upsilon R_{S} - \frac{1}{2} \delta \varphi^2 $                                                                  \\
        Honest                &  strategy             & $\xi \pi + \upsilon (\mathcal{R}_{P} - \mathcal{C}_{P}) - (1 - \upsilon) \mathcal{F}_{P} $                                             & $\upsilon (\mathcal{R}_{P} - \mathcal{C}_{P}) - (1 - \upsilon) \mathcal{F}_{P} $                                  \\
        strategy              & ($\varGamma_{y}^{+}$) & $\mathcal{I}_{B} \mathcal{D} - \pi + \mathcal{R}_{B} $                                                                                 & $\mathcal{I}_{B} \mathcal{D} - \mathcal{F}_{B}  $                                                                 \\              
        ($\varGamma_{x}^{+}$) & Dishonest             & $(1-\xi) \pi - \frac{1}{2} \delta \varphi^2$                                                                                           & $- \frac{1}{2} \delta \varphi^2$                                                                                  \\
                              & strategy              & $\xi \pi  - \mathcal{F}_{P} $                                                                                                          & $ - \mathcal{F}_{P} $                                                                                             \\
                              & ($\varGamma_{y}^{-}$) & $ \mathcal{I}_{B} \mathcal{D} + \mathcal{R}_{B} - \pi $                                                                                & $\mathcal{I}_{B} \mathcal{D} - \mathcal{F}_{B} $                                                                  \\ \midrule
                              &  Honest               & $(1- \upsilon)(1-\eta) (1-\xi) \pi^{'} - \frac{1}{2} \delta \varphi^{'2} - \upsilon \mathcal{F}_{S}$                                      & $-\upsilon \mathcal{F}_{S} - \frac{1}{2} \delta \varphi^{'2} $                                                       \\
        Dishonest             & strategy              & $(1 - \upsilon) ((1 - \eta) \xi \pi^{'} - \mathcal{F}_{P}) + \upsilon (\mathcal{R}_{P} - \mathcal{C}_{P})$                             & $\upsilon (\mathcal{R}_{P} - \mathcal{C}_{P}) - (1 - \upsilon) \gamma \mathcal{F}_{P} $                           \\
        strategy              & ($\varGamma_{y}^{+}$) & $(1 - \upsilon) (1 - \eta )(\mathcal{I}_{B}\mathcal{D}^{'} - \pi^{'}  + \mathcal{R}_{B} - \mathcal{L}_{B})$                            & $(1 - \upsilon) (1 - \gamma ) (\mathcal{I}_{B} \mathcal{D}^{'} - \mathcal{F}_{B}- \mathcal{L}_{B}) $              \\
        ($\varGamma_{x}^{-}$) & Dishonest             & $(1-\xi) \pi^{'} - \frac{1}{2} \delta \varphi^{'2}- w_{S}^{c}$                                                                            & $- \frac{1}{2} \delta \varphi^{'2} - w_{S}^{c}$                                                                      \\ 
                              &  strategy             & $\xi\pi^{'}  - \mathcal{F}_{P} + w_{S}^{c} - w_{P}^{c}$                                                                                & $- \mathcal{F}_{P} - w_{P}^{c} + w_{S}^{c}$                                                                       \\
                              & ($\varGamma_{y}^{-}$) & $ \mathcal{I}_{d} \mathcal{D}^{'} - \pi^{'}  + \mathcal{R}_{B} - \mathcal{L}_{B}$                                                      & $ \mathcal{I}_{B} \mathcal{D}^{'}  - \mathcal{F}_{B} - \mathcal{L}_{B}$                                           \\ \bottomrule
    \end{tabular}
    }
    \end{center}
\end{table}

For suppliers, the expected payoff for choosing $\varGamma_{x}^{+} $ (trusted strategy) and $ \varGamma_{x}^{-} $ (untrusted strategy) are denoted as $ E_{x}^{+} $ and $ E_{x}^{-} $, respectively. 
According to the payoff matrix described in Table \ref{tab:payoff}, the expected payoff for suppliers, $ E_{x}^{+} $ and $ E_{x}^{-} $  can be formulated as follows:
%suppliers的期望收益
\begin{small}
\begin{equation}
    \begin{aligned}
         E_{x}^{+} =& y z ((1-\xi) \pi + \upsilon R_{S} - \frac{1}{2} \delta \varphi^2) + y (1 - z) (\upsilon R_{S} - \frac{1}{2} \delta \varphi^2) 
           \\ &+ (1 - y) z ((1-\xi) \pi - \frac{1}{2} \delta \varphi^2) + (1 - y) (1 - z) (- \frac{1}{2} \delta \varphi^2)
    \end{aligned}
\end{equation}
\end{small}

\begin{small}
\begin{equation}
    \begin{aligned}
        E_{x}^{-} =& y z ((1- \upsilon)(1-\eta) (1-\xi) \pi^{'} - \frac{1}{2} \delta \varphi^{'2} - \upsilon \mathcal{F}_{S}) + y (1 - z)\\
                  & (-\upsilon \mathcal{F}_{S} - \frac{1}{2} \delta \varphi^{'2} ) + (1 - y) z ((1-\xi) \pi^{'} - \frac{1}{2} \delta \varphi^{'2} - w_{S}^{c}) \\
                  &+ (1 - y) (1 - z) (- \frac{1}{2} \delta \varphi^{'2}  - w_{S}^{c})
    \end{aligned}
\end{equation}
\end{small}


According to the pairwise proportional imitation dynamics \cite{liuEvolutionaryGameMining2018}, a supplier with strategy $ \varGamma_{x}^{i} $  will imitate another supplier with strategy $ \varGamma_{x}^{-i} $ with a probability of $ \varGamma_{x}^{i}$.

\begin{small}
\begin{equation} \label{eq:psi_x }
    \begin{aligned}
        \psi _{x}^{-i} = \rho_{x}^{-i} max{\{(E_{x}^{-i} - E_{x}^{i}), 0\}}
    \end{aligned}
\end{equation}
\end{small}

where $ i \in \{ +, -\}$.  $ \rho_{x}^{-i} $ denotes the proportion of suppliers with strategy $ \varGamma_{x}^{-i} $ in the population. 
When $i=+$, $\rho_{x}^{-i}= 1-x$, and when $i=-$, $\rho_{x}^{-i}= x$.

Eq.~\eqref{eq:psi_x } indicates that when suppliers adopt a strategy $ \varGamma_{x}^{i} $ with higher returns, they will continue to maintain this strategy in the next time. 
On the contrary, suppliers will switch to strategy  $ \varGamma_{x}^{-i} $ with a certain probability, depending on $ x^{-i} $ and the difference in payoffs.

Similarly, the expected payoffs for the platform and demanders can be formulated as follows:

%Platform的期望收益
\begin{small}
    \begin{equation}
        \begin{aligned}
            E_{y}^{+} =& x z (\xi \pi + \upsilon (\mathcal{R}_{P} - \mathcal{C}_{P}) - (1 - \upsilon) \mathcal{F}_{P} ) + x (1 - z) 
            \\ &(\upsilon (\mathcal{R}_{P} - \mathcal{C}_{P}) - (1 - \upsilon) \mathcal{F}_{P}) + (1 - x) z ((1 - \upsilon) 
            \\ &((1 - \eta) \xi \pi^{'} - \mathcal{F}_{P}) + \upsilon (\mathcal{R}_{P} - \mathcal{C}_{P})) + (1 - x) (1 - z) 
            \\ &(\upsilon (\mathcal{R}_{P} - \mathcal{C}_{P}) - (1 - \upsilon) \gamma \mathcal{F}_{P} )
        \end{aligned}
    \end{equation}
    \end{small}
    
    \begin{small}
    \begin{equation}
        \begin{aligned}
            E_{y}^{-} =& x z (\xi \pi  - \mathcal{F}_{P})  + (1 - x) z (\xi\pi^{'}  - \mathcal{F}_{P} + w_{S}^{c} - w_{P}^{c}) 
            \\ &+ x (1 - z) (- \mathcal{F}_{P})+ (1-x) (1 - z) (- \mathcal{F}_{P} - w_{P}^{c} + w_{S}^{c})
        \end{aligned}
    \end{equation}
    \end{small}

The transition probability of the platform shifting from strategy  $ \varGamma_{y}^{i} $ to strategy  $ \varGamma_{y}^{-i} $  is determined by the relative expected payoffs of the two strategies. 
This dynamic can be formally expressed using the following transition probability function:

\begin{small}
    \begin{equation} \label{eq:psi_y }
        \begin{aligned}
            \psi_{y}^{-i} = \rho_{y}^{-i} max{\{(E_{y}^{-i} - E_{y}^{i}), 0\}}
        \end{aligned}
    \end{equation}
    \end{small}

    where $ i \in \{ +, -\}$ represents the strategic orientation, with '+'and '-' indicating distinct strategic choices. 
    The values y and (1-y) correspond to the relative probabilities assigned to each strategic alternative based on their expected utility.

    The expected payoffs for the buyer adopting trusted and untrusted strategies are formally denoted as $E_{z}^{+}$ and $E_{z}^{-}$, respectively.

%demanders的期望收益
\begin{small}
    \begin{equation}
        \begin{aligned}
            E_{z}^{+} =& x y (\mathcal{I}_{B} \mathcal{D} - \pi + \mathcal{R}_{B}) + x (1 - y) (\mathcal{I}_{B} \mathcal{D} + \mathcal{R}_{B} - \pi ) 
            \\ &+ (1 - x) y ((1 - \upsilon) (1 - \eta )(\mathcal{I}_{B}\mathcal{D}^{'} - \pi^{'}+ \mathcal{R}_{B} - \mathcal{L}_{B}))
            \\ &+ (1 - x) (1 - y) ( )
        \end{aligned}
    \end{equation}
    \end{small}
    
    \begin{small}
    \begin{equation}
        \begin{aligned}
            E_{z}^{-} =& x y (\mathcal{I}_{B} \mathcal{D} - \mathcal{F}_{B}) + x (1 - y) (\mathcal{I}_{B} \mathcal{D} - \mathcal{F}_{B}) 
            \\ &+ (1 - x) y ((1 - \upsilon) (1 - \gamma ) (\mathcal{I}_{B} \mathcal{D}^{'} - \mathcal{F}_{B}- \mathcal{L}_{B}))
            \\ &+ (1 - x) (1 - y) (\mathcal{I}_{B} \mathcal{D}^{'}  - \mathcal{F}_{B} - \mathcal{L}_{B})
        \end{aligned}
    \end{equation}
    \end{small}

    Building upon these payoff expectations, we derive the transition probability $\psi_{z}^{i}$, which characterizes the buyer's strategic shift from $ \varGamma_{z}^{i} $ to $ \varGamma_{z}^{-i} $ according to the pairwise proportional imitation rule. 
    This probability is mathematically expressed as:

    \begin{small}
        \begin{equation} \label{eq:psi_z }
            \begin{aligned}
                \psi_{z}^{-i} = \rho_{z}^{-i} max{\{(E_{z}^{-i} - E_{z}^{i}), 0\}}
            \end{aligned}
        \end{equation}
        \end{small}

where the $\rho_{z}^{i} $ represents the imitation propensity under the current strategy, while $\rho_{z}^{-i} $  captures the complementary probability for the opposite strategy.
 

\subsection{Replicator dynamics equation and eigenvalues of the Jacobian matrix}

\begin{align}\label{eq:F1}
    \left\{\begin{aligned}
        F(x) = \frac{dx}{dt} &= x(E_{x}^{+} - \bar{E_{x}} )  \\
        F(y) = \frac{dy}{dt} &= y(E_{y}^{+} - \bar{E_{y}} )  \\
        F(z) = \frac{dz}{dt} &= z(E_{z}^{+} - \bar{E_{z}} )
    \end{aligned}\right.
\end{align}

where $ F(x)$, $ F(y)$, and $ F(z)$ represent the evolutionary growth rates of the proportion of suppliers, platforms, and buyers with trusted strategies$(x, y, z) $, respectively. 
 $\bar{E_{x} }$, $\bar{E_{y} }$, and $\bar{E_{z} }$ are the average expected payoffs of suppliers, platforms, and buyers.

Based on Eq.~\eqref{eq:F1}, the evolutionary dynamics of the three-party evolutionary game can be described by the replicator dynamic equation shown in Eq.~\eqref{eq:F2}.
    \begin{align}\label{eq:F2}
        \left\{\begin{aligned}
        F(x) &= x(1-x)(y (\upsilon (\mathcal{F}_{S} + \mathcal{R}_{S}) - w_{S}^{c}) + w_{S}^{c} + \frac{1}{2} \delta (\varphi^{2}-\varphi^{'2}) + z (1-\xi)((1-\eta)(1-\upsilon) \pi^{'} + \pi)) \\
        F(y) &= y(1-y)((1-x) z \xi (\eta + (1-\eta) \upsilon) \pi^{'} + \upsilon (\mathcal{F}_{P} + \mathcal{R}_{P} - \mathcal{C}_{P}) - (1-x) (w_{P}^{c} - w_{S}^{c})) \\
        F(z) &= z(1-z)((1-x) y (\eta + (1-\eta)\upsilon)(\pi^{'} - \mathcal{R}_{B}- \mathcal{F}_{B}) + x(\pi^{'}-\pi) - \pi^{'} + \mathcal{R}_{B} + \mathcal{F}_{B}) 
    \end{aligned}\right.
    \end{align}
The dynamic equations in Eq.~ \eqref{eq:F2} capture the temporal changes in strategy frequencies across the three populations. 
These equations emerge from the aggregate effect of individual payoff-maximizing behavior under bounded rationality, ultimately determining the system's evolutionary trajectory toward potential equilibrium states.

The replicator dynamics equation shown in Eq.~\eqref{eq:F2} forms a three-dimensional dynamical evolutionary system.
By setting $ F(x) = F(y) = F(z)$, 8 equilibrium points(EP) can be obtained, as shown in Table \ref{tab:Eigenvalues}. 
However, not all equilibrium points are evolutionarily stable. These equilibrium points may not necessarily be the ESS points of this evolutionary game.
According to Friedman's theorem, the ESS of the three-party evolutionary game can be determined by examining the Jacobian matrix of the dynamic equation \cite{friedmanEvolutionaryGamesEconomics1991}.
For a given equilibrium point, if all eigenvalues of the Jacobian matrix have negative real parts, the equilibrium point is locally stable and can be considered as an ESS point.
Taking the partial derivatives of $ F(x)$, $ F(y)$, and $ F(z)$ described in Eq.~\eqref{eq:F2} with  respect to $ x$, $ y$, and $ z$, the Jacobian matrix can be formulated as Eq.~\eqref{eq:J2}:

\begin{equation}\label{eq:J2}
    \boldsymbol{\mathit{J}} = 
        \begin{bmatrix}
            
            (2x-1)(z\mathcal{K}_{6}-y\mathcal{K}_{1} +\mathcal{K}_{2} )       & x(1-x) (-z (1-\xi) \rho \pi^{'} + \mathcal{K}_{1}-w_{S}^{c})                      &  x(x-1)\mathcal{K}_{6}                                                \\ 
            
             y(y-1)(z\xi\rho \pi^{'}- \mathcal{K}_{5})                        & (2y-1)(\mathcal{K}_{4} + (1-x)(\mathcal{K}_{5}-z \rho \pi))                       &  y (1-y) (1-x) \rho \xi \pi^{'}                                       \\
            
             z (z-1) ( y \rho \mathcal{K}_{3} + \varDelta \pi)                &  z (z-1)(1-x)\rho \mathcal{K}_{3}                                                 &  (1-2z) ((1+y\rho
             \\
              &    & xy\rho)\mathcal{K}_{3}+x \varDelta \pi)
        \end{bmatrix}
\end{equation}


 where $  \rho = (\eta - 1) \upsilon - \eta $,  $\mathcal{K}_1= \upsilon (\mathcal{F}_{S} + \mathcal{R}_{S})$, $\mathcal{K}_2= \frac{1}{2} \delta (\varphi^{2}-\varphi^{'2})- (1-y)w_{S}^{c}$, $\mathcal{K}_3= \mathcal{F}_{B} + \mathcal{R}_{B} -\pi^{'} $, $ \mathcal{K}_4= \upsilon(\mathcal{C}_{P} - \mathcal{R}_{P} -\mathcal{F}_{P} )$, and $ \mathcal{K}_{5}= w_{S}^{c}-w_{P}^{c}  $ , and $ \varDelta \pi = \pi^{'} - \pi$.

Furthermore, by substituting the equilibrium points $\mathscr{E}_1(0, 0, 0)$ to $\mathscr{E}_8(1, 1, 1)$ into Eq.~\eqref{eq:J2} and solving for the eigenvalues of the Jacobian matrix, the results are presented in Table \ref{tab:Eigenvalues}. 

According to \cite{lyapunovGeneralProblemStability1992}, the stability of the equilibrium point can be determined by the eigenvalues of the Jacobian matrix. 
If all eigenvalues are negative, the equilibrium point is locally stable. 
That is, the evolutionary system will evolve towards the equilibrium point ESS only when $\lambda_{1}, \lambda_{2}, \lambda_{3} < 0 $ are all satisfied.
Based on Table \ref{tab:Eigenvalues}, we will discuss the stability of different equilibrium points and analyze the parameter conditions required for the evolution of the three entities (suppliers, platform, and demanders) towards a trustworthy state:

\begin{table*}[htbp]\rmfamily
    % \centering    % 设置表格是否居中
    \begin{center}   %  作用同 `\centering`,不同：设置表格和标题之间的间隔,效果见表2.
        \caption{Equilibrium Points (EP) and eigenvalues of Jacobian matrix.}  % 插入图表标题
        \label{tab:Eigenvalues}  % 表格标签
        \resizebox{\linewidth}{!}{  % 表格宽度设置为文本宽度
        \begin{tabular}{clll}  % {l:左对齐,C:居中,r:右对齐} 有多少列设置多少个
        \toprule    % \toprule、\midrule 和 \bottomrule，可分别对表格顶部、中部和底部使用不同粗细的水平线
        \begin{tabular}[c]{@{}l@{}} EP \end{tabular} & {Eigenvalue $\lambda_{1}$} & {Eigenvalue $\lambda_{2}$} & {Eigenvalue $\lambda_{3}$}    \\  \midrule  % 中部水平线
        % \multirow:合并行; \multicolumn:合并列 ; \cline{x-y}：第x列到第y列插入线条;表格文字过长可嵌入`\begin{tabular}'环境换行
        $\mathscr{E}_{1} (0,0,0)  $  & $ w_{S}^{c} - \frac{1}{2} \delta (\varphi^{2}-\varphi^{'2})$                  & $ \mathcal{F}_{B} + \mathcal{R}_{B} - \pi^{'}$                                                                                       &  $  \upsilon (\mathcal{R}_{P} + \mathcal{F}_{P}- \mathcal{C}_{P}) - (w_{S}^{c}- w_{P}^{c}) $                                               \\
        $\mathscr{E}_{2} (1,0,0)  $  & $ \mathcal{F}_{B} + \mathcal{R}_{B} - \pi$                                    & $ \upsilon (\mathcal{R}_{P}+ \mathcal{F}_{P} - \mathcal{C}_{P} )$                                                                    &  $ -(w_{S}^{c} - \frac{1}{2} \delta (\varphi^{2}-\varphi^{'2}))$                                                                        \\
        $\mathscr{E}_{3} (0,1,0)  $  & $ (1-\eta)(1-\upsilon)(\mathcal{F}_{B} + \mathcal{R}_{B} - \pi)$              & $ \upsilon (\mathcal{R}_{S} + \mathcal{F}_{S}) - (\frac{1}{2} \delta (\varphi^{2}-\varphi^{'2})) $                                   &  $ \upsilon (\mathcal{C}_{P} -\mathcal{R}_{P} - \mathcal{F}_{P}) + w_{S}^{c}- w_{P}^{c}$                                                   \\
        $\mathscr{E}_{4} (0,0,1)  $  & $ \pi - \mathcal{F}_{B} - \mathcal{R}_{B}$                                    & $ (1-\xi) (\pi - \pi^{'}) - \frac{1}{2} \delta (\varphi^{2}-\varphi^{'2}) + w_{S}^{c}$                                               &  $ ((\eta-1)\upsilon - \eta) \xi \pi^{'} +\upsilon(\mathcal{R}_{P} + \mathcal{F}_{P} -\mathcal{C}_{P}) - (w_{S}^{c} - w_{P}^{c})$          \\
        $\mathscr{E}_{5} (1,1,0)  $  & $ \mathcal{F}_{B} + \mathcal{R}_{B} - \pi $                                   & $ \upsilon (\mathcal{C}_{P} -\mathcal{R}_{P} - \mathcal{F}_{P})$                                                                     &  $ \frac{1}{2} \delta (\varphi^{2}-\varphi^{'2}) - \upsilon (\mathcal{R}_{S} + \mathcal{F}_{S})$                                           \\   
        $\mathscr{E}_{6} (1,0,1)  $  & $ \upsilon (\mathcal{R}_{P}+ \mathcal{F}_{P} - \mathcal{C}_{P})$              & $ \pi - \mathcal{F}_{B} - \mathcal{R}_{B}$                                                                                           &  $ \frac{1}{2} \delta (\varphi^{2}-\varphi^{'2}) - (1-\xi)(\pi - \pi^{'}) - w_{S}^{c} $                                                    \\
        $\mathscr{E}_{7} (0,1,1)  $  & $ -(1-\eta) (1-\upsilon)(\mathcal{F}_{B} + \mathcal{R}_{B} - \pi^{'}) $       & $ -((\eta-1)\upsilon - \eta) \xi \pi^{'} -\upsilon(\mathcal{R}_{P} + \mathcal{F}_{P} -\mathcal{C}_{P}) + (w_{S}^{c} - w_{P}^{c}) $   &  $ (1-\xi)(\pi - (1-\eta)(1-\upsilon)\pi^{'}) + \upsilon (\mathcal{R}_{S} + \mathcal{F}_{S}) - \frac{1}{2} \delta (\varphi^{2}-\varphi^{'2})$   \\
        $\mathscr{E}_{8} (1,1,1)  $  & $ -\upsilon (\mathcal{R}_{P}+ \mathcal{F}_{P} - \mathcal{C}_{P}) $            & $ -(\mathcal{F}_{B} + \mathcal{R}_{B}-\pi )     $                                                                                      &  $ -(1-\xi)(\pi - (1-\eta)(1-\upsilon)\pi^{'}) - \upsilon (\mathcal{R}_{S} + \mathcal{F}_{S}) + \frac{1}{2} \delta (\varphi^{2}-\varphi^{'2})$                                                                  
        \\ \bottomrule   % 底部水平线
        \end{tabular}
        }
    \end{center}
\end{table*}

\subsection{Proof of theorems}
\subsubsection{Proof of Theorem 1}
\begin{theorem} \label{thm:1}
    To prevent untrusted strategy of buyers, the reputation reward and punishment that a buyer receive $( \mathcal{R}_{B}, \mathcal{F}_{B})$ should meet the condition $ \mathcal{R}_{B}+ \mathcal{F}_{B} > \pi^{'}$, where $\pi^{'}$ is the payment made by the buyer for products delivery when suppliers choose dishonest strategy.
\end{theorem}
\begin{proof}
    \renewcommand{\qedsymbol}{} % 去掉证明结束时的方框
    When the buyers choose the untrusted strategy $(z=0)$, there are four equilibrium points:  $\mathscr{E}_{1} (0,0,0)$, $\mathscr{E}_{2} (1,0,0)$, $\mathscr{E}_{3} (0,1,0)$, and $\mathscr{E}_{5} (1,1,0)$.
    The stability of these equilibrium points is determined by the eigenvalues of the Jacobian matrix.
    According to Table \ref{tab:Eigenvalues}, when the condition $ \mathcal{R}_{B}+ \mathcal{F}_{B} - \pi^{'} > 0$ meets, the condition $ \mathcal{R}_{B}+ \mathcal{F}_{B} - \pi >0$ also holds. 
    There are non-negative values in the eigenvalues corresponding to the four equilibrium points mentioned above, as shown in Eq.~\eqref{eq:lambda z}.
    The presence of nonnegative eigenvalues at all four equilibrium points indicates that none of them satisfy the conditions for an evolutionary stable strategy (ESS).
    \begin{align}\label{eq:lambda z}
        \left\{\begin{aligned}
        \lambda_2 (\mathscr{E}_{1}) &= \mathcal{R}_{B}+ \mathcal{F}_{B} - \pi^{'} > 0                        \\
        \lambda_1 (\mathscr{E}_{2}) &= \mathcal{R}_{B}+ \mathcal{F}_{B} - \pi > 0                        \\
        \lambda_1 (\mathscr{E}_{3}) &= (1-\upsilon)(1-\eta)(\mathcal{R}_{B}+ \mathcal{F}_{B} - \pi) > 0  \\
        \lambda_1 (\mathscr{E}_{5}) &= \mathcal{R}_{B}+ \mathcal{F}_{B} - \pi > 0                        
    \end{aligned}\right.\end{align}
\end{proof}

\subsubsection{Proof of Theorem 2}
 \begin{theorem}
    In the absence of platform oversight, construction material suppliers tend to become untrustworthy.
 \end{theorem}
 \begin{proof}
    \renewcommand{\qedsymbol}{}
    When platforms choose to not regulate the quality of products from construction material suppliers $ (y=0) $, there are four equilibrium points at this point: $ \mathscr{E}_{1} (0,0,0) $, $ \mathscr{E}_{2} (1,0,0) $, $ \mathscr{E}_{4} (0,0,1) $, and $ \mathscr{E}_{6} (1,0,1) $.
    As shown in Table ~\ref{tab:Eigenvalues}, the eigenvalues $ \lambda_{1}( \mathscr{E}_{1}) = w_{S}^{c} - \frac{1}{2} \delta (\varphi^{2}-\varphi^{'2})$, $\lambda_{3}(\mathscr{E}_{2}) = -(w_{S}^{c} - \frac{1}{2} \delta (\varphi^{2}-\varphi^{'2}))$, $ \lambda_{2}(\mathscr{E}_{4}) = (1-\xi) (\pi - \pi^{'}) - \frac{1}{2} \delta (\varphi^{2}-\varphi^{'2}) + w_{S}^{c}$ and $ \lambda_{3}( \mathscr{E}_{6}) = \frac{1}{2} \delta (\varphi^{2}-\varphi^{'2}) - (1-\xi)(\pi - \pi^{'}) - w_{S}^{c}$.
    According to the hypothesis in Section 3.1, the cost of high-quality products $\frac{1}{2} \delta \varphi^{2}$ is greater than that of low-quality products and collusion $ \frac{1}{2}\delta\varphi^{'2} + w_{S}^{c} $.
    The profit of honest suppliers is less than that of dishonest suppliers, $\pi - \pi^{'} < 0$.
    Therefore, $ \lambda_{1}( \mathscr{E}_{1}) < 0$, $ \lambda_{3}( \mathscr{E}_{2}) > 0$, $ \lambda_{2}( \mathscr{E}_{4}) > 0$, and $ \lambda_{3}( \mathscr{E}_{6}) < 0$.
    This implies that the equilibrium points $ \mathscr{E}_{1} (0,0,0)$ and $ \mathscr{E}_{6} (1,0,1)$ are locally stable, while the equilibrium points $ \mathscr{E}_{2} (1,0,0)$ and $ \mathscr{E}_{4} (0,0,1)$ are unstable.
    And the evolutionary direction of suppliers is to adopt untrustworthy strategies without platform's regulation.
\end{proof}

\subsubsection{Proof of Theorem 3}

\begin{theorem} \label{thm:cost}
    When the cost of verifying the quality of materials provided by suppliers ($\mathcal{C}_{P}$) exceeds the sum of reputation-based rewards and penalties in a certain proportion ($\mathcal{R}_{P} + \mathcal{F}_{P}$), the platform cannot sustain a Trusted strategy.
\end{theorem}
\begin{proof}
    \renewcommand{\qedsymbol}{}
    When the platforms select the Trusted strategy($y=1$), the corresponding equilibrium points include $\mathscr{E}_{3}$, $\mathscr{E}_{5}$, $\mathscr{E}_{7}$, $\mathscr{E}_{8}$.
    The eigenvalues associated with these four equilibrium points can been seen in Table ~\ref{tab:Eigenvalues}.
    According to section 3.1, suppliers' collusion cost $w_{S}^{c}$ paid to platform is greater than platforms' collusion cost $w_{P}^{c}$ for information fraud, thus $\mathcal{K}_{5}=w_{S}^{c}-w_{P}^{c}>0$. 
    $\upsilon$, $\eta$, and $\xi$ all range from 0 to 1, so $\rho = (\eta - 1) \upsilon - \eta < 0$.
    Therefore, when the condition $\mathcal{K}_{4}=\upsilon(\mathcal{C}_{P} - \mathcal{R}_{P} -\mathcal{F}_{P} )>0$ we derive the non-negativity of the following eigenvalues:
    \begin{align}\label{eq:lambda}
        \left\{\begin{aligned}
            \lambda_3 (\mathscr{E}_{3}) &= \mathcal{K}_{4} + \mathcal{K}_{5} > 0                     \\
            \lambda_2 (\mathscr{E}_{5}) &= -\mathcal{K}_{4} > 0                                      \\
            \lambda_3 (\mathscr{E}_{7}) &=-\rho \xi \pi^{'} +\mathcal{K}_{4} + \mathcal{K}_{5} > 0   \\
            \lambda_2 (\mathscr{E}_{8}) &= \mathcal{K}_{4} > 0  
    \end{aligned}\right.
    \end{align}
According to the analysis above, when the platform's verification cost exceeds the sum of reputation-based rewards and penalties, $\mathscr{E}_{3}$, $\mathscr{E}_{5}$, $\mathscr{E}_{7}$, and $\mathscr{E}_{8}$ cannot be the stable points in the evolutionary game, and the platform will not be able to sustain a trustworthy strategy.
\end{proof}

\subsubsection{Proof of Theorem 4}
 \begin{theorem} \label{thm:upsilon}
    To avoid suppliers' free-riding behavior, the verification rate $\upsilon$ of the platforms should meet the following requirement:   
    \begin{align}\label{eq:upsilon}
        \left\{\begin{aligned}
        \upsilon >& min(\upsilon_{1}^{*}, \upsilon_{2}^{*}), when  z = 0; \\
        \upsilon >& \upsilon_{3}^{*} , when  z = 1.
    \end{aligned}\right.\end{align}
\end{theorem}
\begin{proof}
    \renewcommand{\qedsymbol}{}
    This game-theoretic analysis reveals that when the platform adopts a regulatory strategy while construction material suppliers employ untrustworthy strategies, the system converges to two Nash equilibrium points: $\mathscr{E}_{3}(0,1,0)$ and $\mathscr{E}_{7}(0,1,1)$.
    Through Jacobian matrix eigenvalue analysis, the minimum verification rate  $\upsilon$  required to destabilize these equilibrium points can be derived under two distinct scenarios:

    (1) Case with untrustworthy demanders ($\mathscr{E}_{3}(0,1,0)$):
     In this scenario, supplier behavior is solely constrained by the platform's reputation-based reward-punishment mechanism. 
    To ensure the instability of this equilibrium, the eigenvalues   should satisfy: $\lambda_{2}(\mathscr{E}_{3})= \upsilon (\mathcal{R}_{S} + \mathcal{F}_{S}) - (\frac{1}{2} \delta (\varphi^{2}-\varphi^{'2}))> 0$, or $\lambda_{2}(\mathscr{E}_{3})=\upsilon (\mathcal{C}_{P} -\mathcal{R}_{P} - \mathcal{F}_{P}) + w_{S}^{c}- w_{P}^{c}>0$.
    This yields the critical verification threshold: $\upsilon>min(\upsilon_{1}^{*}, \upsilon_{2}^{*})$, where $\upsilon_{1}^{*}=\frac{\delta (\varphi^{2}-\varphi^{'2})}{2(\mathcal{R}_{S} + \mathcal{F}_{S})} $, $\upsilon_{2}^{*}=\frac{w_{S}^{c}- w_{P}^{c}}{\mathcal{R}_{P} + \mathcal{F}_{P} - \mathcal{C}_{P}}$.
    
    (2) Case with trustworthy demanders ($\mathscr{E}_{7}(0,1,1)$):
Here, supplier behavior is jointly constrained by both the platform's reputation mechanism and demanders' monetary incentives.
    Similarly, the stability condition $\lambda_{3}(\mathscr{E}_{7})>0$ requires:$  (1-\xi)(\pi - (1-\eta)(1-\upsilon)\pi^{'}) + \upsilon (\mathcal{R}_{S} + \mathcal{F}_{S}) - \frac{1}{2} \delta (\varphi^{2}-\varphi^{'2})>0$. 
    So we have the verification threshold in this scenario: $\upsilon > \upsilon_{3}^{*}=\frac{2(1-\xi)((1-\eta)\pi^{'}-\pi) + \delta (\varphi^{2}-\varphi^{'2})}{2(\rho \pi^{'} + \mathcal{R}_{S} + \mathcal{F}_{S})}$.
\end{proof}

Note that the positive or negative values of other eigenvalues are not directly related to the value of $\upsilon$.

\subsubsection{Proof of Theorem 5}

\begin{theorem} \label{thm:condition1}
    When the parametric relationship specified in Eq.~\eqref{eq:condition1}  is satisfied, the adoption of trustworthy strategies by all three stakeholders (building material suppliers, platforms, and buyers) emerges as the unique evolutionary stable outcome of this game. 
    The mathematical formulation of Eq.~\eqref{eq:condition1}  is presented as follows:
    \begin{align}\label{eq:condition1}
        \left\{\begin{aligned}
            &\pi < \mathcal{R}_{B} + \mathcal{F}_{B}     \\
            &\mathcal{C}_{P} < \mathcal{R}_{P} + \mathcal{F}_{P}-(1-\eta)\xi \pi^{'} \\
            &\upsilon > max(min(\upsilon_{1}^{*}, \upsilon_{2}^{*}), \upsilon_{3}^{*}, \upsilon_{4}^{*}), \upsilon_{4}^{*}=\frac{\eta\xi\pi^{'} + w_{S}^{c}-w_{P}^{c}}{\mathcal{C}_{P} - \mathcal{R}_{P} - \mathcal{F}_{P} + (1-\eta)\xi \pi^{'}}
    \end{aligned}\right.\end{align}
\end{theorem}
\begin{proof}
    \renewcommand{\qedsymbol}{}
    First, we examine the stability conditions of equilibrium point $\mathscr{E}_{8}(1,1,1)$ when Eq.~\eqref{eq:condition1} holds. 
    The eigenvalue analysis yields the following conclusions:\\
    (1) When the regulatory intensity $\upsilon$ exceeds the critical threshold $ max(min(\upsilon_{1}^{*}, \upsilon_{2}^{*}), \upsilon_{3}^{*}, \upsilon_{4}^{*} )$, the eigenvalue $\lambda_{3}(\mathscr{E}_{8})<0$.\\
    (2) Under the condition that the monetary expenditure $\pi^{'}$  is below the comprehensive effect intensity of platform regulatory mechanisms on suppliers' strategy selection $\mathcal{R}_{R} + \mathcal{F}_{R}$ (the total magnitude of reputation rewards and penalties), the eigenvalue $\lambda_{2}(\mathscr{E}_{8})<0$.\\
    (3) When the sum of the platform's reputation benefit and penalty exceeds platform's verification cost $\mathcal{C}_{P} < \mathcal{R}_{P} + \mathcal{F}_{P}$, $\lambda_{1}(\mathscr{E}_{8})<0$ is guaranteed.

    Next, we analyze the stability of the seven equilibrium points other than $\mathscr{E}_{8}$ when Eq.~\eqref{eq:condition1} holds. 
    Based on eigenvalue analysis, the following conclusions can be drawn:

    (1)  When the total magnitude of reputation rewards and penalties  $\mathcal{R}_{R} + \mathcal{F}_{R}$ exceeds the penalty cost $\pi^{'}$ , due to $\pi^{'}>\pi$,  $\mathcal{R}_{R} + \mathcal{F}_{R}>\pi$ also holds. 
    The eigenvalues $\lambda_{2}(\mathscr{E}_{1})$, $\lambda_{1}(\mathscr{E}_{2})$, $\lambda_{1}(\mathscr{E}_{3})$, $\lambda_{1}(\mathscr{E}_{5})$ of equilibrium points $\mathscr{E}_{1}$, $\mathscr{E}_{2}$,  $\mathscr{E}_{3}$,  $\mathscr{E}_{5}$ are all positive, indicating that these points are not evolutionarily stable.

    (2)  Due to $\mathcal{R}_{P} + \mathcal{F}_{P}-(1-\eta)\xi \pi^{'}<\mathcal{R}_{P} + \mathcal{F}_{P}$, when the sum of the platform's reputation benefit  and penalty $\mathcal{R}_{P} + \mathcal{F}_{P}$ exceeds platform's verification cost $\mathcal{C}_{P}$,  the first  eigenvalues ($\lambda_{1}$) of equilibrium points $\mathscr{E}_{6}$ is positive. 
         Therefore, this point do not qualify as evolutionarily stable strategies (ESS).

    (3)  When the regulatory intensity $\upsilon > max(min(\upsilon_{1}^{*}, \upsilon_{2}^{*}), \upsilon_{3}^{*}, \upsilon_{4}^{*})$, combined with the condition $\mathcal{R}_{P} + \mathcal{F}_{P}-(1-\eta)\xi \pi^{'} <\mathcal{C}_{P}$, 
         the eigenvalues $\lambda_{3}(\mathscr{E}_{4})$ and $\lambda_{3}(\mathscr{E}_{7})$ also fails to meet the ESS condition. 
    
    In summary, under the parametric constraints of Eq.~\ref{eq:condition1}, none of the seven equilibrium points (other than $\mathscr{E}_{8}(1,1,1)$) can remain stable in the long-term evolutionary process. 
    This finding suggests that only when all three parties(suppliers, the platform, and buyers) adopt trustworthy strategies can the system achieve a stable and optimal equilibrium state.
\end{proof}


%
\pagebreak
%
% Now we start the Appendixes, with the new section name, "Appendix", and a 
%  new counter, "I", "II", etc.
\appendix
%
% And now for some pretty impressive notation.  In this example, I have used
%   the tabular environment to line up the columns in ASCE style.
%   Note that this and all Appendixes (except the references) start with 
%   the \section command
%





%
% Here's the list of references:
%
% \label{section:references}
\bibliography{ascexmpl-new}
%

\end{document}
