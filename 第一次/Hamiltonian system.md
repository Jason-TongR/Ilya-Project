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
$$div V = 0 \iff A \; is \; a \; Hamiltonian \;system$$


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
\mu \coloneqq (A1,A2,B1,B2,C1,C2)
$$
Find the condition of $\mu$ such that $\tilde{A}$ is a $Hamiltonian \; system.$



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
Then we define the $divV \coloneqq{} \frac{\partial P}{\partial x} + \frac{\partial Q}{\partial y}$ 

    We want to show that $div V = 0$
    So  $div V \overset{by\;definition}{=} \frac{\partial P}{\partial x} + \frac{\partial Q}{\partial y} \overset{hypothesis}{=}H_{yx} + (-H_{xy}) \overset{H \; is\;in \;C^2}{=} 0$
    Done
    $\\$
    $(\Rightarrow):$
    We have the hypothesis that $divV = \frac{\partial P}{\partial x} + \frac{\partial Q}{\partial y} = 0$

    >We need to introduce some definitions first:
    >>Definiton 1 ($1-form$):
     We say that $w$ is a $1-form \;$if $ w = A(x,y)dx + B(x,y)dy \;    \\where \;A , B : \mathbb{R}^2 \rightarrow \mathbb{R}$ are fucntions.
     $\\$
     $\\$
     >>Definition 2($Exact form$):
     Given a $1-form \; w = A(x,y)dx+B(x,y)dy  $
     we say $w$ is $exact\;$ if $\; w=dH \; for\;some \;H$
     Where $dH \coloneqq \frac{\partial H}{\partial x}dx + \frac{\partial H}{\partial y}dy$








- ### Answer of Question 2 :





