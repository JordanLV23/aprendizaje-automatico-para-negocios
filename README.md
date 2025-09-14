# Descubriendo tesoros bajo tierra 🚀

Hola, soy Jordan y este proyecto nació de mi curiosidad por aplicar lo aprendido en machine learning al mundo de los negocios. Después de terminar otro sprint, me propuse ayudar a la ficticia empresa **OilyGiant** a decidir dónde perforar nuevos pozos petroleros para que la inversión valiera la pena.

## ¿Qué hice?

- **Analicé datos:** trabajé con tres conjuntos de datos de regiones distintas, cada uno con características geológicas y el volumen real de reservas.
- **Entrené un modelo:** utilicé un modelo de **regresión lineal** para predecir cuántos miles de barriles podría producir cada pozo. Para evitar sesgos dividí los datos en un 75 % de entrenamiento y un 25 % de validación.
- **Seleccioné los mejores pozos:** elegí los 200 pozos con mejores predicciones por región y calculé el beneficio potencial con un precio de 4 500 USD por cada mil barriles, considerando un presupuesto total de 100 millones.
- **Evalué el riesgo:** utilicé **bootstrapping** (muestreo repetido) para estimar cómo varían las ganancias y cuán probable es perder dinero.

## ¿Qué descubrí?

Ninguna región superaba el umbral de 111,1 unidades de producción media (equivalente a 500 000 USD por pozo), aunque una de ellas se acercaba más que las demás. Al comparar beneficios y riesgos, una región destacó por su equilibrio y fue mi recomendación final. Este análisis demuestra que no basta con mirar el promedio de producción: hay que considerar la probabilidad de éxito y el costo de equivocarse.

## ¿Por qué es importante?

Este tipo de proyectos convierte **datos** en **decisiones**. Me permitió comprobar que un modelo sencillo, combinado con un análisis cuidadoso de riesgos, puede guiar inversiones millonarias. Además, reafirmó esa lección de la vida diaria: elegir pozos es como escoger aguacates en el mercado; no solo cuentan el tamaño y el color, también tienes que tantearlos para saber si saldrán buenos.

## Conclusiones

- **La ciencia de datos en acción:** aplicar machine learning a un negocio real es más que escribir código; es crear una brújula para inversiones millonarias.
- **Equilibrio entre beneficio y riesgo:** la mejor región no era la más abundante, sino la que ofrecía un balance atractivo entre ganancias esperadas y probabilidad de pérdidas. Un buen negocio no siempre es el que promete más, sino el que te deja dormir tranquilo.
- **Lecciones personales:** traducir métricas y técnicas como el RMSE y el bootstrapping a un lenguaje sencillo me permitió compartir resultados con un público no técnico. Y sí, elegir pozos es como comprar aguacates: hay que saber evaluar antes de invertir.
