# Práctica Unidad VII — SOLUCIONES

> No mirar hasta haber terminado.

---

## Ejercicio 1

Resultado esperado: con e_H = 0,6·120 = **72**; con e_L = 0,2·120 = **24**.

**a.** Borch: principal neutral → salario fijo. PC con igualdad: √w − v(e) = 4 → w = (4 + v(e))².
- e_H: **w = 36**; e_L: **w = 16**.
- Beneficio: e_H: 72 − 36 = **36**; e_L: 24 − 16 = **8** → **exige e_H y gana 36**.

**b.** Con w = 36 fijo: esforzándose 6 − 2 = **4**; sin esforzarse **6** → **elige e_L**. Beneficio: 24 − 36 = **−12**.

**c.** Mín 0,6w_S + 0,4w_F s.a.
- **PC:** 0,6√w_S + 0,4√w_F − 2 ≥ 4
- **IC:** 0,6√w_S + 0,4√w_F − 2 ≥ 0,2√w_S + 0,8√w_F → 0,4(√w_S − √w_F) ≥ 2

Con u_S = √w_S, u_F = √w_F y ambas con igualdad:
- PC: 0,6u_S + 0,4u_F = 6
- IC: u_S − u_F = 5
- u_F + 0,6·5 = 6 → **u_F = 3**, **u_S = 8** → **w_S = 64, w_F = 9**.

Verificación: e_H: 0,6·8 + 0,4·3 − 2 = 4 = Ū ✓; e_L: 0,2·8 + 0,8·3 = 4 → indiferente ✓.

**d.** 1/u′(w) = 2√w = λ + µ(1 − r), con r_S = 0,2/0,6 = **1/3** y r_F = 0,8/0,4 = **2**.
- Éxito: 16 = λ + (2/3)µ; fracaso: 6 = λ − µ → 10 = (5/3)µ → **µ = 6**, **λ = 12**.
- Control: λ = E_H[2u] = 0,6·16 + 0,4·6 = 12 ✓.
- Salario neutro (r = 1): (λ/2)² = **36** (el fijo simétrico). Éxito (r < 1) se **premia**: 64 > 36. Fracaso (r > 1) se **castiga**: 9 < 36. µ > 0: el riesgo moral le cuesta al principal.

**e.** E_H[w] = 0,6·64 + 0,4·9 = **42** → beneficio 72 − 42 = **30** > 8 → **sigue exigiendo e_H**.
- **Costo del riesgo moral = 42 − 36 = 6** (gana 30 en vez de 36).
- Fórmula: A = 4 + 2 = 6 → A² = 36; Δv = 2; χ² = 0,4²/0,6 + 0,4²/0,4 = 0,267 + 0,4 = **2/3** → (Δv)²/χ² = 4/(2/3) = **6** ✓ → E_H[w] = 42 ✓.
- Interpretación: prima de riesgo. El agente valora la lotería (64 o 9) en (0,6·8 + 0,4·3)² = **36**, pero al principal le cuesta 42. Trade-off seguro vs. incentivos.

**f.**
- Simétrica: 0,6X − 36 ≥ 0,2X − 16 → 0,4X ≥ 20 → **X ≥ 50**
- Riesgo moral: 0,6X − 42 ≥ 0,2X − 16 → 0,4X ≥ 26 → **X ≥ 65**
- → **50 < X < 65**: exige e_L aunque lo eficiente sea e_H.

---

## Ejercicio 2

Resultado esperado: con e_H = 0,8·50 = **40**; con e_L = 0,3·50 = **15**.

**a.** k = E[x | e_H] − Ū − v(e_H) = 40 − 0 − 2 = **38** → el agente cobra 50 − 38 = **12** si hay éxito y **−38** si hay fracaso.
- Sin verificar: con e_H obtiene 40 − 38 − 2 = **0**; con e_L, 15 − 38 = **−23** → **elige e_H solo** (se queda con todo el resultado marginal).
- El principal gana **38**, igual que con información simétrica: costo cero.

**b.**
- IC: (0,8 − 0,3)(w_S − w_F) ≥ 2 → **w_S − w_F ≥ 4**
- PC: 0,8w_S + 0,2w_F − 2 ≥ 0
- Lo más barato con w ≥ 0: **w_F = 0, w_S = 4** → **E[w] = 3,2**.
- PC holgada: el agente obtiene 3,2 − 2 = **1,2** > 0 → **renta = 1,2**.
- Beneficio del principal: 40 − 3,2 = **36,8** (en vez de 38).

**c.** PC e IC con igualdad: w_S = w_F + 4 y 0,8(w_F + 4) + 0,2w_F − 2 = Ū → w_F + 1,2 = Ū → **w_F = Ū − 1,2**. Es no negativo si **Ū ≥ 1,2**: con una reserva alta igual hay que pagarle bastante y la restricción no muerde.

**d.**
- Eficiente (franquicia): 0,8X − 2 ≥ 0,3X → 0,5X ≥ 2 → **X ≥ 4**
- Con responsabilidad limitada (cuesta 3,2; e_L se consigue con salario 0): 0,8X − 3,2 ≥ 0,3X → 0,5X ≥ 3,2 → **X ≥ 6,4**
- → **4 < X < 6,4**.

**e.** La ineficiencia viene de la **responsabilidad limitada**: la franquicia (que da incentivos sin costo a un agente neutral) exige que el agente pague cuando el resultado es malo, y eso no se puede. Para dar incentivos hay que premiar el éxito, lo que deja al agente una **renta**. El trade-off es **renta vs. incentivos** (no seguro vs. incentivos): si la renta es cara en relación con el valor del éxito, el principal renuncia al esfuerzo alto.

---

## Ejercicio 3 — Puntos que tiene que tener cada respuesta

**a.** El agente optimiza **la variable por la que se le paga** (como Bubka). El bono premia "superar 100" en cada mes, no la cantidad total vendida: conviene vender justo 100–101 y pasar el resto al mes siguiente para cobrar el bono más veces. Esquema mal diseñado: pagar por unidad vendida o por ventas acumuladas en un período más largo.

**b.** **Sí, es buena idea (evaluación relativa).** Como los dos locales enfrentan el **mismo shock** de demanda, las ventas del otro local son **informativas** sobre el esfuerzo de cada gerente: comparando se filtra la suerte común y se dan los mismos incentivos con menos riesgo (teorema de Holmström). En **ciudades distintas** los shocks están poco correlacionados: las ventas del otro local informan poco o nada sobre el esfuerzo, y condicionar el pago a ellas sólo agregaría riesgo → conviene pagar sólo según las ventas propias.

**c.** Que haya habido un **siniestro** es informativo sobre el cuidado del asegurado → tiene sentido usarlo (incentiva a cuidarse). El **color del auto** no depende del cuidado ni informa sobre él → por Holmström, condicionar la prima a eso sólo agrega riesgo sin mejorar los incentivos: **mala propuesta** (desde el punto de vista de incentivos).

**d.** **Sí tiene sentido.** El clima no depende del esfuerzo, pero cambia lo que significa el resultado: una buena cosecha con **sequía** es mucho más improbable sin esfuerzo, así que es una **señal más fuerte de esfuerzo** que con buen clima (cociente de verosimilitud más bajo) → se premia más. El clima es una **señal informativa** y tiene valor (Holmström). Con buen clima, una buena cosecha podría deberse a la suerte.

**e.** Ambos usan información sobre la acción oculta y tienen valor.
- **(i) Control aleatorio:** la probabilidad de ser detectado no depende de la suerte del proyecto; con una **probabilidad baja y una multa alta alcanza** para disuadir (control aleatorio de Holmström), y es barato.
- **(ii) Control condicional** (sólo si hay atrasos): también es barato, porque sólo se investiga cuando el resultado es malo; pero detecta sólo cuando hay atraso, que puede deberse a mala suerte. Necesita multas mayores y carga más riesgo sobre empleados aversos, y no detecta a quien no trabaja pero tuvo suerte.
- Conclusión: el aleatorio suele dar incentivos más directos con menos riesgo; lo ideal puede ser combinarlos.
