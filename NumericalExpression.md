$$
    \bm{x} = (x, y, \theta)^{\mathrm{T}}
$$  

$$
    \bm{q} = (q_x, q_y)^{\mathrm{T}}
$$  

$$
    \bm{z} = (z_x, z_y)^{\mathrm{T}}
$$  

$$
    \bm{a} = (\Delta d, 0, \Delta \psi)^{\mathrm{T}}
$$  

$$
  R = \left(
    \begin{array}{ccc}
      cos\theta & -sin\theta \\
      sin\theta & cos\theta \\
    \end{array}
  \right)
$$  

$$
    \bm{t} = (x, y)^{\mathrm{T}}
$$  

$$
    \bm{q} = Rz + t
$$  

$$
  \left(
    \begin{array}{ccc}
      x_i \\
      y_i \\
      \theta_i
    \end{array}
  \right)
   = \left(
    \begin{array}{ccc}
      cos\theta_{i-1} & -sin\theta_{i-1} & 0 \\
      sin\theta_{i-1} & cos\theta_{i-1} & 0 \\
      0 & 0 & 1
    \end{array}
  \right)
  \left(
    \begin{array}{ccc}
      \Delta d_{i-1} \\
      0 \\
      \Delta \psi_{i-1}
    \end{array}
  \right) +
  \left(
    \begin{array}{ccc}
      x_{i-1} \\
      y_{i-1} \\
      \theta_{i-1}
    \end{array}
  \right)
$$  

$$
    \bm{x}_i = \bm{x}_{i-1} \oplus \bm{a}_{i-1}
$$  

$$
    \bm{q}_1 = R_1 z_1 + t_1
$$  

$$
    \bm{q}_2 = R_1 z_2 + t_1
$$  

$$
    \bm{q}_2 = R_2 z_3 + t_2
$$  

$$
    \bm{q}_3 = R_2 z_4 + t_2
$$  

$$
    \bm{q}_3 = R_3 z_5 + t_3
$$  

$$
    \bm{q}_4 = R_2 z_6 + t_3
$$  

$$
    \bm{x}_2 = \bm{x}_{1} \oplus \bm{a}_{1}
$$  

$$
    \bm{x}_3 = \bm{x}_{2} \oplus \bm{a}_{2}
$$  