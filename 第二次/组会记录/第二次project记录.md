# 第二次project记录
## $\color{purple}{\text{Part One : The simplfy of system}}$
$\text{Consider the complex form of the autonomous systems :}$
$$A:\dot{z} = iz+Az^2+B\bar{z}^2+Cz\bar{z}$$
$\text{The condition of A becomes a Hamiltonian system is :}$
$$2A=-\bar{C}$$
$\text{We know that :}$
$$C \coloneqq C_1 + iC_2$$
$\text{Now we do the rotation :}$
$$z\rightarrow ze^{i\alpha}\overset{\text{denote }\sigma \coloneqq e^{i\alpha}}{=}z\sigma$$
$\text{We get }A\text{ becomes :}$
$$\tilde{A}:\sigma\dot{z}=i\sigma z+A\sigma^2z^2+B\bar{\sigma}^2\bar{z}^2+C\sigma\bar{\sigma}z\bar{z}$$
$\iff$
$$\tilde{A}:\dot{z}=iz+A\sigma z^2+B\bar{\sigma}^3\bar{z}^2+\bar{\sigma}Cz\bar{z}$$
$\text{Now the condition for }\tilde{A}\text{ becomes a Hamiltonian system is :}$
$$2(\sigma A)=-(\overline{\bar{\sigma}C})$$
$\iff$
$$2A=-\bar{C}$$
>$\color{red}{\text{This tell us a fact that the condition is preseve under the rotation operation.}}$
>$\color{red}{\text{That is :}}$
>$$\color{red}{\text{We can always choose an }\sigma \text{ s.t C}\in\mathbb{R}}$$
>$\color{red}{\text{That is :}}$
>$$\color{red}{\text{Without losing generality , We can let }Im(C)=0}$$

$\text{Therefore , Let }Im(C)=0$
$\text{Then : }A\text{ becomes in }\mathbb{R}.$
$\text{So now : The system }\tilde{A}\text{ is only depended on }A_1,B_1,B_2$
$\text{We denote :}$
$$\lambda \coloneqq (A_1,B_1,B_2)$$

## $\color{purple}{\text{Part Two : The Singular }\lambda }$

>$\text{Definition 1 : }(singular)$  
>$\lambda = (A_1,B_1,B_2)$  
>$\text{Suppose that we have a Hamiltonian system }A\text{ with }H(x,y,\lambda)$
>$\text{That is :}$
>$$A:\begin{cases} \dot{x}=H_y(x,y,\lambda) \\ \dot{y}=-H_x(x,y,\lambda) \end{cases}$$
>$\text{Then we say that }\lambda\text{ is }Singular\text{ if }H(x,y,\lambda)\text{ satisfies one of the following conditions :}$
>$\color{blue}{\text{CASE } \mathrm{I} \text{ : }H(x,y,\lambda) \text{ has a degenerate critical point as a function of }(x,y)}$
>$\color{blue}{\text{That is : There }\exists (x_0,y_0) \text{ s.t } \begin{cases} H_x(x_0,y_0,\lambda)=0 \\ H_y(x_0,y_0,\lambda)=0 \\ det(HessH(x_0,y_0,\lambda))=0\end{cases}}$
>$\color{blue}{\text{CASE }\mathrm{II}\text{ : }H(x,y,\lambda)\text{ has two diffenent critical points }(x_1,y_1),(x_2,y_2) \text{ s.t } H(x_1,y_1,\lambda)=H(x_2,y_2,\lambda)}$



>$\text{Definition 2 : }(\Sigma, \Sigma_1,\Sigma_2)$  
>$\text{Given a }singular \; \lambda = (A_1,B_1,B_2)$  
>$\text{We define :}$  
>$\mathrm{i.}\; \lambda \in \Sigma_1 \iff H(x,y,\lambda) \text{ is in }\color{blue}{\text{CASE } \mathrm{I}}$  
>$\mathrm{ii.}\; \lambda \in \Sigma_2 \iff H(x,y,\lambda) \text{ is in }\color{blue}{\text{CASE } \mathrm{II}}$  
>$\mathrm{iii.} \; \Sigma \coloneqq \Sigma_1 \cup \Sigma_2$  
>$\color{green}{\text{We call : }\mathrm{i.}\;\Sigma_1  \; caustic}$  
>$\color{green}{\text{We call : }\mathrm{ii.}\; \Sigma_2 \; Maxwell \;stratum}$  
>$\color{green}{\text{We call : }\mathrm{iii.}\; \Sigma \text{ the bifurcation diagram of the family of }H(x,y,\lambda)}$  

$\text{Example : }$  
$\text{Consider } H(x) = x^4+\lambda_1x^2 + \lambda_2x$  
$\text{How to draw }\Sigma \; ?$  
$\color{red}{\mathrm{I.}(\text{About }\Sigma_1):}$  
$$\text{ let } \begin{cases} H_x = 4x^4+2\lambda_1x+\lambda_2 = 0 \\ H_{xx}= 12x^2+2\lambda_1=0 \end{cases}$$
$\overset{\text{Solve this }}{\Rightarrow}$
$$\begin{cases} \lambda_1 = -6x^2 \\ \lambda_2 = 8x^3 \end{cases}$$
$\text{This is a parameter equation about }x$
$\text{Then we can draw }\Sigma_1 \text{in }\lambda_1 \text{ axis and }\lambda_2\text{ axis !}$  
$\color{red}{\mathrm{II.}(\text{About }\Sigma_2):}$  
$\text{Suppose }x_a \text{ and } x_b$  
$$\text{let}\begin{cases} 4x_a^3+2\lambda_1x_a+\lambda_2=0 \\ 4x_b^3+2\lambda_1x_b+\lambda_2=0 \\ x_a^4+\lambda_1x_a^2+\lambda_2x_a = x_b^4+\lambda_1x_b^2+\lambda_2x_b \end{cases}$$
$\overset{\text{Solve it }}{\Rightarrow}$
$$\begin{cases} \lambda_1 <0 \\ \lambda_2=0\end{cases}$$
$\text{Then we can draw }\Sigma_2 \text{in }\lambda_1 \text{ axis and }\lambda_2\text{ axis !}$  
$\text{Therefore , the graph of }\Sigma=\Sigma_1 \cup \Sigma_2 \text{ is done !}$

$\color{green}{\text{Remark :(small trick)}}$  
$\color{green}{\text{Let }C_1=0\text{ and let }C_1=1}$

## $\color{purple}{\text{Part Three : Problem } }$

>$\text{Find and draw the bifurcation diagram }\Sigma = \Sigma_1 \cup \Sigma_2$