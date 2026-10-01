# Cuestionario interactivo de Mecánica de Fluidos

**Cuestionario interactivo de Ecuación general y Pérdidas primarias de energía de un fluido**  
Curso de Mecánica de Fluidos  
Profesor: Ph. D. Juan Sandoval Herrera  
Universidad de América · 2026

## Revisión de notación y dificultad

- Fórmulas compuestas con **LaTeX y KaTeX**, con subíndices reales, fracciones, exponentes y unidades en letra recta. Se aplica a enunciados, opciones, explicaciones, fórmulas de consulta e impresión/PDF.
- Se sustituyeron los cálculos extensos por **operaciones breves**, valores sencillos y comparaciones conceptuales. No se pide resolver Colebrook iterativamente ni evaluar numéricamente los logaritmos y potencias decimales de Haaland.
- Ejemplos: carga de presión con 50 ÷ 10; balance de cargas con 4 + 2 + 1; conversión directa de 1 L/s a m³/s; conversión de Fanning a Darcy con una multiplicación por cuatro.
- **Se mantienen las 50 preguntas del banco y las 30 aleatorias por intento. No se añadió temporizador ni un modo de tres preguntas.**
- La tipografía matemática y sus fuentes están incorporadas en el HTML: no necesitan internet.

## Uso inmediato

Abra **index.html** en un navegador actualizado. Es una aplicación de una sola página, autónoma: no necesita instalación, descargas adicionales, conexión a internet ni servidor para responder y evaluar. Los enlaces a las cuatro fuentes sí requieren conexión.

El nombre es opcional y se usa únicamente en el informe del intento. No hay registro, envío de datos, almacenamiento permanente ni conexión a una plataforma de calificaciones.

## Publicarlo con un enlace en GitHub Pages

1. En GitHub, cree un repositorio público, por ejemplo **CuestionarioEGE**. Suba **index.html** directamente a la raíz del repositorio, no dentro de otra carpeta. No necesita subir los demás archivos para que funcione.
2. Abra **Settings → Pages**. En **Build and deployment**, seleccione **Deploy from a branch**, la rama **main** y la carpeta **/(root)**. Guarde.
3. Cuando GitHub termine de publicar, copie el enlace que aparece en Pages y compártalo con sus estudiantes.

Si el propietario es `juansanher25` y el repositorio se llama exactamente `CuestionarioEGE`, la dirección esperada después de publicarlo será:

`https://juansanher25.github.io/CuestionarioEGE/`

**Esta es una dirección propuesta, no un sitio que ya se haya publicado desde esta entrega.** La vista previa de esta conversación sirve para probar la aplicación; el enlace permanente se obtiene al publicarla en su cuenta.

## Funcionamiento académico

- Banco de **50 preguntas**, todas con cuatro opciones y una sola correcta.
- **25 básicas y 25 de nivel medio**.
- Cinco temas con 10 preguntas cada uno: ecuación de energía; aplicaciones del balance; pérdidas y Darcy; régimen y propiedades; modelos y calculadora.
- Cada ingreso, recarga o nuevo intento selecciona **30 preguntas**: 3 básicas y 3 de nivel medio por tema. Total: 15 básicas y 15 de nivel medio.
- Tanto las preguntas como sus opciones se mezclan. No hay duplicados dentro del intento. Diferentes intentos pueden compartir preguntas; la selección aleatoria no garantiza 30 preguntas completamente distintas cada vez.
- La opción se registra al pulsar **Confirmar respuesta**. Después queda bloqueada y se explican las cuatro opciones.
- Se puede saltar preguntas y volver a ellas mediante el mapa de navegación.
- Al finalizar: cada acierto suma 1 punto; una respuesta incorrecta o sin confirmar suma 0. Una opción seleccionada pero no confirmada se considera omitida.
- El porcentaje siempre se calcula sobre las **30 preguntas**, no solo sobre las contestadas.
- El informe incluye aciertos, errores, omisiones, desempeño por tema, equivalencia orientativa sobre 5 y recomendaciones de estudio. No define una nota oficial ni un umbral de aprobación.
- Descriptores del porcentaje mostrado: ≥85% criterio sólido; de 70 a menos de 85% buen camino; de 50 a menos de 70% base en construcción; menos de 50% volver a los fundamentos.

## Conservar los resultados

Al terminar, pulse **Imprimir / guardar PDF** y elija “Guardar como PDF” en el navegador. La impresión abre todas las explicaciones y contiene las 30 preguntas, aunque se estuviera usando un filtro de revisión. También puede descargar un **CSV** con el resultado y las respuestas del intento, compatible con hojas de cálculo. El CSV usa notación lineal de texto (por ejemplo, `p_(abajo)`) porque ese formato no conserva tipografía matemática; el HTML y el PDF sí la conservan.

En visores incrustados, el navegador puede restringir impresión, descargas o enlaces externos. Para usar esas funciones sin las restricciones del visor, abra la vista previa web o descargue `index.html` y ábralo directamente en su navegador.

**Recargar la página, salir y volver a ingresar o iniciar un intento nuevo reemplaza el intento anterior.** Descargue el informe antes si desea conservarlo. No se envía automáticamente al profesor.

## Convenciones y revisión de fuentes

La ecuación utilizada es:

**E₁ + hₐ − hᵣ − hL = E₂**, donde **E = p/γ + v²/(2g) + z**.

La bomba añade energía y la turbina la retira, con hₐ y hᵣ como magnitudes positivas. La ecuación visible del taller de ejercicios presenta el término hᵣ con un signo distinto al de la presentación principal cuando está en el miembro derecho. El cuestionario usa la convención física consistente de la presentación principal: **E₁ + hₐ = E₂ + hᵣ + hL**.

Se sigue la forma simplificada de la carga cinética de las SPA, v²/(2g), sin evaluar factores de corrección cinética. Para Reynolds se adopta el criterio 2000/4000 de los materiales: laminar por debajo de 2000, transición de 2000 a 4000 incluidos y turbulento por encima de 4000. Se utiliza el factor de **Darcy**, no el de Fanning. Las propiedades numéricas válidas para cada ejercicio aparecen en su enunciado.

Hazen–Williams se trata como una correlación empírica para agua en régimen turbulento y dentro de su rango orientativo; no produce un factor de Darcy ni representa una corrección de seguridad sobre Darcy. Se diferencia la pérdida de presión por fricción del cambio total de presión y la potencia para compensar fricción de la potencia total de una bomba.

Las preguntas son una adaptación didáctica original de los conceptos y ejemplos; no una transcripción íntegra. Algunas cifras se simplificaron. La ventana **Fuentes y criterios** y las explicaciones vinculan los contenidos con las aplicaciones:

1. https://juansanher25.github.io/Genenergyequation/
2. https://juansanher25.github.io/EjerciciosEGE/
3. https://juansanher25.github.io/Primaryenergylosses/
4. https://juansanher25.github.io/Primary_Loss_energy_calculator/

## Archivos y mantenimiento opcional

- **index.html**: cuestionario completo; es el único archivo necesario para usarlo o publicarlo.
- **banco_preguntas.json**: banco editorial de 50 preguntas con opciones, claves, explicaciones y referencias.
- **plantilla.html**: interfaz antes de incorporar el banco.
- **regenerar.py**: herramienta opcional, solo para editar el recurso.
- **recursos/**: motor KaTeX, auto-renderizado, estilos con fuentes incrustadas y licencia MIT. Solo se requiere esta carpeta para regenerar el archivo; el HTML publicado es autónomo.
- **LEEME.md**: esta guía.

Para modificar preguntas, edite `banco_preguntas.json`. Las expresiones matemáticas se escriben en LaTeX entre `\(` y `\)`. Dentro del JSON, las barras invertidas se duplican. Por ejemplo, un texto guardado como `"\\(h_L=2\\,\\mathrm{m}\\)"` se muestra como una ecuación con subíndice y unidades, no como código fuente. El campo `correct` es el índice de la respuesta correcta, empezando por 0. Cada opción contiene `text` (texto) y `why` (explicación). Mantenga los cinco temas y cinco preguntas de cada nivel por tema. **Editar el JSON por sí solo no cambia el HTML ya generado.** Con Python 3 instalado, ejecute en la misma carpeta:

```bash
python regenerar.py
```

Se regenerará `index.html` con el banco actualizado. Para modificar el diseño, edite `plantilla.html` y ejecute también el regenerador. No necesita instalar paquetes de Python.

## Comprobaciones de esta entrega

Se verificaron 1000 selecciones aleatorias (30 preguntas únicas, 15 por nivel y 6 por tema); en ese conjunto aparecieron las 50 preguntas del banco. Se probó una evaluación con 15 aciertos, 5 errores y 10 omisiones, el bloqueo al confirmar, los filtros del informe, la exportación CSV y PDF, el reinicio y la apertura local sin solicitudes de recursos externos. En esta revisión se validó la composición de 304 expresiones matemáticas del banco. Se comprobaron las 50 preguntas, con sus explicaciones, en anchos de 320, 390 y 1300 píxeles, sin desbordamiento horizontal. Se volvieron a probar puntuación, descarga CSV, impresión/PDF y funcionamiento sin conexión.

Este recurso está pensado para práctica y evaluación formativa. Al funcionar íntegramente en el navegador, las claves están incluidas en el archivo. No debe usarse como sistema de examen supervisado de alta seguridad.
