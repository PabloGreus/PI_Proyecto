# IA Bajo Control: de prompts débiles a profesionales

## 1. Título y portada breve

**IA Bajo Control: de prompts débiles a profesionales**

- Integrantes: Pablo Greus y Julián Leita.
- Centro: XTART Formación Profesional.
- Curso: 2º DAW.
- Grupo: [PENDIENTE: número de grupo; deben aportarlo Pablo Greus y Julián Leita].
- Módulo: 0616 Proyecto Intermodular.
- Evaluación: 1ª evaluación.
- Curso académico: 2026/2027.
- Docente: Esteban Castañer.

## 2. Descripción y objetivo del proyecto

Nuestra empresa ficticia será Gedes, una agencia de 20 personas que se dedican al Ecommerce. Necesitamos una web para poder realizar las ventas de los productos Tech (monitores, ratones, portátiles, etc). Identificamos tres necesidades: mostrar los servicios mediante la interfaz, que se busca algo claro y sencillo, poder organizar clientes, pedidos, productos, stock y pagos; y poder ofrecer un asesoramiento mediante un formulario con los campos de nombre, correo electrónico, fecha, hora y consulta.

El proyecto consiste en un banco de ocho prompts profesionales para tareas de desarrollo web y en la comparación de respuestas de dos herramientas por caso. Los ejemplos son demostrativos y utilizan datos ficticios. La memoria registra Gemini y Copilot en P01–P04 y Gemini y Claude en P05–P08.

## 3. Índice

- [IA Bajo Control: de prompts débiles a profesionales](#ia-bajo-control-de-prompts-débiles-a-profesionales)
  - [1. Título y portada breve](#1-título-y-portada-breve)
  - [2. Descripción y objetivo del proyecto](#2-descripción-y-objetivo-del-proyecto)
  - [3. Índice](#3-índice)
  - [4. Organización de archivos](#4-organización-de-archivos)
  - [5. Requisitos](#5-requisitos)
  - [6. Instrucciones de ejecución](#6-instrucciones-de-ejecución)
    - [P01 — Creación de una página web](#p01--creación-de-una-página-web)
    - [P02 — Revisión de JavaScript](#p02--revisión-de-javascript)
    - [P03 — Validación con PHP](#p03--validación-con-php)
    - [P04 — Base de datos relacional](#p04--base-de-datos-relacional)
    - [P05 — API](#p05--api)
    - [P06 — Diseño y accesibilidad](#p06--diseño-y-accesibilidad)
    - [P07 — Detección de errores](#p07--detección-de-errores)
    - [P08 — Documentación](#p08--documentación)
  - [7. Pruebas](#7-pruebas)
  - [8. Comparación de herramientas y decisiones](#8-comparación-de-herramientas-y-decisiones)
  - [9. Iteraciones](#9-iteraciones)
  - [10. Banco reutilizable](#10-banco-reutilizable)
    - [Plantilla de creación reutilizable](#plantilla-de-creación-reutilizable)
    - [Plantilla de revisión y corrección](#plantilla-de-revisión-y-corrección)
    - [Plantilla de documentación](#plantilla-de-documentación)
  - [11. Limitaciones y puntos pendientes](#11-limitaciones-y-puntos-pendientes)
  - [12. Control de versiones con Git](#12-control-de-versiones-con-git)
    - [Inicializar y registrar la primera versión](#inicializar-y-registrar-la-primera-versión)
    - [Guardar una revisión posterior](#guardar-una-revisión-posterior)
    - [Consultar el historial](#consultar-el-historial)
    - [Exportar el historial](#exportar-el-historial)
  - [13. Declaración de uso de IA](#13-declaración-de-uso-de-ia)

## 4. Organización de archivos

El árbol siguiente recoge archivos disponibles para redactar esta guía, sin proponer una estructura de carpetas que no se ha aportado. Los comentarios P01–P08 son identificadores documentales de esta guía, no nombres nuevos de archivos.

```text
10_2_DAW_P_I_Pablo_Greus_y_Julian_Leita(1).docx   # P01–P08: memoria actual
IA_Bajo_Control_Proyecto_Intermodular_DAW (2).pdf # Enunciado
tienda_online_gedes_b2b.html                     # P01
gedes_e_commerce_tech_b2b_y_b2c.html              # P06: Gemini
gedes_mejorado.html                             # P06: Claude
index.html                                     # P06: versión separada
styles.css                                     # P06: estilos de index.html
Markdown pegado.md                             # P05: respuesta de Claude
Markdown pegado(1).md                          # P07 y apoyo a P02: respuesta de Claude
README.md                                      # P08: esta guía
```

Nomenclatura del enunciado, reproducida literalmente:

```text
n.º de grupo_curso_ciclo_módulo_evaluación_título del proyecto
```

Ejemplo del enunciado, que no identifica el grupo de este equipo:

```text
03_2DAW_DAW_1Ev_IA_Bajo_Control
```

El enunciado pide el mismo nombre base para la memoria y el ZIP. No exige renombrar cada ejemplo con esa fórmula.

## 5. Requisitos

| Herramienta o recurso mencionado       | Uso documentado                                 |
| -------------------------------------- | ----------------------------------------------- |
| Navegador y herramientas de desarrollo | Interfaces, consola y Network                   |
| Visual Studio Code                     | Edición de ejemplos                             |
| XAMPP y Apache                         | Ejecución del formulario PHP                    |
| PHP                                    | Validación y API                                |
| MySQL o MariaDB con PDO                | Propuesta de API de pedidos                     |
| Git                                    | Registro y exportación del historial            |
| Gemini, Copilot y Claude               | Generación y comparación de respuestas          |
| ChatGPT                                | Apoyo en prompts, comparación y redacción       |
| Internet                               | JSONPlaceholder e imágenes externas             |
| curl                                   | Peticiones propuestas en la respuesta de la API |

La respuesta de la API menciona PHP 8.2; no acredita que sea la versión instalada por el equipo.

## 6. Instrucciones de ejecución

### P01 — Creación de una página web

Abrir `tienda_online_gedes_b2b.html` en el navegador. Revisar las secciones, el formulario y el listado ficticio. Las imágenes externas requieren conexión. El ejemplo es independiente de los demás casos.

### P02 — Revisión de JavaScript

El original está en el anexo 2.1 de la memoria actual. El formulario asociado debe conservar los identificadores del JavaScript. La respuesta de `Markdown pegado(1).md` contiene un HTML mínimo y un `app.js` corregido para P07, que reutiliza el fragmento de P02.

[PENDIENTE: guardar las versiones de P02 y su HTML asociado como archivos independientes, identificar la respuesta elegida y sus rutas; deben aportarlos Pablo Greus y Julián Leita].

No utilizar el `index.html` de P06 como si fuera el formulario de P02. Una vez guardado el HTML asociado, abrirlo en el navegador con consola y Network visibles y comparar original y corrección con la misma entrada. JSONPlaceholder simula el POST; no confirma reservas reales.

### P03 — Validación con PHP

Ejecutar mediante Apache de XAMPP. Iniciar Apache, colocar los archivos del ejemplo en su directorio de publicación y acceder mediante la dirección local correspondiente. No abrir PHP directamente ni utilizar Live Server.

### P04 — Base de datos relacional

Ejecutar el esquema SQL aportado para P04 en el gestor elegido, registrar su salida y comprobar las claves y restricciones con los datos de prueba del ejemplo.

### P05 — API

`Markdown pegado.md` contiene código por extraer a los archivos que la propia respuesta enumera: `public/.htaccess`, `public/index.php`, `src/ApiException.php`, `src/Database.php`, `src/PedidoService.php` y `sql/schema.sql`, dentro de `gedes-api/`.

Para esta entrega, la ejecución se realizará mediante Apache de XAMPP. Iniciar Apache y el gestor de base de datos; importar el esquema y sus datos de prueba; configurar la conexión conforme al entorno local y acceder al endpoint a través de Apache. No abrir PHP directamente ni utilizar Live Server.

[PENDIENTE: configuración comprobada de Apache para esta API, ruta publicada, URL del endpoint, configuración de reescritura y procedimiento de importación en el equipo; deben aportarlos Pablo Greus y Julián Leita].

La respuesta disponible aporta un arranque con el servidor integrado de PHP, que no acredita una configuración de Apache. No se proporcionan aquí una URL ni comandos de despliegue específicos sin evidencia. Repetir las peticiones de la respuesta usando la URL real una vez confirmada.

### P06 — Diseño y accesibilidad

- Gemini: abrir `gedes_e_commerce_tech_b2b_y_b2c.html`.
- Claude: abrir `gedes_mejorado.html`.
- Claude con archivos separados: mantener `index.html` y `styles.css` en la misma carpeta y abrir `index.html`.

Comprobar etiquetas, teclado, foco, contraste y adaptación móvil según las propuestas. Las imágenes externas requieren conexión.

### P07 — Detección de errores

La respuesta `Markdown pegado(1).md` contiene en su sección 2 el HTML mínimo y en su sección 3 el JavaScript corregido. Guardar el HTML como `index.html` y el JavaScript como `app.js` en una carpeta independiente de P06, respetando el enlace al script. Conservar el original del anexo 2.1 de la memoria en una versión identificada.

Abrir el formulario en el navegador, activar Network y Preserve log y reproducir la misma prueba antes y después de sustituir el JavaScript. Si se utiliza una versión intermedia para aislar fallos, conservarla con su identificación.

### P08 — Documentación

Abrir `README.md` en un editor compatible con Markdown. Contrastar el inventario con la carpeta de entrega y seguir las instrucciones de los ejemplos disponibles. Registrar revisiones reales con Git según la sección 12.

[PENDIENTE: comprobación independiente de las instrucciones y rutas del README en la carpeta final; deben aportarla Pablo Greus y Julián Leita].

## 7. Pruebas

Los resultados esperados por la IA no se presentan como resultados observados por el equipo. La memoria describe comparación de código con ChatGPT y pasos de prueba; no se aportan registros de ejecución suficientes para completar los resultados reales de esta tabla.

| Caso | Entrada o comprobación                                                | Resultado esperado por la IA o requisito de la consigna | Resultado observado por nosotros | Conclusión             |
| ---- | --------------------------------------------------------------------- | ------------------------------------------------------- | -------------------------------- | ---------------------- |
| P01  | Abrir interfaz y enviar formulario ficticio                           | Secciones y comportamiento descritos en su propuesta    | pendiente de comprobar           | pendiente de comprobar |
| P02  | Mismo formulario y datos en original y corregido; error HTTP o de red | Sin recarga en la corrección y manejo de errores        | pendiente de comprobar           | pendiente de comprobar |
| P03  | Una entrada válida y otra inválida                                    | Aceptación o rechazo según reglas del PHP               | pendiente de comprobar           | pendiente de comprobar |
| P04  | Registro válido y registro que vulnere una restricción                | Aceptación del válido y rechazo del inválido            | pendiente de comprobar           | pendiente de comprobar |
| P05  | Petición válida y cantidad negativa en la API de pedidos disponible   | La respuesta propone HTTP 201 y 422, respectivamente    | pendiente de comprobar           | pendiente de comprobar |
| P06  | Etiquetas, teclado, foco, contraste y móvil                           | Criterios de accesibilidad y diseño solicitados         | pendiente de comprobar           | pendiente de comprobar |
| P07  | Repetir un fallo del original tras corregirlo                         | Corrección demostrada mediante la misma prueba          | pendiente de comprobar           | pendiente de comprobar |
| P08  | Seguir README y revisar historial Git                                 | Ejecución reproducible y cambios trazables              | pendiente de comprobar           | pendiente de comprobar |

## 8. Comparación de herramientas y decisiones

| Caso | Decisión que expresa la memoria                         | Justificación literal de la memoria                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| ---- | ------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| P01  | Gemini                                                  | Preferimos el desarrollo que nos dio Gemini, ya que es una versión mas completa, tanto como interactiva, como visual, además, cumplía con las secciones y restricciones que se le han pedido con exactitud. Por último, hace uso de JavaScript, cuando era una de las restricciones.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| P02  | Preferencia por Gemini, sin elección técnica definitiva | Ambas respuestas siguieron el formato solicitado. No tenemos en claro cual fue la mejor respuesta o la más precisa según el prompt enviado, pero creemos que la de Gemini a nivel código y la manera que tiene de explicar las cosas, parecen ser más fácil de entender que la de Copilot que ejemplifico con casos aislados con código y nada más.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| P03  | Ambas consideradas correctas                            | Las dos respuestas son para que alguien aprenda y trate de implementarlo. La de Copilot es útil por su explicación inicial del flujo y la de Gemini por el orden que le da a los conceptos. Creemos que las dos son correctas, ya que Copilot te da un pantallazo inicial sobre los conceptos básicos y la otra herramienta, da todo de manera mucho mas ordenada, no haciendo énfasis en lo básico.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| P04  | Sin elección explícita                                  | Ambas herramientas cubrieron el recorrido solicitado. Copilot hizo más visible el paso de requisitos a diseño; Gemini destacó la revisión final.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| P05  | Claude como base                                        | Ambas herramientas siguen la estructura solicitada y proponen implementar la creación de pedidos mediante PHP nativo, JSON y transacciones. Gemini concentra la implementación en un único bloque y dedica bastante explicación al control del stock. Claude distribuye la solución en archivos y aporta más materiales para reproducirla: esquema SQL, datos de ejemplo, arranque local y una tabla de pruebas más amplia. Por esos motivos, elegiríamos la propuesta de Claude como base para realizar las comprobaciones, aunque su mayor desarrollo no garantiza que todo funcione correctamente.                                                                                                                                                                                                                                                                                                                      |
| P06  | Claude como base, pendiente de pruebas                  | Gran parte del próximo análisis está hecho con IA ya que se le volvió a pedir que compare la totalidad del código para notar cambios y/o mejoras de la interfaz visual, como también en la parte del código con sus restricciones y demás detalles que llevarían mucho tiempo poder verlas o analizarlas uno mismo.<br><br>Ambas herramientas eliminan JavaScript y proponen mejoras en el formulario, el foco y la estructura de la página. Gemini adapta además el contenido a compras individuales y por volumen, mientras que Claude conserva más elementos del enfoque B2B y señala las dudas comerciales. Claude destaca por entregar los archivos separados y explicar con claridad sus supuestos y comprobaciones pendientes. Aprovecharíamos esa organización para continuar trabajando, aunque la elección definitiva requiere probar ambas interfaces, especialmente el formulario y la navegación por teclado. |
| P07  | Claude                                                  | Ambas herramientas identifican los principales problemas y proporcionan código corregido y pasos de comprobación, dejándonos conforme con las respuestas. Gemini presenta una solución más directa, mientras que Claude desarrolla más el proceso de corrección, como que hace mucho más énfasis en los problemas y en como corregirlos. Elegimos la respuesta de Claude porque detalla bien que pasa antes y que pasa después, cosa de que, si uno no se entera del error que tiene, pueda verlo entenderlo y no repetirlo, ya que debería de entenderlo. De todos modos, no probamos el código, asique no sabemos que tan bien están las correcciones.                                                                                                                                                                                                                                                                   |
| P08  | Claude                                                  | Las dos herramientas cubren lo pedido y bastante completos, de todos modos la respuesta de Gemini, al darnos todo el README en el mismo chat, genera confusión al encontrar errores o prestar atención a la descripción, por lo tanto, la versión de Claude nos parece un poco mejor, ya que te da la respuesta concreta de los problemas que encontró en los materiales, mas que es lo que hay que saber del README y lo mas importante para nosotros, es que te genera un archivo aparte, para poder analizarlo por separado a la contestación de este.                                                                                                                                                                                                                                                                                                                                                                  |

## 9. Iteraciones

La memoria contiene las siguientes instrucciones para P02, P05 y P08, reproducidas literalmente. No se incorporan resultados de mejora que no estén documentados.

Prompt 2. Primera iteración, “Conservá el código y el HTML de la consulta anterior. Revisá la corrección y justificá los cambios en submit, respuesta HTTP, errores de red y salida de datos. Indicá cómo probar un envío válido y un fallo, sin afirmar resultados que no ejecutaste”.
Segunda iteración: “Te adjunto nuestros resultados de esas pruebas. Corregí únicamente los problemas que demuestren y devolvé la versión final con las diferencias y la misma prueba para repetir”.

Prompt 5. Primera iteración: “La consigna pide reservas y la respuesta anterior implementa pedidos. Reorientá el ejemplo a una API de reservas demostrativa, con un único endpoint en PHP nativo, JSON y datos ficticios. Separá rutas diseñadas de implementadas e incluí pruebas de éxito y error”.
Segunda iteración: “Con los resultados reales que adjuntamos, corregí el endpoint y las instrucciones de ejecución. Repetí los mismos casos y distinguí resultados esperados de observados”.

Prompt 8. Primera iteración: “Revisá el README anterior: corregí formato y rutas, diferenciá no aportado de no realizado y quitá requisitos atribuidos a la consigna sin respaldo. Justificá Markdown y Git y hacé que la guía pueda consultarse desde el README”. Segunda iteración: “Te adjunto la revisión del inventario y el resultado de seguir las instrucciones. Actualizá solo lo que esas evidencias justifiquen, indicando cambios y pendientes”.

## 10. Banco reutilizable

### Plantilla de creación reutilizable

Actúa como (rol) para (breve contexto), desarrollá (tarea) a partir de (contenido extra o algún requisito). Usá (tecnologías y herramientas) y respetá (restricciones). Entregá (formato). El resultado debe cumplir (criterios de aceptación). Explicá cómo comprobarlo y diferenciá las pruebas ejecutadas de los resultados esperados.

Ejemplo de uso: crear una pantalla de reservas de GEDES en HTML5/CSS3, con campos y listado ficticio definidos, sin JavaScript. Comprobar estructura, etiquetas, contraste y adaptación móvil antes de aceptarla.

### Plantilla de revisión y corrección

Actúa como (rol) revisá (código y entorno) cuyo comportamiento esperado es (resultado). Priorizá los problemas y explicá sus consecuencias. Reproducí (fallo) y proponé una corrección limitada a (alcance). Entregá diagnóstico, código, cambios y prueba antes y después. Si no podés ejecutar, indicá pasos y resultados esperados.

Ejemplo de uso: revisar el mismo submit y fetch de P02, conservar los identificadores, comprobar respuesta HTTP y errores de red y evitar insertar el nombre mediante innerHTML. Repetir el envío y registrar Network y el mensaje.

### Plantilla de documentación

Actúa como (rol). Documentá (proyecto) para (destinatarios) usando (materiales). Prepará (README) con requisitos, ejecución, pruebas, limitaciones y fuentes. Respetá los archivos existentes y señalá datos pendientes. Incluí cómo registrar cambios reales con (control de versiones). No inventes resultados ni fuentes consultadas.

Ejemplo de uso: documentar los ejemplos independientes de GEDES, identificar archivos que solo aparecen dentro de respuestas y explicar cómo registrar el README y sus correcciones en Git. Validar cada ruta y comando con el entorno real.

## 11. Limitaciones y puntos pendientes

El alcance es demostrativo y los ejemplos se ejecutan por separado. Las revisiones de IA no equivalen a comprobaciones ejecutadas por el equipo. Las instrucciones concretas que carecen de archivos o configuración aportados están marcadas en la sección 6.

## 12. Control de versiones con Git

Los siguientes son comandos generales para ejecutar por el equipo; no representan un historial existente. Ejecutarlos desde la carpeta real del proyecto. Si ya existe un repositorio, continuar en él.

### Inicializar y registrar la primera versión

```bash
git init
git status
git add README.md
git diff --cached
git commit
```

`git commit` permite escribir un mensaje que describa el cambio realmente preparado. Incorporar los demás archivos mediante sus rutas reales después de comprobar su contenido. Cada integrante debe usar su identidad de Git configurada.

[PENDIENTE: archivos y rutas finales que se incluirán en el primer registro; deben aportarlos Pablo Greus y Julián Leita].

### Guardar una revisión posterior

Después de efectuar un cambio real en el README:

```bash
git diff
git add README.md
git diff --cached
git commit
```

### Consultar el historial

```bash
git log
git log --oneline
git log --stat
```

### Exportar el historial

El siguiente es un comando de exportación genérico, no una referencia a un archivo ya aportado. Su salida es un archivo nuevo que debe incluirse en las evidencias:

```bash
git log --stat --date=iso > historial_git.txt
```

La redirección de salida se muestra para Bash/Git Bash. El enunciado permite historial exportado o repositorio accesible al docente.

[PENDIENTE: ejecutar y aportar la exportación real o el enlace autorizado al repositorio; deben aportarlo Pablo Greus y Julián Leita].

## 13. Declaración de uso de IA

La memoria registra Gemini y Copilot en P01–P04 y Gemini y Claude en P05–P08. Las propuestas de código, explicaciones y respuestas se distinguen del análisis y las decisiones del equipo.

Texto literal de la memoria:

Utilizamos los ocho prompts que sacamos del proyecto como ejemplos. Cada vez que les enviamos los prompts fuertes a las IAs, empezamos un chat nuevo, si hacia falta reutilizar material para poder contextualizar, lo hacíamos, se lo adjuntábamos. Utilizamos Gemini, Copilot y Claude según los casos descritos. También recurrimos a ChatGPT para ayudar a diseñar prompts, comparar respuestas, redactar descripciones y completar esta propuesta de memoria. Las aportaciones nuevas aparecen en azul y las observaciones de revisión, en rojo. La revisión, la ejecución de pruebas y las decisiones finales corresponden al equipo. No presentamos los resultados esperados por las herramientas como pruebas realizadas por nosotros.
