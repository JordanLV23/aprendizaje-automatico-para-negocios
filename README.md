# Proyecto Diplomado Data Science para encontrar los mejores lugares para realizar una inversión de extracción de petroleo 🚀

Hola, soy Jordan y este proyecto nació de mi curiosidad por aplicar lo aprendido en machine learning al mundo de los negocios. Después de terminar otro sprint, me propuse ayudar a la ficticia empresa OilyGiant a decidir dónde perforar nuevos pozos petroleros para que la inversión valiera la pena.

## ¿Qué hice?
- Analicé tres conjuntos de datos de regiones distintas, cada uno con características geológicas y el volumen real de reservas.
- Entrené un modelo de **regresión lineal** para predecir cuántos miles de barriles podría producir cada pozo. Usé una división 75 % – 25 % para entrenar y validar sin sesgo.
- Seleccioné los 200 pozos con mejores predicciones por región y calculé el beneficio potencial con un precio de 4 500 USD por cada mil barriles, considerando un presupuesto total de 100 millones.
- Evalué la rentabilidad y el riesgo mediante **bootstrapping** (muestreo repetido) para ver cómo varían las ganancias y cuán probable es perder dinero.

## ¿Qué descubrí?
Ninguna región superaba el umbral de 111,1 unidades de producción media, aunque una de ellas se acercaba más que las demás. Al comparar beneficios y riesgos, una región destacó por su equilibrio y fue mi recomendación final. Este análisis demuestra que no basta con mirar el promedio de producción: hay que considerar la probabilidad de éxito y el costo de equivocarse.

## ¿Por qué es importante?
Este tipo de proyectos convierte datos en decisiones. Me permitió comprobar que un modelo sencillo, combinado con un análisis cuidadoso de riesgos, puede guiar inversiones millonarias. Además, reafirmó esa lección de la vida diaria: elegir pozos es como escoger aguacates en el mercado; no solo cuentan el tamaño y el color, también tienes que tantearlos para saber si saldrán buenos.
