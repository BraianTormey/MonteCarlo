# Guion de Presentación: Simulación de Montecarlo
## Grupo 2: Braian Tormey, Dante Passone, Matias Martinez

---

## SLIDE 1: Presentación del Equipo
**Acción:** Reproducir audio intro (botón play)
- Esperar 44 segundos (overlay oscuro)
- Mostrar slide con fondo de fuego

**Hablar:**
- "Buenos días/tardes. Somos el Grupo 2."
- Presentar a cada integrante
- "Hoy vamos a hablar sobre Simulación de Montecarlo"

---

## SLIDE 2: Introducción

### 2.1: Título
**Hablar:**
- "Vamos a ver qué es la Simulación de Montecarlo"

### 2.2: ¿Qué es?
**Hablar:**
- "La Simulación de Montecarlo es una técnica matemática que se utiliza para estimar los posibles resultados de un evento incierto."
- "Es muy útil cuando tenemos situaciones con mucha incertidumbre."

### 2.3: Historia
**Hablar:**
- "Fue inventada por John von Neumann y Stanislaw Ulam durante la Segunda Guerra Mundial."
- "Debe su nombre al famoso casino de Montecarlo en Mónaco, ya que el elemento de azar es fundamental, similar a los juegos del casino."

---

## SLIDE 3: Aplicaciones
**Hablar:**
- "Esta técnica tiene muchas aplicaciones prácticas:"
- Mencionar cada una:
  - Finanzas: evaluar riesgos y estimar ganancias o pérdidas
  - Ingeniería: optimizar procesos y medir confiabilidad
  - Ciencias: simular fenómenos físicos, climáticos o biológicos
  - Computación/Juegos/IA: estrategias y comportamientos aleatorios

---

## SLIDE 4: Conceptos Matemáticos y Estadísticos

### 4.1: Conceptos básicos
**Hablar:**
- "Antes de ver ejemplos, necesitamos entender algunos conceptos:"
- **Variable Aleatoria:** "Es aquella cuyo valor depende del azar."
- **Distribución de Probabilidad:** "Describe cómo se comportan los valores de una variable aleatoria."

### 4.2: Distribución Normal
**Hablar:**
- "Tiene forma de campana. La mayoría de los valores se concentran cerca del promedio."

### 4.3: Distribución Uniforme
**Hablar:**
- "Todos los valores tienen la misma probabilidad. No hay preferencia por ningún número."

### 4.4: Promedio y Desviación Estándar
**Hablar:**
- **Promedio:** "Representa el resultado esperado."
- **Desviación Estándar:** "Representa el riesgo o la incertidumbre."

### 4.5: Rigor Estadístico
**Hablar:**
- **Rigor:** "Definir bien las variables, hacer suficientes iteraciones, analizar correctamente."
- **Muestra:** "Conjunto de datos que usamos para hacer estimaciones."

### 4.6: Confianza y Error
**Hablar:**
- **Confianza:** "Qué tan seguros estamos de nuestra estimación."
- **Error:** "Puede reducirse aumentando el tamaño de la muestra y la precisión del modelo."

### 4.7: Ley de los Grandes Números
**Hablar:**
- "Cuando repetís un experimento aleatorio muchas veces, el promedio se acerca cada vez más al valor real esperado."
- "Esto es clave para entender por qué funcionan las simulaciones de Montecarlo."

---

## SLIDE 5: Pasos para realizar una simulación
**Hablar:**
- "Para hacer una simulación de Montecarlo seguimos estos pasos:"
- Leer cada paso:
  1. Definir el problema
  2. Definir los datos de entrada
  3. Generar valores aleatorios
  4. Ejecutar múltiples simulaciones
  5. Analizar los resultados

---

## SLIDE 6: Ejemplo 1 - Lanzamiento de Moneda

### 6.1: Imagen de moneda
**Hablar:**
- "Vamos a ver nuestro primer ejemplo práctico: lanzar una moneda."

### 6.2: Simulación Interactiva
**Acción:** Mostrar simulación interactiva

**Hablar:**
- "Este gráfico muestra cómo la proporción acumulada de caras se estabiliza alrededor del 50%."
- "Cada lanzamiento puede resultar en cara (valor 1) o cruz (valor 0), cada uno con 50% de probabilidad."
- "Vamos a hacer una demostración en vivo."

**INTERACCIÓN CON AUDIENCIA:**
- "¿Quién quiere participar? Vamos a lanzar una moneda varias veces."
- Repartir monedas y papeles para anotar
- "Vamos a lanzar la moneda [X] veces y anotar cuántas veces sale cara."
- "Después vamos a calcular la proporción y ver cómo se acerca al 50%."
- Comparar con la simulación en pantalla

**Hablar:**
- "Como pueden ver, a medida que aumentamos el número de lanzamientos, la proporción se estabiliza alrededor del 50%."
- "Esto es la Ley de los Grandes Números en acción."

---

## SLIDE 7: Ejemplo 2 - Juego de Dados

### 7.1: Imagen de dados
**Hablar:**
- "Ahora vamos a un ejemplo más complejo: un juego con dados."

### 7.2: Explicación del juego
**Hablar:**
- "Queremos estimar el valor esperado de un juego donde:"
- "Se tiran dos dados."
- "Si salen dobles → ganás 100 × (producto de los dados)."
- "Si NO salen dobles → perdés 200 dólares."
- "¿Es un juego conveniente o desfavorable a largo plazo?"

**INTERACCIÓN CON AUDIENCIA:**
- "Para comprobarlo, trajimos algunos dados."
- Repartir dados y papeles
- "Intenten sacar unos dobles. Tiren los dados varias veces y anoten los resultados."
- "¿Cuántas veces salieron dobles? ¿Cuántas veces no?"
- "Ahora, díganos: ¿les parece un juego conveniente o desfavorable?"

**Hablar:**
- "Vamos a verlo analíticamente y luego con una Simulación Monte Carlo."

### 7.3: Probabilidades y Valor Esperado
**Hablar:**
- Mostrar la tabla con las probabilidades
- "Como pueden ver, hay 6 formas de sacar dobles, cada una con probabilidad 1/36."
- "Y 30 formas de NO sacar dobles, con probabilidad 30/36."
- "El valor esperado total es aproximadamente 86.11 dólares."
- "Esto significa que, a largo plazo, el juego es conveniente para el jugador."

### 7.4: Código Python (opcional)
**Hablar:**
- "Veamos cómo se implementa esto en código Python."
- Explicar brevemente el código si hay tiempo

### 7.5: Simulación Interactiva
**Acción:** Mostrar simulación interactiva

**Hablar:**
- "Ahora vamos a simular este juego muchas veces."
- "Pueden cambiar el número de partidas y ver cómo el valor esperado se acerca a 86.11 dólares."
- "A mayor número de simulaciones, más preciso será el resultado."
- "Esto demuestra el poder de la Simulación de Montecarlo."

---

## SLIDE 8: Conclusiones

### 8.1: Conclusiones generales
**Hablar:**
- "La simulación de Monte Carlo permite entender mejor la variabilidad, el riesgo y la incertidumbre en problemas complejos."
- "Siempre que se aplique con rigor estadístico, es una herramienta muy poderosa."

### 8.2: Ventajas
**Hablar:**
- "Las ventajas incluyen:"
- Leer cada ventaja

### 8.3: Desventajas
**Hablar:**
- "Pero también tiene sus limitaciones:"
- Leer cada desventaja

---

## SLIDE 9: Fuentes (imágenes)
**Hablar:**
- "Estas son algunas fuentes de las ciudades que visitamos durante nuestra investigación."
- Mostrar imágenes de las fuentes

---

## SLIDE 10: Fuentes (enlaces)
**Hablar:**
- "Y estas son nuestras fuentes bibliográficas."
- Mencionar brevemente las fuentes principales

---

## SLIDE 11: Pregunta para reflexionar
**Hablar:**
- "Para terminar, les dejamos una pregunta para reflexionar:"
- **"¿Qué estará haciendo J2?"**
- Pausa para reflexión
- "Muchas gracias por su atención."

**Acción:** Esperar 10 segundos y reproducir audio de aplausos

---

## NOTAS ADICIONALES

### Materiales necesarios:
- Monedas (para Ejemplo 1)
- Dados (para Ejemplo 2)
- Papeles para anotar resultados
- Lápices/bolígrafos

### Tiempo estimado:
- Presentación completa: ~20-25 minutos
- Incluyendo interacciones: ~30-35 minutos

### Puntos clave a enfatizar:
1. La Ley de los Grandes Números es fundamental
2. Más simulaciones = mayor precisión
3. El rigor estadístico es esencial
4. Las simulaciones son herramientas, no respuestas absolutas

### Tips para la presentación:
- Mantener contacto visual con la audiencia
- Hacer pausas después de conceptos importantes
- Invitar a preguntas durante las interacciones
- Usar la simulación interactiva para demostrar conceptos en tiempo real
- Relacionar los ejemplos con situaciones reales cuando sea posible

