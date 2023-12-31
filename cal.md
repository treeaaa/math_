Proof. Let A be an  $n * m$ matrix and B be an $m * n$ matrix over C.Show that $I_{n} - AB$ is invertible if and only if $I_{m} - BA$ is invertible.

思路: invertible 說明反矩陣存在，假設 $\exists C_{n},C_{n}$ 是 $I_{n} - AB$的反矩陣，所以會有 $$C_{n}(I_{n} - AB)=I_{n}$$
接下來，我需要把BA湊出來所以把兩邊同乘以A $$C_{n}(I_{n} - AB)A=I_{n}A$$
$$C_{n}(A - ABA)=A$$
$$C_{n}(AI_{m} - ABA)=A$$
$$C_{n}A(I_{m} - BA)=A$$
然後我需要讓等式的右邊變成 $I_{m}$, A 是一個non-square matrix，所以不能乘上 $A^{-1}$ , 而是要乘上 $B$
$$BC_{n}A(I_{m} - BA)=BA$$
$$I_{m} + BC_{n}A(I_{m} - BA)=I_{m} +BA$$
$$I_{m} - BA + BC_{n}A(I_{m} - BA)=I_{m} $$
$$I_{m}(I_{m} - BA) + BC_{n}A(I_{m} - BA)=I_{m} $$
$$(I_{m}+ BC_{n}A)(I_{m} - BA)=I_{m} $$


這樣就把 $I_{m} - BA$的反矩陣湊出來了 $(I_{m}+ BC_{n}A)$
