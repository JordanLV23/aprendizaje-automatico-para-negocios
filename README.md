# ¡Cazadores de Oro Negro! 💥

Imagina que acabas de terminar otro curso y en lugar de irte a celebrar, te toca demostrar lo que aprendiste en un proyecto que huele a petróleo. Este repositorio es tu bitácora de aventuras en **OilyGiant**, una empresa que busca nuevos pozos de crudo y necesita tu talento para encontrar *las joyas escondidas* bajo tierra.

## ¿De qué va todo esto? (Project Overview)

¿Alguna vez has jugado a buscar tesoros? Pues aquí el “tesoro” son reservas de petróleo y la arena del desierto se convierte en **datos**. Tu misión es:

1. **Conocer las regiones:** Tienes tres conjuntos de datos (`geo_data_0.csv`, `geo_data_1.csv` y `geo_data_2.csv`) que representan regiones diferentes. Cada archivo trae:
   - Un `id` (identificador del pozo).
   - Tres *features* (`f0`, `f1`, `f2`) que son como pistas misteriosas sobre la calidad del suelo (no te preocupes por lo que significan; son importantes para el modelo pero no necesitas saber su origen).
   - `product`, que indica el volumen de reservas en miles de barriles (el premio gordo).

2. **Construir un modelo predictivo:** Aquí entras tú con lo que aprendiste. Usas **regresión lineal** (una herramienta de machine learning que intenta ajustar una línea a los datos para hacer predicciones; imagina una regla que ayuda a trazar la mejor línea recta entre puntos), separando tus datos en entrenamiento (75 %) y validación (25 %) para no engañarte a ti mismo. El modelo intentará predecir cuántos barriles puede producir un pozo nuevo basándose en sus características.

3. **Elegir los mejores pozos:** No vas a perforar todos los pozos posibles, eso sería como comerse todos los dulces de la piñata de una sola sentada. Vas a escoger *los 200 pozos con las predicciones más altas* en cada región. Es como seleccionar las piezas de fruta más jugosas de tres canastos diferentes: te quedas con las 200 que prometen más jugo.

4. **Calcular la ganancia:** Luego traduces esas predicciones en dinero. Sabes que:
   - Tienes un **presupuesto** de 100 millones de dólares para perforar 200 pozos (es decir, 500 000 USD por pozo como mínimo para no perder dinero). Eso equivale a 111,1 unidades de producción por pozo.
   - Cada unidad (mil barriles) vende a 4,500 USD.
   - Para que el negocio sea rentable, el promedio de producción de cada pozo debe superar ese umbral de 111,1 unidades.
   - Usas estas reglas para calcular la **rentabilidad** de cada región. Si una región tiene un promedio de producción por encima de 111,1, está dando la talla; si no, mejor seguir buscando.

5. **Evaluar el riesgo (bootstrapping):** Porque no todo es color de rosa, analizas los riesgos usando una técnica llamada **bootstrapping** (tomar muchas muestras aleatorias con reemplazo de tus datos para ver qué tan variable es el beneficio; es como simular miles de realidades paralelas para ver en cuáles ganas y en cuáles pierdes). Calculas:
   - La **ganancia media** de cada región.
   - El **intervalo de confianza del 95 %** (un rango que, con un 95 % de seguridad, contiene la ganancia real).
   - El **riesgo de pérdida** (la probabilidad de terminar con números rojos), que no debe superar el 2,5 %.

Finalmente, recomiendas la región con la mejor combinación de beneficio alto y riesgo bajo. Es como elegir a qué fiesta ir: la que promete diversión pero donde tienes menor probabilidad de acabar con resaca económica.

## ¿Por qué es importante este proyecto? (Why It Matters)

Más allá de perforar la tierra, este ejercicio te enseña a aplicar ciencia de datos al mundo real: transformas archivos con números en decisiones de millones de dólares. Es como cuando revisas tu cuenta bancaria y decides si te alcanza para comprar un nuevo gadget; aquí solo multiplicas la escala… ¡y el drama!

## ¿Cómo puedo usar este repositorio? (Usage)

1. **Explora el notebook** (`a4658fee-0069-4901-a069-98478dfab54c.ipynb`) para ver cómo se cargan los datos, se entrenan los modelos y se calculan las ganancias y riesgos. Las celdas están comentadas y contienen bloques de **validación y feedback** de un revisor (¡sí, alguien te acompaña en el camino!).
2. **Ejecuta el código** en tu entorno favorito de Jupyter Notebook o colab. Recuerda que los datasets están disponibles en la ruta `/datasets/` (la carpeta tiene los archivos `geo_data_0.csv`, `geo_data_1.csv` y `geo_data_2.csv`).
3. **Replica el análisis o modifica parámetros**. ¿Quieres probar con otro umbral de rentabilidad? Adelante, solo cambia las variables. ¿Prefieres probar otro modelo? ¡Ten en cuenta que la instrucción oficial es usar regresión lineal, pero no se puede detener tu curiosidad!

## Conexiones con la vida diaria

- **Comparando regiones es como elegir aguacates en el mercado:** Miras tres puestos de frutas y de cada uno vas palpando para encontrar los aguacates más maduros. Solo comprarás los que se sienten firmes y prometen un buen guacamole (los pozos con más reservas). Si una caja entera parece floja, mejor la dejas.
- **El umbral de 111,1 unidades es tu presupuesto de la quincena:** Si gastas más de lo que ganas, te vas a endeudar. Así que marcas un mínimo que necesitas para no terminar comiendo maruchan el resto del mes.
- **Bootstrapping es jugar muchas partidas de lotería:** Compras miles de boletos (muestras aleatorias) y ves cuántas veces ganas o pierdes. Te ayuda a estimar tu suerte… o en este caso, el riesgo de que la inversión salga mal.

## Créditos y agradecimientos

Este proyecto forma parte del **Sprint 11** del programa de entrenamiento. Fue revisado por *Hesus Garcia*, un revisor que se toma muy en serio la calidad del código y te dejó valiosos comentarios en el notebook. Su guía hace que este repo no sea solo un montón de números, sino una historia de aprendizaje y mejora continua.

---

¿Listo para perforar datos y encontrar oro negro? 💪🏻🛢️
