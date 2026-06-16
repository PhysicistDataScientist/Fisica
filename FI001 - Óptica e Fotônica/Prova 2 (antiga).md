# Questão 1
Considere o modo TE em um guia de onda cuja propagação ocorra na direção z com dependência em z e em t da forma $e^{(kz - \omega t)}$. Escreva as expressões para as componentes pertinentes dos campos elétrico e magnético, considerando $\Psi(x, y)$ como solução para a equação de Helmholtz cargas e correntes livres.
## Resolução

Considerando a equação de Helmholtz do enunciado e a separação das componentes longitudinais e transversais do campo, é possível calcular as componentes transversais a partir das longitudinais, precisando resolver apenas a Equação de Helmholtz que se aplica para $\Psi(x,y)$ representando $E_{z}$ ou $B_{z}$. Para o modo transversal elétrico (TE), tem-se $E_{z} = 0$, bastando resolver a Equação de Helmholtz para $B_{z}$. Para dentro do guia, $$ (\nabla_{t}^2 + \gamma^2 ) B_{z}(x,y) = 0 \Leftrightarrow \frac{\partial^2 B_{z}}{\partial x^2} + \frac{\partial^2 B_{z}}{\partial y^2} + \gamma^2 B_{z} = 0,$$
em que $\gamma \equiv \sqrt{ \frac{n_{D}^2 \omega^2}{c_{0}^2} - k^2 }$.
 Suponha uma solução do tipo separável, isto é, $B_{zD}(x, y) = X_D(x) Y_D(y)$, logo a equação diferencial parcial (EDP) se torna $$X_D''(x) Y_D(y) + X_D(x) Y_D''(y) + \gamma^2 X_D(x) Y_D(y) = 0.$$
Descartando as soluções do tipo $X_D(x) = 0$ ou $Y_D(y) = 0$, o que levaria a um campo $B_{zD} = 0$, resultando em um modo TEM, no entanto este modo só é possível se tivermos os vetores de campo elétrico e magnético nulos. Desta forma, dividimos ambos lados da EDP por $B_{zD}$, assim $$\frac{X_D''(x)}{X_D(x)} + \frac{Y_D''(y)}{Y_D(y)} + \gamma^2 = 0.$$
Esta EDP só é satisfeita para $\frac{X_D''(x)}{X_D(x)} = C_{x_{D}}$ e $\frac{Y_D''(y)}{Y_D(y)} = C_{y_{D}}$, com $C_{x,y;D} \in \mathbb{R}$. Para obter soluções oscilatórias dentro do guia, considera-se $C_{\alpha_{D}} = - k_{\alpha_{D}}^2 < 0, \ \forall \alpha \in {x,y}$. Resolver a EDO acima se traduz em solucionar as seguintes EDPs desacopladas $$X_D''(x) + k_{x_{D}}^2 X_D(x) = 0 \quad \text{e} \quad Y_D''(y) + k_{y_{D}}^2 Y_D(y) = 0,$$
as quais são EDPs de osciladores harmônicos e as soluções são dadas por $$X_D(x) = A_{x_{D}} \cos(k_{x_{D}}x) + B_{x_{D}} \sin(k_{x_{D}} x) \quad \text{e} \quad Y_D(y) = A_{y_{D}} \cos(k_{y_{D}} y) + B_{y_{D}} \sin(k_{y_{D}} y),$$
além de os números de onda $k_{x,y;D}$ estarem restritos por $k_{xD}^2 + k_{yD}^2 = \gamma^2$.
Portanto, a solução geral para $B_{z_{D}}$ é dada por $$B_{z_{D}}(x, y) = \left[A_{x_{D}} \cos(k_{x_{D}}x) + B_{x_{D}} \sin(k_{x_{D}} x)\right] \left[A_{y_{D}} \cos(k_{y_{D}} y) + B_{y_{D}} \sin(k_{y_{D}} y)\right].$$
A primeira 
Para fora do guia, vale $$ (\nabla_{t}^2 - \beta^2 ) B_{z}(x,y) = 0,$$
em que $\beta \equiv \sqrt{ k^2 - \frac{n_{F}^2 \omega^2}{c_{0}^2}}$. De maneira análoga, supondo solução separável $B_{zF}(x, y) = X_F(x) Y_F(y)$, deve-se resolver as EDPs $$\frac{X_F''(x)}{X_F(x)} + \frac{Y_F''(y)}{Y_F(y)} - \beta^2 = 0.$$
Como espera-se obter soluções que decaiam fora do guia, escolhe-se $C_{\alpha_{F}} = k_{\alpha_{F}}^2$, desta forma  deve-se resolver as EDPs $$X_{F}''(x) - k_{x_{F}}^2 X_{F}(x) = 0 \quad \text{e} \quad Y_{F}''(y) - k_{y_{F}} Y_{F}(y) = 0$$ com a restrição $k_{x_{F}}^2 + k_{y_{F}}^2 = \beta^2$. 
As soluções para $X_{F}(x)$ e $Y_{F}(y$) são dadas por $$X_{F}(x) = A_{x_{F}} e^{k_{x_{F}} x} + B_{x_{F}} e^{-k_{x_{F}} x} \quad \text{e} \quad Y_{F}(y) = A_{y_{F}} e^{k_{y_{F}} y} + B_{y_{F}} e^{-k_{y_{F}} y},$$
resultando na solução geral para $B_{z_{F}}$ dada por $$B_{z_{F}}(x,y) = \left[A_{x_{F}} e^{k_{x_{F}} x} + B_{x_{F}} e^{-k_{x_{F}} x}\right] \left[A_{y_{F}} e^{k_{y_{F}} y} + B_{y_{F}} e^{-k_{y_{F}} y}\right].$$
Sabe-se que os campos $\vec{E}$ e $\vec{B}$ devem respeitar as condições de contorno $$\left\{\begin{array}{l} \hat{n} \times (\vec{E}_{F} - \vec{E}_{D}) = 0 \Rightarrow E_{t_F} = E_{t_D}\\ \hat{n} \cdot (\epsilon_{F} \vec{E}_{F} - \epsilon_{D} \vec{E}_{D}) = \sigma_{free} \\ \\
\hat{n} \times \left(\frac{\vec{B}_{F}}{\mu_{F}} - \frac{\vec{B}_{D}}{\mu_{D}}\right) = \vec{K}_{free} \\ \hat{n} \cdot (\vec{B}_{F} - \vec{B}_{D}) = 0 \Rightarrow B_{n_{F}} = B_{n_{D}}. \end{array}\right.$$
Para este caso específico $\sigma_{free} = 0$ e $\vec{K}_{free} = \vec{0}$, logo $\frac{B_{t_{F}}}{\mu_{F}} = \frac{B_{t_{D}}}{\mu_{D}}$ e $\epsilon_{F} E_{n_{F}} = \epsilon_{D} E_{n_{D}}$. Considerando a região dentro e fora do guia como meios não magnéticos, vale $\mu_{F} = \mu_{0_{F}}$ e $\mu_{D} = \mu_{0_{D}}$. Por definição $n = \sqrt{ \epsilon_{r} \mu_{r}}$, logo para meios os meios não magnéticos $\epsilon_{r} = n^2$. Portanto, as condições de contorno para este caso em particular se resumem a $$\left\{ \begin{array}{l} E_{t_{F}} = E_{t_{D}} \\ n_{F}^2 E_{n_{F}} = n_{D}^2 E_{n_{D}} \\ \frac{B_{t_{F}}}{\mu_{0_{F}}} = \frac{B_{t_{D}}}{\mu_{0_{D}}} \\ B_{n_{F}} = B_{n_{D}}. \end{array} \\
\right.$$
Para aplicar estas condições de contorno e obter a expressão completa para $B_{z}$, é preciso conhecer a forma do guia. Uma vez conhecida a expressão para $B_{z}$, é possível obter as demais componentes dos campos elétricos e magnéticos usando  
$$E_{z_{D}} = 0, \quad E_{x_{D}} = \frac{i \omega}{\gamma^2} \frac{\partial B_{z_{D}}}{\partial y}, \quad E_{y_{D}} = -\frac{i \omega}{\gamma^2} \frac{\partial B_{z_{D}}}{\partial x}, \quad B_{x_{D}} = -\frac{ik}{\gamma^2} \frac{\partial B_{z_{D}}}{\partial x} \quad \text{e} \quad B_{y_{D}} = \frac{ik}{\gamma^2} \frac{\partial B_{z_{D}}}{\partial y},$$ as quais são válidas para um modo TE dentro do guia.
Já para a região de fora, basta substituir $\gamma^2$ por $-\beta^2$, obtendo $$E_{z_{F}} = 0, \quad E_{x_{F}} = -\frac{i \omega}{\beta^2} \frac{\partial B_{z_{F}}}{\partial y}, \quad E_{y_{F}} = \frac{i \omega}{\beta^2} \frac{\partial B_{z_{F}}}{\partial x}, \quad B_{x_{F}} = \frac{ik}{\beta^2} \frac{\partial B_{z_{F}}}{\partial x} \quad \text{e} \quad B_{y_{F}} = -\frac{ik}{\beta^2} \frac{\partial B_{z_{F}}}{\partial y}. \ \square$$
# Questão 2
Num guia de onda dielétrico, determina-se $\gamma$ definido como $\gamma \equiv \sqrt{ \frac{n_{D}^2 \omega^2}{c_{0}^2} - k^2 }$ . Considere uma frequência $\omega$ e índice de refração do guia como $n_{D}$. Portanto, obtenha o índice de refração efetivo do guia.
## Resolução
Note que pode-se reescrever o parâmetro $\gamma$ como $$\gamma \equiv \sqrt{ \frac{(n_{D}^2 - n_{eff}^2) \omega^2}{c_{0}^2} },$$
em que define-se $n_{eff} = \frac{c_{0} k}{\omega}$. Desta forma, dado o parâmetro $\gamma$ é possível obter $n_{eff}$ por meio de $$n_{eff} = \sqrt{ n_{D}^2 - \left(\frac{c_{0} \gamma}{\omega}\right)^2 }.$$
# Questão 3
O espectro de uma cavidade ressonante é dado por $f(\omega) = \frac{A}{1 + C(\omega - \omega_0)^2}$. (a) Qual é o fator de qualidade da cavidade em $\omega_0$? (b) Qual é o tempo de vida fotônico nesta mesma frequência?
## Resolução
*(a)* Para um espectro de cavidade ressonante em forma de lorentziana, sabe-se que ele é da forma $$|\tilde{\phi}(r, t)|^2 \propto \frac{|f(r)|^2}{1 + \left(\frac{\omega - \omega_n}{\omega_{n} / (2Q)}\right)^2} \equiv f(\omega) = \frac{A}{1 + C(\omega-\omega_{0})^2},$$
assim pode-se identificar $A = |f(r)|^2$ e $C = \left(\frac{2Q}{\omega_{n}}\right)^2$, ou seja, $Q = \frac{\omega_{n}}{2} \sqrt{C}$, considerando $C > 0$. 
Portanto, para a frequência de ressonância $\omega_{0}$, obtém-se $Q = \frac{\omega_{0}}{2}\sqrt{C}. \quad \square$
*(b)*  Por definição, $Q \equiv \omega_{n} \tau_{p}$. Assim, o tempo de vida fotônico para a n-ésima ressonância dentro da cavidade é dado por $\tau_{p} = Q / \omega_{n}$. Logo, para $\omega_{0}$, tem-se $\tau_{p} = Q / \omega_{0}$. Substituindo a expressão para $Q$ obtida no item anterior, obtém-se $\tau_{p} = \frac{\sqrt{ C }}{2}. \quad \square$  
#  Questão 4
Considere um feixe gaussiano centrado em $z = 0$, com comprimento de onda $\lambda$ e comprimento de Rayleigh igual a $z_0 = a$. Obtenha (a) a cintura do feixe em $z = 0$; (b) o raio de curvatura da frente de onda $R$ em $z = a$, ou seja, na extremidade da zona de Rayleigh; (c) se este feixe fosse inserido em uma cavidade simétrica de comprimento $L = 4a$, qual deveria ser o raio de curvatura dos espelhos para haver o casamento modal?
## Resolução
*(a)* Deseja-se saber a cintura do feixe em seu centro $z = 0$, ou seja, deseja-se calcular o valor de $\omega_{0}$. Partindo de $\omega_{0} = \sqrt{ \frac{\lambda z_{0}}{\pi} }$, em que é necessário conhecer apenas o comprimento de onda do feixe e o parâmetro de Rayleigh. Considerando $\lambda$ e $z_{0} = a$, obtém-se $\omega_{0} = \sqrt{ \frac{\lambda a}{\pi}}$ como a cintura mínima do feixe.
*(b)* A partir da expressão para o raio de curvatura do feixe $$R(z) = z\left[1 + \left(\frac{z_{0}}{z}\right)^2\right] = z\left[1 + \left(\frac{a}{z}\right)^2\right],$$
é possível calcular $R(a) = 2a$.
*(c)* Se a cavidade em que o feixe será inserido possui comprimento total $L = 4a$, logo possui $\frac{L}{2} = 2a$ à direita e à esquerda do centro $z = 0$, definindo a posição dos espelhos como $z_{2} = -z_{1} = 2a$, logo $R(2a) = 2a \frac{5}{4} = \frac{5}{2}a$. Considerando dois espelhos côncavos e a convenção de sinal de Siegman, $R(z_{1}) > 0$ e $R(z_{2}) < 0$, obtém-se $R(z_{1}) = R(2a) = \frac{5}{2}a$ e $R(z_{2}) = -R(2a) = -\frac{5}{2}a$ . Isto define uma cavidade na configuração mostrada na figura abaixo.

![[Teste 2 (antigo) - Esquema Q4.png]]











