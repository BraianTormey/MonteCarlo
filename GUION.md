# Guion de Presentación: Simulación de Montecarlo
## Grupo 2: Braian Tormey, Dante Passone, Matias Martinez

**SLIDE 1: Presentación del Equipo**

Reproducir audio intro (botón play)

Entrar cuando en el audio salgan nuestros nombres

El fondo de fuego se muestra automáticamente

Pasar a la slide 2 después de los aplausos

**SLIDE 2: Introducción**

**2.1: Título**

"Vamos a ver qué es la Simulación de Montecarlo"

"Esta es una técnica que combina matemática, estadística y computación para resolver problemas complejos."

**2.2: ¿Qué es?**

"La Simulación de Montecarlo es una técnica matemática que se utiliza para estimar los posibles resultados de un evento incierto."

"Es muy útil cuando tenemos situaciones con mucha incertidumbre."

**2.3: Historia**

"Fue inventada por John von Neumann y Stanislaw Ulam durante la Segunda Guerra Mundial."

"Debe su nombre al famoso casino de Montecarlo en Mónaco, ya que el elemento de azar es fundamental, similar a los juegos del casino."

**SLIDE 3: Aplicaciones**

"Esta técnica tiene muchas aplicaciones prácticas:"

**Finanzas:** evaluar riesgos y estimar ganancias o pérdidas

**Ingeniería:** optimizar procesos y medir confiabilidad

**Ciencias:** simular fenómenos físicos, climáticos o biológicos

**Computación/Juegos/IA:** estrategias y comportamientos aleatorios

**SLIDE 4: Conceptos Matemáticos y Estadísticos**

**4.1: Conceptos básicos**

"Antes de ver ejemplos, necesitamos entender algunos conceptos:"

**Variable Aleatoria:** "Es aquella cuyo valor depende del azar."

**Distribución de Probabilidad:** "Describe cómo se comportan los valores de una variable aleatoria."

**4.2: Distribución Normal**

"Tiene forma de campana. La mayoría de los valores se concentran cerca del promedio."

**4.3: Distribución Uniforme**

"Todos los valores tienen la misma probabilidad. No hay preferencia por ningún número."

**4.4: Promedio y Desviación Estándar**

**Promedio:** "Representa el resultado esperado."

**Desviación Estándar:** "Representa el riesgo o la incertidumbre."

**4.5: Rigor Estadístico**

**Rigor:** "Definir bien las variables, hacer suficientes iteraciones, analizar correctamente."

**Muestra:** "Conjunto de datos que usamos para hacer estimaciones."

**4.6: Confianza y Error**

**Confianza:** "Qué tan seguros estamos de nuestra estimación."

**Error:** "Puede reducirse aumentando el tamaño de la muestra y la precisión del modelo."

**4.7: Ley de los Grandes Números**

"Cuando repetís un experimento aleatorio muchas veces, el promedio se acerca cada vez más al valor real esperado."

"Esto es clave para entender por qué funcionan las simulaciones de Montecarlo."

**SLIDE 5: Pasos para realizar una simulación**

"Para hacer una simulación de Montecarlo seguimos estos pasos:"

1. **Definir el problema**
2. **Definir los datos de entrada**
3. **Generar valores aleatorios**
4. **Ejecutar múltiples simulaciones**
5. **Analizar los resultados**

"Vamos a ver cómo aplicamos estos pasos en nuestros ejemplos prácticos."

**SLIDE 6: Ejemplo 1 - Lanzamiento de Moneda**

**6.1: Imagen de moneda**

"Vamos a ver nuestro primer ejemplo práctico: lanzar una moneda."

**6.2: Simulación Interactiva**

Mostrar simulación interactiva

"Este gráfico muestra cómo la proporción acumulada de caras se estabiliza alrededor del 50%."

"Cada lanzamiento puede resultar en cara (valor 1) o cruz (valor 0), cada uno con 50% de probabilidad."

"Vamos a hacer una demostración en vivo."

**INTERACCIÓN CON AUDIENCIA:**

"¿Quién quiere participar? Vamos a lanzar una moneda varias veces."

Repartir monedas y papeles para anotar

"Vamos a lanzar la moneda 20-30 veces y anotar cuántas veces sale cara y cuántas cruz."

"Después vamos a calcular la proporción y ver cómo se acerca al 50%."

Comparar con la simulación en pantalla

"Noten cómo, con pocos lanzamientos, la proporción puede variar mucho, pero con más lanzamientos se estabiliza."

**CONCEPTOS APLICADOS EN ESTE EJEMPLO:**

"En este ejemplo aplicamos varios conceptos que vimos antes:"

"**Variable Aleatoria:** el resultado de cada lanzamiento (cara o cruz) es una variable aleatoria, porque depende del azar."

"**Distribución Uniforme:** cada resultado tiene exactamente 50% de probabilidad, es decir, una distribución uniforme."

"**Ley de los Grandes Números:** como pueden ver, a medida que aumentamos el número de lanzamientos, la proporción se estabiliza alrededor del 50%. Esto es la Ley de los Grandes Números en acción."

"**Muestra:** cada conjunto de lanzamientos que realizamos es una muestra que nos permite estimar la probabilidad real."

"**Promedio:** la proporción acumulada que calculamos es el promedio de caras en nuestros lanzamientos."

"**Rigor Estadístico:** para obtener resultados confiables, necesitamos hacer suficientes lanzamientos. Con pocos lanzamientos, el error puede ser grande, pero con más lanzamientos, el error se reduce."

**SLIDE 7: Ejemplo 2 - Juego de Dados**

**7.1: Imagen de dados**

"Ahora vamos a un ejemplo más complejo: un juego con dados."

**7.2: Explicación del juego**

"Queremos estimar el valor esperado de un juego donde:"

"Se tiran dos dados."

"Si salen dobles → ganás 100 × (producto de los dados)."

"Si NO salen dobles → perdés 200 dólares."

"¿Es un juego conveniente o desfavorable a largo plazo?"

**INTERACCIÓN CON AUDIENCIA:**

"Para comprobarlo, trajimos algunos dados."

Repartir dados y papeles

"Intenten sacar unos dobles. Tiren los dados varias veces y anoten los resultados."

"¿Cuántas veces salieron dobles? ¿Cuántas veces no?"

"Ahora, díganos: ¿les parece un juego conveniente o desfavorable?"

"Vamos a verlo analíticamente y luego con una Simulación Monte Carlo."

**7.3: Probabilidades y Valor Esperado**

Mostrar la tabla con las probabilidades

"Como pueden ver, hay 6 formas de sacar dobles, cada una con probabilidad 1/36."

"Y 30 formas de NO sacar dobles, con probabilidad 30/36."

"El valor esperado total es aproximadamente 86.11 dólares."

"Esto significa que, a largo plazo, el juego es conveniente para el jugador."

**CONCEPTOS APLICADOS EN ESTA PARTE:**

"En esta tabla aplicamos varios conceptos:"

"**Variable Aleatoria:** la ganancia o pérdida del juego es nuestra variable aleatoria, porque depende del resultado aleatorio de los dados."

"**Distribución de Probabilidad:** esta tabla muestra la distribución de probabilidad completa del juego. Cada evento tiene su probabilidad asociada."

"**Promedio/Valor Esperado:** el valor esperado de 86.11 dólares es el promedio que esperamos obtener a largo plazo. Este es el concepto de promedio que vimos antes."

**7.4: Código Python (opcional)**

"Veamos cómo se implementa esto en código Python."

Explicar brevemente el código si hay tiempo

**7.5: Simulación Interactiva**

Mostrar simulación interactiva

"Ahora vamos a simular este juego muchas veces."

"Pueden cambiar el número de partidas y ver cómo el valor esperado se acerca a 86.11 dólares."

"A mayor número de simulaciones, más preciso será el resultado."

"Esto demuestra el poder de la Simulación de Montecarlo."

**CONCEPTOS APLICADOS EN LA SIMULACIÓN:**

"En esta simulación interactiva aplicamos todos los conceptos que vimos:"

"**Ley de los Grandes Números:** más simulaciones = resultado más cercano al valor esperado real. Esto es la Ley de los Grandes Números en acción."

"**Muestra:** cada conjunto de N partidas es una muestra que nos permite estimar el valor esperado. A mayor tamaño de muestra, mejor nuestra estimación."

"**Promedio:** el valor esperado que calculamos es el promedio de todas las partidas simuladas."

"**Rigor Estadístico:** para obtener resultados confiables, necesitamos hacer suficientes simulaciones. Con pocas simulaciones, el error puede ser grande, pero con más simulaciones, el error se reduce."

"**Confianza:** a mayor número de simulaciones, mayor confianza tenemos en que nuestro resultado está cerca del valor real esperado."

"**Error:** el error es la diferencia entre nuestro resultado simulado y el valor esperado real (86.11). Este error se reduce aumentando el tamaño de la muestra, es decir, haciendo más simulaciones."

**SLIDE 8: Conclusiones**

**8.1: Conclusiones generales**

"La simulación de Monte Carlo es una herramienta poderosa que nos permite estimar resultados en situaciones de incertidumbre mediante la repetición de experimentos aleatorios."

"Como vimos en los ejemplos, a mayor número de simulaciones, más precisos serán nuestros resultados, demostrando la Ley de los Grandes Números en acción."

"Sin embargo, es fundamental aplicarla con rigor estadístico para obtener conclusiones confiables."

**8.2: Ventajas**

"Las ventajas incluyen:"

Leer cada ventaja

**8.3: Desventajas**

"Pero también tiene sus limitaciones:"

Leer cada desventaja

**SLIDE 9: Fuentes (imágenes)**

"Estas son algunas fuentes. ¿Cuál es tu favorita?"

**SLIDE 10: Fuentes (enlaces)**

"Y estas son nuestras fuentes bibliográficas."

**SLIDE 11: Pregunta para reflexionar**

"Para terminar, les dejamos una pregunta para reflexionar:"

"¿Qué estará haciendo J2?"

"Muchas gracias por su atención."

Se reproduce automáticamente después de 10 segundos el audio de aplausos
