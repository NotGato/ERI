# ERI — Segundo parcial (Unidades VI a X) explicado fácil

> Guía armada a partir de las notas de clase 6–10 y de la guía de estudio del parcial
> (todo está en `material/`). La idea es entender **la lógica** primero; las fórmulas salen solas.

---

## 0. El mapa de todo el parcial en un minuto

Toda la segunda parte de la materia es **una sola historia**:

> Alguien (el **principal**) contrata a alguien (el **agente**). El agente **sabe algo** que el principal no.
> ¿Qué contrato le conviene ofrecer al principal?

Lo único que cambia de unidad a unidad es **qué** se ignora y **cuándo**:

| Unidad | Nombre | ¿Qué no sabe el principal? | ¿Cuándo? | ¿Quién mueve primero? | Solución típica |
|---|---|---|---|---|---|
| VI | Info simétrica (punto de referencia) | nada | — | P | Borch: el neutral asegura al averso |
| VII | **Riesgo moral** | lo que el agente **hace** (esfuerzo) | **después** de firmar | P (contrato) | pagar según el resultado (incentivos) |
| VIII | **Selección adversa** | **quién es** el agente (su tipo) | **antes** de firmar | P (ofrece un **menú**) | menú autoseleccionable |
| IX | **Señalización** | quién es la parte informada | **antes** de firmar | **el informado** (manda una señal) | acción costosa que sólo le conviene al "bueno" |
| X | **Subastas** | cuánto valoran los compradores | antes | el vendedor fija reglas | hacer competir a los que saben |

**Truco para clasificar (ejercicio 6.1 y 10.8e):**
1. ¿La asimetría aparece **después** de firmar? → **riesgo moral** (acción oculta si es un esfuerzo; información oculta si el agente se entera de algo después de firmar).
2. ¿Aparece **antes** y el **no informado** diseña el contrato? → **selección adversa** (screening).
3. ¿Aparece **antes** y el **informado** hace algo costoso para mostrarse? → **señalización**.

Ejemplos de 6.1 resueltos:
- (a) No ve si el asegurado pone la alarma → **riesgo moral, acción oculta**. P = aseguradora, A = asegurado.
- (b) El banco no sabe la probabilidad de éxito del proyecto → **selección adversa**. P = banco.
- (c) Posgrado no relacionado en el CV → **señalización** (agente señala).
- (d) Gerente ya contratado conoce la demanda → **riesgo moral, información oculta**.
- (e) Regulador no conoce costos → **selección adversa**. P = regulador, A = empresa.
- (f) Garantía de 3 años → **señalización por el principal** (el vendedor informado usa el contrato como señal).

---

## 1. Unidad VI — El punto de partida: información simétrica

### La idea en una frase
Si todos saben lo mismo, el contrato sólo sirve para **repartir el riesgo**: **el que no le teme al riesgo se lo carga al que sí le teme.**

### Conceptos
- **Variable verificable**: se puede ver **y probar ante un juez**. Sólo eso puede ir en un contrato. Si algo no es verificable, "faltan mercados".
- **Principal**: diseña el contrato y lo ofrece "tómelo o déjelo" (tiene todo el poder).
- **Agente**: acepta si gana al menos su **utilidad de reserva Ū** (lo que tendría en su mejor alternativa).
- **Restricción de participación (PC)**: E[u(w)] − v(e) ≥ Ū. En el óptimo **se satura** (el principal no le deja "de más").
- Se resuelve **hacia atrás**: (1) qué esfuerzo elige el agente, (2) si acepta, (3) qué contrato ofrece P.

### Condición de eficiencia = Teorema de Borch (de la Clase 3)
B′(x − w) / u′(w) = λ **igual en todos los resultados**.

Traducción: el cociente de "cuánto le duele perder un peso" a cada uno es el mismo en todos los estados. De ahí salen **tres casos** (esto se pregunta siempre):

| Caso | Contrato | Por qué |
|---|---|---|
| Principal **neutral**, agente **averso** | **Salario fijo**: w = u⁻¹(Ū + v(e)) | el neutral asegura completamente al averso |
| Agente **neutral**, principal **averso** | **Franquicia**: w = x − k, con k = E[x] − Ū − v(e) | el agente "compra el negocio" y se queda con todo el riesgo |
| **Ambos aversos** | se reparten: dw/dx = r_P/(r_P + r_A) | cada uno carga riesgo según su **tolerancia** |

**Bajo CARA** (u = −e^(−rw)) el contrato es **lineal**: w = c + b·x con **b = r_P/(r_P + r_A) = T_A/(T_A + T_P)**.
- r_A → 0 (agente neutral) ⇒ b → 1 ⇒ franquicia.
- r_P → 0 (principal neutral) ⇒ b → 0 ⇒ salario fijo.
- ∂b/∂r_A < 0 (más averso el agente, menos riesgo le doy); ∂b/∂r_P > 0.
- Ej: r_A = 3, r_P = 1 ⇒ b = 1/4.

### Esfuerzo óptimo con info simétrica
- Con 2 niveles de esfuerzo: **no derivás, comparás** el beneficio de pedir e_H vs e_L.
- Continuo, principal neutral: Σ p′ᵢ(e)·xᵢ = v′(e)/u′(w). Condición suficiente: Σ p″ᵢ(e)·xᵢ ≤ 0 (rendimientos decrecientes del esfuerzo). Ej. p_S(e) = e/(1+e) ⇒ p_S″ = −2/(1+e)³ < 0 ✓.

### Ejercicio 6.2 resuelto (x ∈ {0,60}; p_H=3/4, p_L=1/4; u=√w; v(e_H)=1, v(e_L)=0; Ū=3)
- (a) Principal neutral + agente averso ⇒ Borch dice salario fijo (lo aseguro).
- (b) w(e_H) = (3+1)² = **16**; w(e_L) = 3² = **9**.
- (c) Beneficio con e_H: 0,75·60 − 16 = **29**; con e_L: 15 − 9 = 6 ⇒ pide **e_H**, gana 29.
- (d) Si el esfuerzo no es verificable y paga 16 fijo: el agente con e_H tiene 4−1=3, con e_L tiene 4−0=4 ⇒ **elige e_L**. Beneficio: 15 − 16 = **−1**. (¡El seguro completo mata los incentivos!)
- (e) Agente neutral: franquicia k = 45 − 3 − 1 = **41** (cobra 19 si sale bien, −41 si sale mal). Sin verificar: e_H le da 45−41−1 = 3; e_L le da 15−41 = −26 ⇒ elige e_H solo. **La franquicia funciona aunque no se vea el esfuerzo.**

### Contratos implícitos (6.6)
El contrato laboral es **también un seguro**: la firma (neutral) paga un salario que **no depende del shock** ⇒ el salario no iguala la productividad marginal en cada estado ⇒ explica la **rigidez salarial**.

---

## 2. Unidad VII — Riesgo moral ("no veo lo que hacés")

### La idea en una frase
Si te pago fijo, no te esforzás; si te pago según el resultado, te hago cargar riesgo. **Trade-off: seguro vs. incentivos.**

### Lo nuevo: la restricción de incentivos (IC)
Además de la PC, el contrato debe hacer que al agente **le convenga** esforzarse:

Σ (pᴴᵢ − pᴸᵢ)·u(wᵢ) ≥ v(e_H) − v(e_L)

"Lo que gano en utilidad esperada por esforzarme ≥ lo que me cuesta."

**Si P quiere e_H, las dos (PC e IC) se saturan.** Con dos resultados (éxito S, fracaso F) y u = √w, el ejercicio se reduce a **dos ecuaciones lineales** en u_S = √w_S y u_F = √w_F:
- PC: p_H·u_S + (1−p_H)·u_F = Ū + v(e_H)
- IC: (p_H − p_L)·(u_S − u_F) = v(e_H) − v(e_L)

### Receta para cualquier ejercicio de riesgo moral con 2 esfuerzos
1. Plantear PC e IC con igualdad y resolver u_S, u_F.
2. Elevar al cuadrado (si u=√w) para tener los salarios.
3. Calcular E[w] con las probabilidades de e_H.
4. Comparar beneficio con e_H vs e_L (el contrato de e_L sigue siendo el fijo de antes).
5. Costo del riesgo moral = E[w] − salario fijo de info simétrica.

**Atajo (u = √w):** costo del riesgo moral = **(Δv)²/χ²**, con χ² = Σ (pᴴᵢ − pᴸᵢ)²/pᴴᵢ.
χ² mide **qué tan informativo** es el resultado sobre el esfuerzo: más informativo ⇒ más barato.

### Ejercicio 7.1 resuelto (mismos datos que 6.2, esfuerzo no verificable)
- PC: 0,75 u_S + 0,25 u_F = 4. IC: 0,5 (u_S − u_F) = 1 ⇒ u_S − u_F = 2.
- ⇒ u_F = 2,5, u_S = 4,5 ⇒ **w_F = 6,25 ; w_S = 20,25**.
- E[w] = 0,75·20,25 + 0,25·6,25 = **16,75** (vs 16 con info simétrica ⇒ costo 0,75).
- Check fórmula: χ² = 0,25/0,75 + 0,25/0,25 = 4/3 ⇒ (Δv)²/χ² = 1/(4/3) = 0,75 ✓.
- Beneficio con e_H: 45 − 16,75 = **28,25** > 6 ⇒ sigue pidiendo e_H.
- Multiplicadores: 1/u′ = 2√w; r_S = 1/3, r_F = 3 ⇒ 9 = λ + µ·(2/3), 5 = λ − 2µ ⇒ **µ = 1,5 ; λ = 8**.
- (e) Valor del éxito X: info simétrica pide e_H si X ≥ 14; con riesgo moral si X ≥ 15,5 ⇒ para **X ∈ (14; 15,5)** pide un esfuerzo ineficientemente bajo.

### El cociente de verosimilitud (lo más conceptual de la unidad)
rᵢ = pᴸᵢ / pᴴᵢ. Condición de primer orden: **1/u′(wᵢ) = λ + µ(1 − rᵢ)**.
- rᵢ < 1 (ese resultado es más típico de quien se esforzó) ⇒ **premio**.
- rᵢ > 1 (más típico de quien vagó) ⇒ **castigo**.
- **Se paga lo que el resultado *informa* sobre el esfuerzo, no lo que *vale* para el principal.**
- **FOSD** (dominancia estocástica) **no alcanza** para que el salario sea creciente; hace falta **MLRP** (r decreciente en el resultado). Por eso puede pasar que se pague **más por un resultado intermedio que por el más alto** (ej. 7.2).
- **Señal perfecta**: si un resultado es imposible con e_H (pᴴ = 0 < pᴸ), pongo un castigo enorme ahí y llego al óptimo de info simétrica (el castigo nunca se aplica en equilibrio: "al buen cochero le basta la amenaza").

### Teorema de informatividad de Holmström
**Una señal extra tiene valor ⇔ es informativa sobre el esfuerzo** (dado el resultado).
- Informe de supervisor correlacionado con el esfuerzo ⇒ vale.
- El clima, si cambia qué tanto el resultado informa sobre el esfuerzo ⇒ vale (una buena cosecha con mal clima es mejor señal de esfuerzo ⇒ se paga más).
- Una moneda tirada al aire ⇒ **no vale nada**, sólo agrega riesgo.
- Aplicaciones: **evaluación relativa** (vendedores de paraguas en la misma tienda), **auditorías y controles aleatorios**.
- 7.7(c): multar más si hay heridos (no depende de si bebió) ⇒ **no informativo, sólo agrega riesgo**. (d): multar a sobrios que chocan ⇒ castigar algo que no informa de haber bebido, mal diseño.
- 7.7(a) Bubka: le pagaban **por récord**, no por cuántos cm ⇒ optimizaba la variable por la que se le pagaba: **de a 1 cm**.

### Responsabilidad limitada (salarios ≥ 0)
Con agente **neutral** la franquicia resuelve todo… salvo que no se le pueda cobrar cuando sale mal. Entonces el agente se queda con una **renta** y el trade-off pasa a ser **renta vs. incentivos**.

**7.4 resuelto** (neutrales, x∈{0,60}, p_H=3/4, p_L=1/4, Δv=1, Ū=0):
- Franquicia: k = 45 − 0 − 1 = 44 (cobra 16 o −44) → funciona sin verificar.
- Con w ≥ 0: w_F = 0 y la IC 0,5·w_S ≥ 1 ⇒ **w_S = 2**. E[w] = 1,5 ⇒ **renta = 0,5**.
- (c) Sin costo si Ū ≥ 0,5. (d) Eficiente pedir e_H si X ≥ 2, pero con resp. limitada lo pide recién si X ≥ 3 ⇒ ineficiencia para **X ∈ (2,3)**.

### Racionamiento del crédito (Bester–Hellwig)
Proyecto **a** seguro y más rentable en esperanza; **b** riesgoso, paga más si sale bien. El banco cobra R sólo si hay éxito. El empresario elige a si **R ≤ R̂ = (p_a X_a − p_b X_b)/(p_a − p_b)**. Si el banco sube la tasa, empuja al empresario al proyecto riesgoso ⇒ prefiere no subirla ⇒ **racionamiento**.

**7.5 resuelto** (p_a=0,8; X_a=50; p_b=0,4; X_b=80; I=20):
- Simétrica: exige a, R = 50, gana 20.
- R̂ = (40 − 32)/0,4 = **20**. Con R = 20 gana 0,8·20 − 20 = −4; con R = 80 (y proyecto b) gana 0,4·80 − 20 = 12 ⇒ **cobra 80, se hace b (ineficiente), no hay racionamiento** (al empresario no le queda nada).
- (d) Hay racionamiento si 0,8·R̂ > 0,4·X_b con R̂ = 100 − X_b ⇒ **X_b < 66,7** (y > 50).
- (e) Con garantía C: hace falta **C ≥ 24** para lograr el resultado simétrico.

### Holmström–Milgrom (contratos lineales, 7.6)
x = e + ε, w = A + Bx, equivalente cierto = E[w] − (r/2)·Var(w) − e²/2. El agente elige e = B.
- Verificable: e = 1, B = 0 (lo aseguro).
- No verificable: **B* = 1/(1 + rσ²)**, e = B*. Más aversión o más ruido ⇒ menos incentivos.
- r = 2, σ² = 0,5 ⇒ B = 1/2, e = 1/2, beneficio 1/4 (vs 1/2).
- B > 0 aunque P sea neutral: **acá la parte variable es por incentivos, no por reparto de riesgo** (en la Clase 6 B era 0 con P neutral).

### Franquicias en seguros
Con riesgo moral, la póliza óptima tiene **franquicia** (deducible): el asegurado carga parte del daño para que le convenga cuidarse.

---

## 3. Unidad VIII — Selección adversa ("no sé quién sos")

### La idea en una frase
El "bueno" puede hacerse pasar por "malo" para cobrar de más ⇒ el principal le deja una **renta** y, para achicarla, **empeora el contrato del malo**. Trade-off: **eficiencia vs. renta informacional**.

### Limones (Akerlof)
El precio refleja la **calidad promedio** ⇒ los buenos se retiran ⇒ baja la calidad promedio ⇒ baja el precio… el mercado puede desaparecer.
- Valoración del comprador **θ + c** (aditiva): funciona **parcialmente**. Con θ ~ U[0,1]: se venden θ ≤ p, calidad media p/2, el comprador paga p/2 + c = p ⇒ **p = 2c**. Con c = 0,25: p = 0,5, se vende **la mitad**. Excedente 0,125 vs 0,25 con info simétrica. Se venden todos si **c ≥ 0,5**.
- Valoración **βθ** (proporcional): "**todo o nada**": β·p/2 ≥ p ⇔ **β ≥ 2** (si β < 2 no hay intercambio).

### Modelo con dos tipos (receta clave)
Tipo **G** (bueno, esfuerzo barato v(e)) y **B** (malo, esfuerzo caro k·v(e)), prob. q de ser G.
Cuatro restricciones, pero **sólo dos importan**:
- **PC_B se satura**: el malo queda en su reserva.
- **IC_G se satura**: el bueno queda indiferente entre su contrato e imitar al malo.
- PC_G e IC_B **sobran** (no se saturan).

Resultados (memorizar):
1. **Renta del bueno** = (k−1)·v(e_B) = lo que ganaría imitando al malo.
2. **Sin distorsión en la cima**: e_G = eficiente.
3. **Distorsión hacia abajo del malo**: Π′(e_B) = k v′(e_B) + [q/(1−q)]·(k−1) v′(e_B). Le pido menos esfuerzo para que su contrato sea menos tentador para el bueno.
4. Posible **exclusión** del malo.
5. No hace falta aversión al riesgo (a diferencia del riesgo moral).

**Principio de revelación**: alcanza con ofrecer un contrato por tipo donde a cada uno le convenga decir la verdad.

### Ejercicio 8.1 resuelto (Π=4e; G: w−e²; B: w−2e²; q=1/2; Ū=0)
- Simétrica: G: máx 4e − e² ⇒ e = 2, w = 4, gana 4. B: máx 4e − 2e² ⇒ e = 1, w = 2, gana 2. Promedio 3.
- No autoseleccionable: G con el contrato de B: 2 − 1 = 1 > 0 ⇒ lo imita.
- Menú: e_G = 2. Distorsión: 4 = 4e_B + 1·(2e_B) ⇒ **e_B = 2/3**, w_B = 2·(4/9) = **8/9**.
- Renta de G = (2−1)·(2/3)² = **4/9** ⇒ w_G = 4 + 4/9 = **40/9**.
- Beneficio: G: 8 − 40/9 = 32/9; B: 8/3 − 8/9 = 16/9 ⇒ promedio **8/3 ≈ 2,67**.
- Pérdida 1/3 = renta (½·4/9 = 2/9) + ineficiencia (½·[2 − 16/9] = 1/9).
- En general e_B = 2(1−q)/(2−q): q → 1 ⇒ e_B → 0 (distorsiono mucho a los pocos malos).

### Competencia (Rothschild–Stiglitz, seguros)
Ahora los tipos difieren en **riesgo** (prudentes vs imprudentes) y hay muchas aseguradoras (beneficio 0).
- **No hay equilibrio agrupador** (siempre alguien ofrece un contrato que sólo atrae a los buenos).
- Candidato separador: **alto riesgo ⇒ seguro completo justo**; **bajo riesgo ⇒ cobertura parcial** (justo para él, pero tal que el malo no lo quiera).
- **Existe sólo si hay pocos buenos** (q < umbral); si hay muchos, **puede no haber equilibrio**.
- Ahora quien quiere imitar es el **malo**, y "no distorsión en la cima" vale para el malo.
- Los malos quedan igual que con info simétrica; **los buenos pierden** (cargan riesgo para diferenciarse).

### Continuo de tipos (8.5)
- Renta por envolvente: I′(c) = −v(e(c)) ⇒ la renta de un tipo = suma de las desutilidades de todos los tipos peores.
- **Costo virtual** = c + F(c)/f(c). Con c ~ U[1,2]: F/f = c − 1 ⇒ costo virtual 2c − 1.
- El mejor tipo no se distorsiona; todos los demás hacen menos que lo eficiente; puede haber **bunching** (varios tipos con el mismo contrato).

### Espiral del seguro de salud (8.6 resuelto: c ~ U[20,100], pagan hasta 1,25c)
- Compran los c ≥ P/1,25 = 0,8P. Prima = gasto medio de los que compran: P = (0,8P + 100)/2 ⇒ **P ≈ 83,3**, se aseguran c ≥ 66,7 ⇒ **41,7 %**.
- Espiral desde 60: corte 48 → media 74; corte 59,2 → media 79,6; …
- Seguro obligatorio a 60: excedente 0,25·60 = **15** por persona vs ≈ 8,7 privado. **Pierden** los de bajo riesgo con 1,25c < 60, o sea **c < 48**.

### Instituciones correctoras
Garantías, marcas, cadenas (por eso están **en las rutas**: clientes de paso que no conocen los locales), licencias, certificaciones, informes técnicos independientes (8.7d), seguros obligatorios.

**Franquicia, dos lecturas (8.7b):** con selección adversa **separa tipos** (la eligen los de bajo riesgo); con riesgo moral **da incentivos** a cuidarse. El argumento del amigo ("para que los que chocan paguen $500") no es la razón: es que la elijan los prudentes.

---

## 4. Unidad IX — Señalización ("te muestro quién soy")

### La idea en una frase
El informado hace algo **costoso** que **sólo le conviene si es bueno**. Funciona porque **cuesta menos al bueno** (condición de **cruce único / Spence–Mirrlees**). La señal puede no producir nada: sólo informa.

### Diferencia con selección adversa
- **Screening (VIII)**: el que **no sabe** ofrece un menú.
- **Señalización (IX)**: el que **sabe** mueve primero.

### Spence (educación)
Ejemplo de la nota: productividad 1 (costo y) y 2 (costo y/2), salario 2 si y ≥ y*, 1 si no.
- Bajo no imita: 1 ≥ 2 − y* ⇒ y* ≥ 1. Alto se educa: 2 − y*/2 ≥ 1 ⇒ y* ≤ 2. ⇒ **separadores con y* ∈ [1,2]**.
- Hay **infinitos** equilibrios + **agrupadores**. Retorno privado ≠ retorno social (puede haber **sobreinversión** en educación).

### Ejercicio 9.1 resuelto (θ ∈ {1,3}, costo e/θ, w = 3 si e ≥ e₀)
- (a) Info simétrica: nadie se educa (no aumenta productividad).
- (b) Bajo: 1 ≥ 3 − e₀ ⇒ e₀ ≥ 2. Alto: 3 − e₀/3 ≥ 1 ⇒ e₀ ≤ 6 ⇒ **e₀ ∈ [2, 6]**.
- (c) λ = 0,4: agrupador en 0 paga 1 + 2·0,4 = 1,8 a todos. Desvío e′ ∈ (1,2; 3,6): al bajo no le conviene ni pagándole 3 (3 − e′ < 1,8) pero al alto sí (3 − e′/3 > 1,8) ⇒ el agrupador **no pasa el criterio intuitivo**. Sobrevive el **separador de menor costo, e₀ = 2**.
- (d) λ=0,4: separador: bajo 1, alto 3 − 2/3 ≈ 2,33; agrupador: ambos 1,8. λ=0,9: agrupador paga 2,8 ⇒ **ambos estarían mejor agrupados**, pero el criterio elige el separador igual.
- (e) Si educación sube productividad 0,1e: parte del diferencial es capital humano y el resto es revelación de productividad preexistente.

### Equilibrio bayesiano perfecto + criterio intuitivo
- **PBE**: cada uno optimiza dadas sus creencias; creencias por Bayes **donde se puede**. **Fuera del equilibrio las creencias son libres** ⇒ muchos equilibrios.
- **Criterio intuitivo (Cho–Kreps)**: si un tipo **nunca** ganaría mandando cierta señal (aun con la mejor respuesta posible), no se le puede atribuir. ⇒ Con 2 tipos se queda con el **separador de menor costo**.

**9.2 (tabla de la nota):** Δ = U_G* − U_B* ≈ 1,741; δ = U_G* − EU_G ≈ 0,137.
- v_B > Δ y v_G < δ ⇒ **sólo separador**.
- v_B > Δ y δ ≤ v_G ≤ Δ ⇒ **ambos**.
- v_B < Δ o v_G > Δ ⇒ **sólo agrupador**.
- Aplicado: (0,05; 3) → sólo separador (el bueno gana: 9,437 > 9,350). (0,5; 3) → ambos (el agrupador sobrevive porque al bueno no le conviene desviarse ni aunque lo reconozcan: 9,487 − 0,5 = 8,987 < 9,350). (0,5; 1,2) → sólo agrupador (al malo le sale barato imitar). (2; 3) → sólo agrupador (muy caro hasta para el bueno).

### Principal informado (9.3: el contrato es la señal)
El empresario con trabajo **fácil** quiere demostrarlo y para eso pide **pocas horas**: un empresario con trabajo arduo (para el que cada hora vale mucho) nunca pediría tan pocas.
- Simétrica: fácil e = 6, w = 18, gana 18; arduo e = 6, w = 54, gana 54.
- Separador: w₁ = e₁²/2 y 18e₁ − e₁²/2 = 54 ⇒ **e₁ ≈ 3,30, w₁ ≈ 5,46**; gana ≈ 14,36 ⇒ **costo de señalar ≈ 3,64**.

### Otras aplicaciones
- **Precios de lanzamiento (9.4)**: el bueno lanza **por debajo de su costo** (p₁ = c_B) para que prueben y vuelvan. Beneficio = (c_B − c_G) + δ(X − c_G). Con X=12, c_G=5, c_B=3: δ ≥ **2/7**; con δ = 0,5 gana **1,5**. No hay agrupador porque qX = 2,4 < c_B = 3. Publicidad de marca = "quemar plata" que sólo recupera el bueno.
- **Deuda como señal (Ross, 9.5)**: sólo un gerente de empresa buena se arriesga a quebrar. Intervalo: k_B·(1−γ)(k_G−k_B)/(2γL) ≤ D ≤ k_G·(…). Con 120/60/½/60: factor 0,5 ⇒ **30 ≤ D ≤ 60**. Doble multa ⇒ intervalo a la mitad (15–30). k_G = 180 ⇒ 60–180.
- **Índices y discriminación (9.6)**: grupos idénticos pueden quedar en **equilibrios distintos** (trampa de nivel bajo). A en 1,2: alto neto 1,4; B en 1,8: alto neto 1,1. La diferencia **no** se debe a capacidades distintas.
- **Cheap talk**: decir "soy productivo" no sirve porque **todos** lo dirían (9.7c). Un título sí, porque cuesta distinto.
- **9.7(d)** Franquicia (VIII): la diseña el **no informado** (aseguradora) para separar. Garantía (IX): la ofrece el **informado** (vendedor) para señalar.

---

## 5. Unidad X — Subastas

### La idea en una frase
El vendedor no sabe cuánto vale el bien para cada uno ⇒ **los hace competir** para que lo revelen.

### Los 4 formatos
| Formato | Gana | Paga | Equivale a |
|---|---|---|---|
| Inglesa (ascendente) | el último que queda | precio de retiro del penúltimo | 2º precio (valores privados) |
| Holandesa (descendente) | el primero que acepta | lo que aceptó | 1º precio (**siempre**) |
| 1º precio sobre cerrado | la más alta | **su** oferta | holandesa |
| 2º precio (Vickrey) | la más alta | la **segunda** oferta | inglesa |

### Valores privados independientes (VPI)
- **2º precio: ofertar tu valuación es débilmente dominante.** Tu oferta sólo decide *si* ganás, no *cuánto* pagás. Ofertar menos: podés perder algo que te convenía; ofertar más: podés ganar pagando de más.
- **1º precio**: rebajás la oferta. Con U[0,1] y N oferentes: **b(v) = (N−1)/N · v** (N=2 ⇒ v/2; N=3 ⇒ 2v/3).
- **Equivalencia de recaudación**: VPI + neutrales + simétricos + mismo ganador + el tipo más bajo paga 0 ⇒ **misma recaudación esperada** = E[segunda valuación] = (N−1)/(N+1).
- **Falla con**: aversión al riesgo de compradores (**favorece 1º precio**: se rebaja menos), asimetrías, valores correlacionados, colusión.
- La **varianza** del precio es **menor en 1º precio** ⇒ un vendedor averso prefiere 1º precio.

### Ejercicio 10.1 (v = 50, 40, 30; segundo precio)
- Para el oferente 2 (v=40), ofertar 40 nunca es peor que 30 o 50 para cualquier máximo rival m: si m=35, ofertando 30 pierde (0) y con 40 gana 5; si m=45, ofertando 50 gana y paga 45 (−5), con 40 pierde (0).
- (b) Gana el 1 y paga **40**. En la inglesa igual: el precio sube hasta 40 y el 2 se retira.
- (c) En 3º precio conviene ofertar **más** que la valuación ⇒ deja de ser dominante.
- (d) Riesgo: el vendedor mete una oferta falsa (**shill**) justo debajo de la ganadora; Vickrey propone **mostrar la segunda oferta**.

### Ejercicio 10.2 (N = 3, U[0,1])
- b(v) = 2v/3. Recaudación esperada en ambos = 2/4 = **1/2**. Ganancia del ganador = 1/(N+1) = **1/4**.
- Var 1º = 1/60; Var 2º = 1/20 ⇒ cociente **3 = N**.
- Con 0,9; 0,3; 0,2: 1º precio cobra 0,6; 2º cobra 0,3. **No contradice** el teorema: es sobre el **promedio**, no cada realización.
- Vendedor averso ⇒ **1º precio** (menos varianza).

### 10.3 Aversión al riesgo (u = x^ρ, N = 2)
2º precio sigue b = v (la aversión no cambia que ofertar la verdad sea dominante). 1º precio: b = v/(1+ρ). Con ρ = ½: b = 2v/3 ⇒ recauda (2/3)(2/3) = **4/9 > 1/3**.

### Precio de reserva (10.4)
R(r) = 1/3 + r² − (4/3) r³ ⇒ **r* = ½, R = 5/12 ≈ 0,417**. No se vende con prob. r² = **1/4** ⇒ **ineficiente** (extraer renta a costa de eficiencia, igual que el monopolista del menú en VIII). Con v₀ = 0,2: r − (1−r) = 0,2 ⇒ **r = 0,6**. La reserva óptima **no depende de N**.

### Equipos (Holmström 1982, 10.6)
Si se reparte todo el producto entre los socios ⇒ **free riding** (nadie se queda con todo su aporte). No hay reparto con presupuesto equilibrado que sea eficiente.
- 3 socios, x = e₁+e₂+e₃, c = e²/2: eficiente e = 1, x = 3, excedente 1,5.
- Reparto igual: e = 1/3, x = 1, cada uno 1/3 − 1/18 = **5/18**.
- Solución: **principal externo** que "rompe el presupuesto": paga 1 a cada uno si x ≥ 3, si no se queda todo ⇒ e = 1 es equilibrio (cada uno ½). No puede ser un socio porque tendría incentivo a sabotear.
- Subasta inglesa del derecho al residuo (1,2; 0,9; 0,5): gana el de **1,2** y paga **0,9**.

### Valor común y maldición del ganador (10.5)
El bien vale lo mismo para todos pero nadie lo sabe. **Ganar es una mala noticia**: ganó el que más sobreestimó.
- Error U[−a, a]: el ganador sobrestima (N−1)/(N+1)·a. Con a = 20, N = 5 ⇒ **13,3**. Si ofertó 150 estimando 150 ⇒ pierde ≈ 13,3 en promedio.
- 2º precio: b(x) = x − (N−2)/N · a = 150 − 12 = **138**.
- Wilson (normales): b = θ − √π·s ≈ θ − 1,77s ⇒ s = 12: **128,7**; s = 6: **139,4** (menos incertidumbre ⇒ oferto más cerca).
- **Más oferentes puede no subir las ofertas**: la maldición empeora y todos rebajan más.

### Milgrom–Weber (valores afiliados)
- Orden de recaudación: **inglesa ≥ 2º precio ≥ 1º precio = holandesa** (principio de vinculación: cuanto más depende el precio de la info de los demás, menos renta para el ganador).
- **"La honestidad es la mejor política"**: al vendedor le conviene **comprometerse a publicar** la tasación. Si publicara sólo las buenas, el silencio se lee como mala noticia (limones).

### Varias unidades (10.7: A quiere 2 a 12 c/u; B 8; C 3)
- Precio uniforme = primera rechazada, ofertas sinceras (12,12,8,3): A gana las 2, precio **8**, recauda **16**; A gana 8.
- A oferta (12, 0): ganan A y B, precio 3 ⇒ A gana 9 > 8 ⇒ **reducción de demanda**; ineficiente (la 2ª unidad vale 12 para A).
- Vickrey: A paga lo que su victoria le quita a los demás (B+C = 11) ⇒ paga **11**, gana 13.
- Discriminatoria (pagás tu oferta): **no** ofertan su valuación (rebajan).
- Letras del Tesoro "holandés de precio único" = sobre cerrado de **precio uniforme = última aceptada** ⇒ incentivos a reducir demanda.

### Reputación online
- Calificaciones libres ⇒ inflación por reciprocidad/represalias. MercadoLibre usa **reclamos, cancelaciones y demoras**: conductas **verificables**.
- **Sniping** (ofertar al último segundo) es más común con **cierre fijo** que con cierre extendido.
- 10.8(e): producto original o no → **selección adversa**; envío a tiempo según esfuerzo → **riesgo moral**; vendedor nuevo con envío gratis y devolución → **señalización**.
- 10.8(b) 4G 2014: reservar un bloque para un entrante a precio mínimo **sacrifica recaudación hoy a cambio de competencia futura**.

---

## 6. Cuadro final para repasar la noche antes

| | Riesgo moral (VII) | Selección adversa (VIII) | Señalización (IX) |
|---|---|---|---|
| ¿Qué se oculta? | acción | tipo | tipo |
| ¿Cuándo? | después de firmar | antes | antes |
| ¿Quién mueve primero? | P | P (menú) | el informado |
| Restricciones activas | PC e IC | PC del malo, IC del bueno | (señal: bueno la manda, malo no imita) |
| Trade-off | seguro vs incentivos | eficiencia vs renta | costo de la señal vs. separarse |
| ¿Hace falta aversión al riesgo? | sí (o resp. limitada) | no | no |
| ¿Quién gana renta? | nadie (agente averso) | el bueno | — |
| ¿Qué se distorsiona? | riesgo al agente / esfuerzo bajo | esfuerzo del malo | el bueno gasta en la señal |
| En un mercado | racionamiento de crédito | limones, no existencia de equilibrio | sobreinversión en educación |

### Frases que suman puntos
- "El salario paga el **contenido informativo** del resultado, no su valor."
- "Sin distorsión en la cima": **no se distorsiona el contrato del tipo al que nadie quiere imitar**; se distorsiona el del tipo que el otro querría imitar (en VIII monopolista, el malo; en Rothschild–Stiglitz, el bueno).
- "La señal funciona porque **cuesta menos** al tipo bueno (cruce único)."
- "Las creencias fuera del equilibrio son libres; el criterio intuitivo las disciplina."
- "Con VPI el formato no importa para la recaudación esperada; importan la **reserva**, la aversión al riesgo y las asimetrías."
- "Con valor común, **ganar es una mala noticia**."
