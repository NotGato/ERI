# ERI — Repaso de la primera parte (Unidades I a V)
## y qué de todo esto vas a necesitar en el segundo parcial

> Complementa a `GUIA_SIMPLE_PARCIAL2.md`. Las Unidades I–V no se toman en el 2º parcial,
> pero **las herramientas sí se usan todo el tiempo** en las Unidades VI–X (y entran en el final).
> Cada sección termina con un recuadro **"→ En el 2º parcial"** que dice dónde reaparece.

---

## Mapa rápido

| Unidad | Tema | Herramienta clave que te llevás |
|---|---|---|
| I | Decidir bajo riesgo / incertidumbre | utilidad esperada, equivalente cierto, prima de riesgo |
| II | Utilidad esperada y aversión al riesgo | cóncava = averso, Jensen, Arrow–Pratt, **π ≈ ½·r·σ²**, CARA–Normal |
| III | Reparto óptimo del riesgo | seguro, estados contingentes, **teorema de Borch**, riesgo agregado vs idiosincrático |
| IV | Finanzas (Markowitz, CAPM) | diversificación, covarianza, β, riesgo sistemático |
| V | Firma bajo incertidumbre (Sandmo) | la firma aversa produce menos; media–varianza |

---

## Unidad I — Decidir sin saber qué va a pasar

**Riesgo vs. incertidumbre (Knight):**
- **Riesgo** = conozco las probabilidades (dado, seguro de autos).
- **Incertidumbre** = ni siquiera conozco las probabilidades (algo único e irrepetible). Para Knight, el beneficio empresario nace de acá.

**Sin probabilidades** (matriz de pagos), cinco criterios:
| Criterio | Regla | Personalidad |
|---|---|---|
| Maximin (Wald) | el mejor de los peores | pesimista |
| Maximax | el mejor de los mejores | optimista |
| Hurwicz | α·mejor + (1−α)·peor | intermedio (α = optimismo) |
| Laplace | promedio simple (todos los estados igual de probables) | "no sé, entonces todo 1/S" |
| Minimax arrepentimiento (Savage) | minimizar el máximo "me hubiera convenido otra cosa" | evita el remordimiento |

No hay uno "correcto": sobre la misma matriz eligen cosas distintas.

**Con probabilidades → utilidad esperada:** U = Σ πₛ·v(yₛ).
- **Equivalente cierto (EC):** monto seguro que te deja igual que la lotería: v(EC) = E[v(y)].
- **Prima de riesgo:** ρ = E[y] − EC = cuánto pagarías por sacarte el riesgo.
- Ejemplo: v = 2√y, lotería (½; 1, 9): E[y] = 5; E[v] = ½·2 + ½·6 = 4 ⇒ 2√EC = 4 ⇒ **EC = 4**, prima = **1**.

**Kahneman–Tversky (lo que la gente hace de verdad):**
- **Efecto certeza** (Allais): lo seguro pesa de más.
- **Efecto reflejo**: aversos al riesgo en ganancias, **amantes del riesgo en pérdidas**.
- **Efecto aislamiento / framing**: se ignora lo común a las opciones; cómo te lo presentan cambia la elección.
- **Función de valor en S**: definida sobre **ganancias y pérdidas** respecto a un punto de referencia; cóncava en ganancias, convexa en pérdidas, **más empinada en pérdidas** (aversión a las pérdidas).
- **Ponderación de probabilidades**: probabilidades chicas pesan de más ⇒ explica a la vez que la gente compre **loterías y seguros**.
- **Cisnes negros (Taleb)** y **sesgo de optimismo**: ponen en duda que las probabilidades sean conocidas o bien calibradas.

> **→ En el 2º parcial:** el equivalente cierto y la prima de riesgo son **exactamente** lo que paga el principal por el riesgo moral. En el ejemplo de la Clase 7 el agente recibe una lotería (64 ó 9) cuyo EC es 49 = el salario fijo de info simétrica; los 4 pesos extra son **la prima de riesgo** que hay que pagarle.

---

## Unidad II — Utilidad esperada y aversión al riesgo

**¿Por qué no alcanza el valor esperado?** San Petersburgo: el juego tiene valor esperado infinito y nadie paga más que unos pesos. Bernoulli: el dinero tiene **utilidad marginal decreciente** (con ln, el juego vale 4 ducados).

**Axiomas de von Neumann–Morgenstern:** completitud y transitividad, continuidad, **independencia** (el corazón), monotonía ⇒ existe u con U = E[u].
- La utilidad vNM es **cardinal**: sólo se puede transformar como a·u + c con a > 0.
- **Allais** viola **independencia**. **Ellsberg** viola la existencia de **probabilidades subjetivas** (aversión a la ambigüedad).

**Actitud frente al riesgo:**
| u | Actitud | EC vs E[x] | Prima |
|---|---|---|---|
| cóncava (u″ < 0) | **averso** | EC < E[x] | > 0 |
| lineal | **neutral** | EC = E[x] | 0 |
| convexa | amante | EC > E[x] | < 0 |

La herramienta matemática es la **desigualdad de Jensen**: si u es cóncava, E[u(X)] < u(E[X]).

**Medidas de Arrow–Pratt:**
- **Absoluta:** r_A = −u″/u′.  **Relativa:** r_R = w·r_A.  **Tolerancia** al riesgo T = 1/r_A.
- **CARA:** u = −e^(−a·w) ⇒ r_A = a constante.
- **CRRA:** u = w^(1−R)/(1−R) (ln w si R = 1) ⇒ r_R = R constante, r_A = R/w decreciente.
- **Aproximación de Pratt:** para un riesgo chico, **prima ≈ ½ · r_A · σ²**.
- **Teorema de Pratt:** "A es más averso que B" ⇔ r_A mayor en todo w ⇔ A es una transformación cóncava de B ⇔ A paga más por evitar cualquier riesgo.
- **CARA + Normal ⇒ media–varianza:** maximizar E[u] equivale a maximizar **μ − (a/2)·σ²**.

**Demanda de seguro:** prima por unidad p, cobertura q.
- Prima **justa** (p = probabilidad del siniestro) ⇒ el averso se asegura **por completo** (q = L).
- Prima **con recargo** (p > π) ⇒ **cobertura parcial**.

> **→ En el 2º parcial:**
> - **Holmström–Milgrom (7.6)** usa justo el EC media–varianza: E[w] − (r/2)·Var(w) − costo del esfuerzo. Es la aproximación de Pratt / CARA–Normal.
> - **Jensen** es el argumento de por qué una señal **no informativa** no sirve (sólo agrega riesgo) y de por qué el principal neutral asegura al agente averso.
> - **CARA** da el contrato lineal de la Clase 6: b = r_P/(r_P + r_A) = T_A/(T_A + T_P).
> - El **seguro con prima justa ⇒ cobertura completa** es el punto de partida del ej. 6.3 y de **Rothschild–Stiglitz** (Clase 8).

---

## Unidad III — Repartir el riesgo entre varios

**La idea:** el riesgo no se destruye, **se reparte**. Y si se lo pasa a quien lo soporta mejor (o se lo diluye entre muchos), todos ganan.

**Estados de la naturaleza / ingresos contingentes:** "un peso si hay accidente" y "un peso si no hay" son **bienes distintos**.
- Curvas de indiferencia en (y₁, y₂): sobre la **línea de certeza** (y₁ = y₂) la pendiente es **−π₁/π₂** para todos.
- Comprar seguro = vender pesos del estado "sin accidente" para comprar pesos del estado "con accidente". La prima es el **precio del derecho contingente**.

**Mercados de Arrow–Debreu:** si hay un título para cada estado (**mercados completos**), el equilibrio competitivo reparte el riesgo de forma **Pareto-óptima** (1er teorema del bienestar). Si faltan mercados, no.

**Tres formas de abaratar el riesgo:**
1. **Difusión (Arrow–Lind):** si un riesgo independiente se reparte entre n personas, el costo total del riesgo → 0 (cada uno carga varianza σ²/n², la suma es σ²/n → 0). Un grupo grande actúa **como si fuera neutral**.
2. **Fondo común (pooling):** juntar riesgos independientes y repartir el promedio baja la varianza sin cambiar la media; dividir en **partes iguales** es óptimo.
3. **Diversificación:** lo mismo, pero para un solo inversor.

Base de todo: **Ley de Grandes Números** (el **promedio** se estabiliza; el **total** no).

**Riesgo idiosincrático vs. agregado:** el idiosincrático (independiente entre personas) se puede eliminar; el **agregado** no: sólo se puede repartir.

**Teorema de Borch (lo más importante de la unidad):**
- Reparto eficiente ⇔ **λᵢ·u′ᵢ(cᵢ) = λⱼ·u′ⱼ(cⱼ) en cada estado**.
- **Mutualidad:** lo que recibe cada uno depende **sólo del total** W, no de a quién le pasó qué.
- **Regla de reparto:** dcᵢ/dW = Tᵢ / ΣTⱼ ⇒ cada uno absorbe riesgo **en proporción a su tolerancia**.
- **Bajo CARA:** reparto **lineal** (Wilson): cᵢ = αᵢ·W + βᵢ con αᵢ = (1/aᵢ)/Σ(1/aⱼ).
- **Caja de Edgeworth de estados:** la curva de contrato son las tangencias. Sin riesgo agregado, es la diagonal (todos con ingreso cierto).
- Borch dice que **qué** λ se elige (cómo se reparten las ganancias) queda **indeterminado**: depende de la negociación.

> **→ En el 2º parcial, esto es el centro de la Clase 6:**
> - El contrato principal–agente con info simétrica **es** un reparto de Borch entre dos: B′(x−w)/u′(w) = λ.
> - Principal neutral ⇒ salario fijo; agente neutral ⇒ franquicia; ambos aversos ⇒ reparto por tolerancias; CARA ⇒ lineal.
> - La indeterminación de Borch se resuelve dándole **todo el poder al principal** (λ queda fijado por Ū).
> - **Mutualidad** ⇒ con info simétrica, una señal que no afecta x **se ignora**. Con riesgo moral, en cambio, vale si es informativa (Holmström).
> - **Mercados incompletos:** la información asimétrica es una causa de que falten mercados (no se puede escribir un derecho contingente sobre algo no verificable).
> - **Riesgo común vs. idiosincrático** ⇒ **evaluación relativa** (dos vendedores de paraguas con el mismo shock de lluvia).
> - **Arrow–Lind** justifica suponer **principal neutral** (accionistas diversificados).

---

## Unidad IV — Finanzas: Markowitz y CAPM

**Un activo es un paquete de derechos contingentes.** Si el inversor mira sólo media y varianza (válido con CARA–Normal o utilidad cuadrática):
- Media de la cartera: promedio ponderado. **Varianza: no**; aparecen las **covarianzas**.
- Cartera con N activos iguales: σ²_p = σ̄²/N + (1 − 1/N)·c̄ → **c̄**. El riesgo propio desaparece; **queda la covarianza** (riesgo no diversificable).

**Markowitz:** maximizar el valor esperado nunca te haría diversificar ⇒ hay que mirar también la varianza.
- **Dos activos:** ρ = +1 ⇒ no gano nada diversificando; ρ = −1 ⇒ puedo armar una cartera **sin riesgo**; en el medio, la curva se comba hacia la izquierda.
- **Frontera eficiente:** la parte de arriba de la "bala" (hipérbola). Vértice: cartera de **mínima varianza global**.

**Activo libre de riesgo + separación de Tobin:**
- Todos combinan **la misma cartera riesgosa T** (tangente) con el activo seguro; la aversión sólo cambia **cuánto** de T compran.
- **CML:** μ_p = r_f + [(μ_M − r_f)/σ_M]·σ_p. La pendiente es el **ratio de Sharpe** ("precio del riesgo").

**CAPM (Sharpe):**
- **μᵢ = r_f + βᵢ·(μ_M − r_f)**, con **βᵢ = Cov(rᵢ, r_M)/Var(r_M)**. Su gráfico es la **SML**.
- Riesgo total = **sistemático** (βᵢ²·σ²_M) + **no sistemático** (σ²_ε).
- **Sólo se paga el riesgo sistemático**: el otro lo elimino gratis diversificando.

**Futuros:** contrato estandarizado para comprar o vender en T a precio F₀; **cobertura** (reducir riesgo) vs **especulación** (tomarlo). Costo de acarreo: F₀ = S₀·e^((r+u−y)T). **Contango** F₀ > S₀; **backwardation** F₀ < S₀. Cobertura de mínima varianza: h* = Cov(ΔS, ΔF)/Var(ΔF) (es un β).

**Puente con Unidad III:** precio de un activo = E[m·x] (núcleo estocástico). El CAPM es el caso en que m es lineal en el rendimiento del mercado.

> **→ En el 2º parcial:** es la unidad menos usada. Te sirve la idea de **filtrar el ruido común** (como el β aísla el componente de mercado): eso es la **evaluación relativa** de Holmström. Y la frase "**sólo se remunera el riesgo que no se puede evitar**" ayuda a entender por qué el principal neutral (diversificado) asegura al agente.

---

## Unidad V — La firma competitiva cuando no sabe el precio (Sandmo)

**Planteo:** la firma decide cuánto producir **antes** de conocer el precio p (aleatorio, media μ). Maximiza E[U(px − C(x) − B)].

**Producto de certeza x_c:** el que elegiría si p = μ seguro ⇒ C′(x_c) = μ.

| Firma | Regla | Producción |
|---|---|---|
| Neutral | C′(x) = μ | x = x_c |
| **Aversa** | **C′(x*) < μ** | **x* < x_c** (se "autocubre" produciendo menos) |
| Media–varianza (Markowitz) | C′(x) = μ − ρσ²x | **x* = μ/(c + ρσ²)** con C = (c/2)x² |

- Ejemplo: μ = 10, c = 1, ρ = 1, σ² = 1 ⇒ x_c = 10, **x* = 5**. La brecha μ − C′(x*) = ρσ²x* = 5 es la **prima marginal de riesgo**.
- Más varianza o más aversión ⇒ menos producción.

**Neutralidades que se rompen con incertidumbre:**
- **Costos fijos importan:** con **DARA** (aversión absoluta decreciente), subir B reduce x. (Con media–varianza/CARA no importan.)
- **Impuesto proporcional:** sube, no cambia o baja x según que la aversión **relativa** sea creciente, constante o decreciente.
- **Oferta con pendiente positiva:** DARA alcanza (descomposición tipo Slutsky).
- **Largo plazo:** la firma aversa exige **beneficio esperado positivo** (μ > costo medio) ⇒ **el beneficio es el pago por soportar riesgo**. Las firmas menos aversas producen más y pueden concentrar el mercado.

> **→ En el 2º parcial:** misma lógica que el agente averso en riesgo moral: **cuanto más riesgo cargás, menos te esforzás o producís**, y el que es menos averso es el que conviene que cargue el riesgo (franquicia). La forma **media–varianza** es la misma que en Holmström–Milgrom.

---

## Resumen de una línea por herramienta (la "caja" que llevás al 2º parcial)

| Herramienta (Unidad) | Dónde aparece en VI–X |
|---|---|
| Equivalente cierto / prima de riesgo (I–II) | costo del riesgo moral = prima de riesgo al agente (VII) |
| Cóncava ⇔ averso; Jensen (II) | salario fijo con principal neutral (VI); señal no informativa no sirve (VII) |
| Arrow–Pratt, tolerancia T = 1/r (II) | b = T_A/(T_A + T_P) (VI) |
| π ≈ ½ r σ², CARA–Normal (II) | Holmström–Milgrom, B* = 1/(1 + rσ²) (VII) |
| Seguro: prima justa ⇒ cobertura total (II–III) | ej. 6.3; Rothschild–Stiglitz (VIII); señalización en seguros (IX) |
| Pendiente −π₁/π₂ sobre la línea de certeza (III) | gráficos (w_F, w_S) de VII y VIII; cruce único |
| **Teorema de Borch**, mutualidad, tolerancias (III) | **todo el modelo básico de la Clase 6** |
| Caja de Edgeworth de estados (III) | caja principal–agente (VI) |
| Mercados completos ⇒ Pareto (III) | info asimétrica = mercados incompletos (VI) |
| Riesgo agregado vs idiosincrático (III–IV) | evaluación relativa, torneos (VII) |
| Arrow–Lind (III) | por qué suponer principal neutral (VI–VII) |
| Sandmo: más aversión ⇒ menos producción (V) | trade-off seguro–incentivos (VII) |
