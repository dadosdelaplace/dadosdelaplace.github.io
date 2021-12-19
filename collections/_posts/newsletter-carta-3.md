---
header_type: "hero"
header_img : "https://as01.epimg.net/diarioas/imagenes/2021/09/26/actualidad/1632652327_985785_1632686173_noticia_normal.jpg"
title: "Carta #3: ¿qué sucedió en Alemania?"
subtitle: "Elecciones alemanas. Cambia, todo cambia...¿o no?"
last_modified_at: 2021-12-18
tags: [dataviz, R, datos electorales, mapas]
categories: [Cartas de Laplace (newsletter)]
---

La **elección del lenguaje** es una de las **preguntas más habituales** que recibimos muchos/as de los/as que nos dedicamos al **análisis de datos y la divulgación estadística** en redes: de todo el vasto universo de lenguajes de programación, **¿cuál elegir?**

Y te voy a decepcionar con la respuesta: depende.
![image](https://user-images.githubusercontent.com/26646492/146410201-d58d1c02-fc1a-4aaa-86a5-2c751d8f7a47.png)

El propósito de esta entrada no es hacer una disertación sobre el mundo de la programación sino servir de guía a un usuario muggle para elegir entre los **tres lenguajes más comunes en la ciencia (sin requerir grandes conocimientos de informática)**: ¿`R`, `Python` o `Matlab`?

* ¿Necesito una ejecución rápida (tareas diarias iguales, por ejemplo)?
* ¿Estoy dispuesto a sacrificar tiempo en ejecución a cambio de una curva de aprendizaje más rápida y un tiempo en la programación más corto?

Aunque los **tres lenguajes son diferentes entre sí**, he optado por ellos ya que comparten una virtud: son **lenguajes de alto nivel**. Como regla general, los lenguajes de alto nivel suelen ser **más lentos en ejecución pero mucho más cómodos y sencillos para un usuario medio**, mientras que lenguajes de bajo nivel son mucho más rápidos en ejecución, pero requieren de un mayor conocimiento informático. Y aunque algunos científicos con conocimientos en programación siguen optando por los lenguajes de bajo nivel, la mayoría de la comunidad científica empiezan a apostar en sus análisis por lenguajes que puedan aprender rápido, al no requerir en general de una gran eficiencia en tiempos de ejecución (sacrificando algunos segundos o minutos en la ejecución, a cambio de poder ser más o menos **autosuficientes en su programación**).

## Consejo: descarta Matlab, apuesta por el software libre

Debido a su potencia, seguramente si eres un usuario medio que necesita cosas sencillas para el análisis de datos, las tres herramientas te puedan cubrir la mayoría de tus necesidades. Sin embargo, hay un aspecto que diferencia `Matlab` (M) de los otros dos lenguajes: **Matlab es de pago**. Como sucede con lenguajes/herramientas como `SPSS` (IBM) o `SAS`, `Matlab` **requiere de una licencia de pago**. Esta desventaja a priori puede que no nos parezca relevante a la hora de decidirnos por un lenguaje de programación, ya que probablemente lo hayas podido usar de forma «gratuita», bien porque hayas encontrado una forma de piratearlo, bien porque tengas acceso a una licencia académica o corporativa, siendo tu universidad o empresa la que tenga un acuerdo de licencias.

**¿Es entonces una desventaja real?** Sí, pero no por el precio que tengas que pagar por su uso, sino por lo que ello implica: **su código no es de libre uso**. Matlab, como todos los programas de software de pago, son de código cerrado, lo que impide acceder fácilmente a la totalidad del código de las funciones internas del lenguaje, lo cual a su vez impide la colaboración entre usuarios: Matlab no permite la instalación directa de código validado por la comunidad de usuarios (puedes copiar y pegar código que encuentres en la red, pero sin tener una garantía de que realiza lo que promete, ni de compatibilidad, ni de integración, ni de documentación).

Otra aspecto diferencial para descartar Matlab es que, como probablemente hayas experimentado si has trabajado con dicha herramienta, tiene un **alto consumo de recursos**. No solo consume una monstruosa cantidad de espacio en el disco duro tras sus instalación (mientras que instalar R puede ocupar 100MB, una instalación de Matlab puede superar los 5GB), sino que además consume una gran cantidad de memoria RAM en su ejecución: es una herramienta tan potente pero tan rígida en su configuración que «por si lo necesitases» implementa toda una **compleja infraestructura**.

Y es que precisamente una de las desventajas (en mi opinión) de `Matlab`, aunque pueda parecer contradictorio, es su propósito general, ya que pretende abarcar tantos campos que, salvo necesidades muy especiales donde no hay competidor (modelización y simulación de ecuaciones diferenciales y cálculo matricial, entre ellas, no es casualidad que se llame MATrix LABoratory), seguramente puedas encontrar otro lenguaje o software libre cuyas funcionalidades sean más acordes y específicas a tu necesidad.

 
## ¿R o Python?

Se acabó el hype, vamos a pinchar la burbuja: **ambos son válidos para el análisis de datos**.

En mi caso particular, durante la carrera aprendí lenguajes como `C++`, `FORTRAN`, `PASCA`L o `Java`, mi TFM lo realicé en `Python` y mi tesis doctoral la hice entera en `Matlab`, por lo que no fue hasta finalizar la tesis (julio de 2018) cuando empecé a programar más intensamente en `R`, así que se podría decir que es el lenguaje que menos horas he dedicado (pero en el que más he producido, curiosamente). Y es que mientras que `Python` es un lenguaje de un propósito mucho más general, `R` fue diseñado por y para matemáticos y estadísticos, y se nota desde la propia arquitectura del lenguaje. Obviamente este objetivo tan específico tiene una desventaja: por regla general, `Python` es más eficiente (con tiempos de ejecución más cortos), y está dotado de una mayor flexibilidad para el desarrollo web, la Inteligencia Artificial, el preprocesamiento de imágenes o la integración con todo tipo de apps o programas (incluso con herramientas de edición de audio y vídeo de la saga Adobe).

Ambos tienen tres ventajas que los hacen muy difícil de superar en el ámbito del análisis de datos:

* **Software libre**, con una inmensa comunidad de usuarios produciendo y validando código: seguramente lo que necesites ya haya sido implementado (en su totalidad o de forma parcial) por alguien antes y solo necesites adaptarlo.

* **Fácil integración de otros lenguajes** para tareas más tediosas y costosas (como la programación en paralelo).

* **Modulares**: su instalación básica ocupa muy poco espacio, y mediante la instalación de paquetes (`R`) o librerías (`Python`), permiten su configuración totalmente adaptada a nuestras necesidades.

Dada su **flexibilidad y potencia**, ambos seguramente cubran tus necesidades en cuanto a análisis de datos se refiere, por lo que **si ya has empezado con alguno de ellos, mi consejo es que sigas con el lenguaje que te resulte más cómodo**, y del que tengas ya cierta base. Sin embargo, si estás partiendo de cero, mi recomendación (para el análisis de datos) es sin duda `R` ya que cuenta con tres ventajas frente a `Python`:

* En lo referente al análisis de datos y la estadística,  cuenta una **mayor comunidad de usuarios**, por lo que tendrás a tu disposición una mayor variedad de paquetes y de soporte en la web.
