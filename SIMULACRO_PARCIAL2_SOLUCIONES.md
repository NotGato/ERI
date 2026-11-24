# Simulacro de Segundo Parcial — SOLUCIONES

> No mirar hasta haber terminado el simulacro.

---

## Ejercicio 1

Resultado esperado: con e_H = 0,8·100 = **80**; con e_L = 0,4·100 = **40**.

**a.** Borch: principal neutral (B′ constante) → u′(w) igual en éxito y fracaso → como u′ es decreciente, **w igual**: salario fijo. El neutral asegura al averso; y como el esfuerzo se exige por contrato, no hace falta atar el pago al resultado.
- PC con igualdad: √w − v(e) = 3 → w = (3 + v(e))².
- e_H: **w = 25**; e_L: **w = 9**.
- Beneficio: e_H: 80 − 25 = **55**; e_L: 40 − 9 = **31** → **exige e_H y gana 55**.

**b.** Con w = 25 fijo: esforzándose 5 − 2 = **3**; sin esforzarse **5** → **elige e_L**. Beneficio: 40 − 25 = **15**. El seguro completo destruye los incentivos (habría ganado 31 pidiendo e_L con w = 9).

**c.** Franquicia w = x − k, con k = E[x] − Ū − v(e):
- e_H: k = 80 − 3 − 2 = **75** → cobra **25** en éxito y **−75** en fracaso.
- e_L: k = 40 − 3 = **37** → el principal prefiere e_H (75 > 37).
- Sin verificar: con e_H el agente obtiene 80 − 75 − 2 = **3**; con e_L, 40 − 75 = **−35** → **se esfuerza solo** (se queda con todo el resultado marginal).
- Control: 0,8·25 + 0,2·(−75) − 2 = 20 − 15 − 2 = 3 = Ū ✓

**d.** u_S = √w_S, u_F = √w_F:
- PC: 0,8u_S + 0,2u_F = 5
- IC: (0,8 − 0,4)(u_S − u_F) = 2 → **u_S − u_F = 5**
- u_F + 4 = 5 → **u_F = 1**, **u_S = 6** → **w_S = 36, w_F = 1**
- Verificación: e_H: 0,8·6 + 0,2·1 − 2 = 3 ✓; e_L: 0,4·6 + 0,6·1 = 3 → indiferente ✓
- E[w] = 0,8·36 + 0,2·1 = **29** → beneficio 80 − 29 = **51** (> 31, sigue pidiendo e_H)
- **Costo del riesgo moral = 29 − 25 = 4** (control: χ² = 0,16/0,8 + 0,16/0,2 = 1 → (Δv)²/χ² = 4 ✓). Es la prima de riesgo: el agente valora la lotería en (0,8·6 + 0,2·1)² = 25.

**e.**
- Simétrica: 0,8X − 25 ≥ 0,4X − 9 → 0,4X ≥ 16 → **X ≥ 40**
- Riesgo moral: 0,8X − 29 ≥ 0,4X − 9 → 0,4X ≥ 20 → **X ≥ 50**
- → **40 < X < 50**: exige e_L aunque lo eficiente sea e_H.

---

## Ejercicio 2

**a.** Simétrica (salario = costo):
- G: máx 8e − e² → **e = 4, w = 16**, gana **16**.
- B: máx 8e − 2e² → **e = 2, w = 8**, gana **8**.
- Esperado: ⅓·16 + ⅔·8 = **32/3 ≈ 10,67**.
- No autoseleccionables: G con el contrato de B obtiene 8 − 2² = **4 > 0** (con el suyo 0) → el bueno imita al malo.

**b.** Se saturan **PC_B** (el malo queda en su reserva; si ganara de más se le baja el pago) e **IC_G** (el que quiere mentir es el bueno). PC_G sobra (G imitando a B ya gana algo) e IC_B queda holgada (el contrato de G pide mucho esfuerzo).
- PC_B: **w_B = 2e_B²**; IC_G: **w_G = e_G² + e_B²** (renta = e_B²).
- Beneficio: ⅓[8e_G − e_G² − e_B²] + ⅔[8e_B − 2e_B²].
- e_G: 8 − 2e_G = 0 → **e_G = 4** (sin distorsión en la cima).
- e_B: ⅓(−2e_B) + ⅔(8 − 4e_B) = 0 → −2e_B + 16 − 8e_B = 0 → **e_B = 1,6** (menos que 2).
- w_B = 2·2,56 = **5,12**; **renta de G = 2,56**; w_G = 16 + 2,56 = **18,56**.
- Beneficio: con G 32 − 18,56 = 13,44; con B 12,8 − 5,12 = 7,68 → esperado ⅓·13,44 + ⅔·7,68 = **9,6**.
- Verificación: G con el suyo 18,56 − 16 = 2,56; imitando 5,12 − 2,56 = 2,56 → indiferente ✓. B con el de G: 18,56 − 32 < 0 ✓.

**c.** Pérdida = 10,67 − 9,6 = **1,07**:
- Renta: ⅓·2,56 = **0,853**
- Ineficiencia de B: ⅔·(8 − 7,68) = **0,213**
- Total ≈ 1,067 ✓

**d.** −2q·e_B + (1 − q)(8 − 4e_B) = 0 → **e_B = 4(1 − q)/(2 − q)** (con q = ⅓: (8/3)/(5/3) = 1,6 ✓).
- q → 0: e_B → 2 = eficiente → **no hay distorsión** (la renta casi nunca se paga).
- q → 1: e_B → 0 → **distorsión máxima / exclusión** (conviene sacrificar a los pocos malos para no pagar renta a los muchos buenos).

---

## Parte II — Puntos que tiene que tener cada respuesta

**3a.** Seguro vs. incentivos: el reparto eficiente (Borch) pide asegurar al agente averso con salario fijo, pero con salario fijo no se esfuerza. Para dar incentivos el pago debe depender del resultado → el agente carga riesgo → hay que pagarle una prima de riesgo (o pedir menos esfuerzo). Con agente neutral no hay conflicto: la franquicia (w = x − k) le deja todo el resultado marginal, se esfuerza solo y no hay que compensarlo por riesgo → costo cero. Con responsabilidad limitada la franquicia (que exige pagar si sale mal) no se puede usar: hay que premiar el éxito, el agente gana una renta → trade-off renta vs. incentivos, y a veces se pide un esfuerzo ineficientemente bajo.

**4a.** El vendedor conoce la calidad y el comprador no → el precio refleja la calidad promedio de lo que se ofrece → a ese precio los dueños de lo bueno no venden → baja la calidad promedio → baja el precio… Lo malo expulsa a lo bueno y el mercado se achica o desaparece, aunque para cada bien haya un comprador que lo valora más que su dueño (se pierden ganancias del intercambio).

**4b.** "Sin distorsión en la cima": el contrato del tipo eficiente cumple la condición de eficiencia (hace el esfuerzo de información simétrica), porque nadie quiere imitarlo y distorsionarlo no ahorra nada. Al tipo menos eficiente se le pide menos esfuerzo: así su contrato es menos tentador para el bueno y baja la renta informacional que hay que pagarle. En el óptimo del malo, reducir un poco el esfuerzo tiene un costo de segundo orden y un ahorro de renta de primer orden → siempre conviene distorsionar algo. Trade-off eficiencia vs. renta.

**4c.** Ejemplos (dos, con mecanismo): garantías (le cuestan poco al que vende calidad → separan), marcas/cadenas (dan información y un medio de represalia), certificaciones/licencias/informes independientes (generan información), seguro obligatorio (evita la espiral agrupando a todos). Franquicia voluntaria: menú de autoselección; la eligen los de bajo riesgo (la pagan pocas veces y ahorran prima), los de alto riesgo prefieren cobertura completa → separa tipos. (Con riesgo moral, además, da incentivos al cuidado.)

**5a.** Segundo precio: la propia oferta sólo decide si se gana; el precio lo fija la segunda oferta. Ofertar menos que la valuación sólo cambia el resultado cuando la oferta rival está entre ambas → se pierde un objeto rentable. Ofertar más sólo lo cambia cuando la oferta rival supera la valuación → se gana pagando de más. Ofertar la valuación nunca es peor y a veces es mejor → débilmente dominante, sin necesidad de prever a los rivales. Primer precio: se paga la propia oferta; ofertar la valuación da ganancia nula, así que conviene rebajar (b = (N − 1)/N·v con uniformes), y cuánto depende de lo que hagan los demás → no hay estrategia dominante.

**5b.** Valor común: el bien vale lo mismo para todos pero nadie lo conoce; cada uno lo estima con error. Gana quien más lo sobreestimó → ganar es una mala noticia sobre el valor; quien oferta su estimación pierde en promedio (maldición del ganador). La oferta racional corrige: se oferta el valor esperado condicional a ganar (por debajo de la estimación). Con más oferentes, ganarle a todos es peor noticia (el ganador sobreestima más: (N − 1)/(N + 1)·a), así que la corrección crece y puede compensar el efecto de la mayor competencia → las ofertas pueden no subir.
