# <span style="color: red;">MISSION 1</span>

## <span style="color: purple;">The Questions</span>

- ### Question 1
    >Consider the two dimensional autonomous system :
$$
A:\begin{cases}
\dot{x} = P(x,y)\\
\dot{y} = Q(x,y)
\end{cases}
$$
Suppose our domain is simply connected , Is the following statment correct?
$$div V = 0 \iff A\text{ is a }Hamiltonian \;system$$


- ### Question 2
    >Suppose we have the two dimensional autonomous system :
$$
A:\begin{cases}
\dot{x} = P(x,y)\\
\dot{y} = Q(x,y)
\end{cases}
$$
And the complex form of A is given by:
$$
\tilde{A} : \; \dot{z} = iz + Az^2 + B\bar{z}^2 + Cz\bar{z}
$$
Supoose :
$$
A \coloneqq A_1 + iA_2\\
B \coloneqq B_1 + iB_2\\
C \coloneqq C_1 + iC_2\\
\mu \coloneqq (A_1,A_2,B_1,B_2,C_1,C_2)
$$
Find the condition of $\mu$ such that $\tilde{A}$ is a $Hamiltonian \; system.$


*********
## <span style="color: purple;">The Answers</span>

- ### Answer of Question 1 :
    >YES , it is correct.

    PROOF:
    $\\$
    $(\Leftarrow):$
 We have the hypothesis that $A \; is \; a \;Hamiltonian \;system$ 
that is $\exist \; H:\mathbb{R}^2 \rightarrow \mathbb{R} \; and \;H\in C^2(\mathbb{R}^2) \;such\;that \begin{cases}
P(x,y) = H_y\\
Q(x,y) = -H_x
\end{cases}$
Now , we have the definiton of $div V:$
    >$Definiton$ : Suppose we have the two dimensional autonomous system :
$$
A:\begin{cases}
\dot{x} = P(x,y)\\
\dot{y} = Q(x,y)
\end{cases}
$$
$\text{Then we define the }divV \coloneqq{} \frac{\partial P}{\partial x} + \frac{\partial Q}{\partial y}$ 

    We want to show that $div V = 0$
    So  $div V \overset{by\;definition}{=} \frac{\partial P}{\partial x} + \frac{\partial Q}{\partial y} \overset{hypothesis}{=}H_{yx} + (-H_{xy}) \overset{H \; is\;in \;C^2}{=} 0$
    $\square$
    $\\$
    $(\Rightarrow):$
    >We need to introduce some definitions first:
        >>$\text{Definiton 1} (1-form):$
        We say that $w$ is a $1-form \;\text{if } w = A(x,y)dx + B(x,y)dy \;    \\where \;A , B : \mathbb{R}^2 \rightarrow \mathbb{R}$ are fucntions.
        $\\$
        $\\$
        >>$\text{Definiton 2}(Exact \; form):$
        Given a $1-form \; w = A(x,y)dx+B(x,y)dy  $
        we say $w$ is $exact\;\text{ if }\; w=dH \; for\;some \;H$
        Where $dH \coloneqq \frac{\partial H}{\partial x}dx + \frac{\partial H}{\partial y}dy$
        $\\$
        $\\$
        >>$\text{Definiton 3}(Closed \; form):$
        Given a $1-form \; w = A(x,y)dx+B(x,y)dy$ we say that $w$ is closed
        $\text{if}$
        $dw = 0 \\(\text{where }dw \coloneqq dA \wedge dx + dB\wedge dy = (A_xdx + A_ydy)\wedge dx + (B_xdx+B_ydy)\wedge dy = (B_x-A_y)dx\wedge dy)$

    >$\text{Theorem}(Poincare\;lemma):$
    Given a $1-form\;w\coloneqq A(x,y)dx + B(x,y)dy$ and the domain of $A,B$ are simply connected.
    Then
    $w\text{ is } exact \iff w \text{ is } closed$

    Now back to our proof, We have the hypothesis that $divV = \frac{\partial P}{\partial x} + \frac{\partial Q}{\partial y} = 0$
    We want to find $H \text{ such that } H_y=P \text{ and } -H_x=Q.$

    $\text{Since } dH = H_xdx + H_ydy = -Qdx + Pdy $
    $$\text{So } \exist H \iff w \coloneqq -Qdx+Pdy \text{ is } exact \tag{*} $$
    $\text{Now compute } dw:\\w \coloneqq -Qdx+Pdy \Rightarrow dw= (P_x + Q_y)dx\wedge dy \overset{\text{hypothesis}}{=} 0dx\wedge dy = 0\\ \text{So } w \text{ is } closed \\ \text{by } Poincare \; lemma \text{ , we konw that }w \text{ is } exact \text{ , then by } (*) \text{ we konw that } \exist H$
    That is , the system is $Hamiltonian.$ 
    $\square$
- ### Answer of Question 2 :
    >$\text{The condition is : }2A = -\bar{C} \text{ and }B \text{ is free.} $

    $\text{We know that all two dimensional autonomous system can be writen as the complex form :}$
    $$\dot{z}=iz+Az^2+B\bar{z}^2+Cz\bar{z} \tag{*}$$
    $\text{where}$
    $$A\coloneqq A_1+iA_2$$
    $\text{Now we try to change this complex form into the original form}$
    $\text{Supoose}$
    $$z\coloneqq x+iy$$
    $\text{Then } (*) \text{ is equal to } $
    $$\dot{z} \coloneqq \dot{x}+i\dot{y} = i(x+iy) + A(x+iy)^2+B(x-iy)^2+C(x+iy)(x-iy)$$
    $\Rightarrow$
    $$\dot{z} = i(x+iy)+(A_1+iA_2)(x^2-y^2+2xyi)+(B_1+iB_2)(x^2-y^2-2xyi) +(C_1+iC_2)(x^2+y^2)$$
    $\Rightarrow$
    $$\dot{z} \overset{\text{after simplify}}{=} (-y+(A_1+B_1)(x^2-y^2)+(2B_2-2A_2)xy+C_1(x^2+y^2)) \\\;\;\;\;\;\;\;\;\;\;\;\;\;\;\;+i(x+(2A_1-2B_1)xy+(A_2+B_2)(x^2-y^2)+C_2(x^2+y^2))$$

    $\text{Now we have the original form :}$
    $$\begin{cases}
    \dot{x}=-y+(A_1+B_1)(x^2-y^2)+(2B_2-2A_2)xy+C_1(x^2+y^2)\\
    \dot{y}=x+(2A_1-2B_1)xy+(A_2+B_2)(x^2-y^2)+C_2(x^2+y^2)
    \end{cases}$$

    $\text{Now compute the }divV = \frac{\partial P}{\partial x}+\frac{\partial Q}{\partial y} = (2(A_1+B_1)x+(2B_2-2A_2)y+2C_1x)+((2A_1-2B_1)x-2(A_2+B_2)y+2C_2y)$
    $\\$
    $\text{In Question 1 , We konw that :}$
    $$div V = 0 \iff A\text{ is a }Hamiltonian \;system$$
    $\text{Let }divV=0 \text{ ,Then we have :}$
    $$divV = (4A_1+2C_1)x+(-4A_2+2C_2)y=0 \;\;\;\;\forall x,y$$
    $\text{So we have :}$
    $$\begin{cases}
        4A_1+2C_1=0\\
        -4A_2+2C_2=0
    \end{cases}$$
    $\Rightarrow$
    $$\begin{cases}
        2A_1=-C_1\\
        2A_2=C_2
    \end{cases}$$
    $\text{That is :}$
    $$2A=-\bar{C} \\B \text{ is free}$$
    $\square$






