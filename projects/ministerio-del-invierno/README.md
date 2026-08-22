<div align="center">

# ❄️ El Ministerio del Invierno

### Sobrevive al sistema, administra tus ingresos y protege a tu familia

![game play de ministerio](./screenshots/gameplay.jpg)

**Simulación de trabajo y gestión financiera en una ciudad distópica**

![Estado](https://img.shields.io/badge/Estado-Prototipo_funcional-22C55E?style=for-the-bero](https://img.shields.io/badge/Glación-38BDF8?style=for-the-badge
![Tecnología](https://img.shields.io/badge/Tecnología-HTML5_JavaScript-F59E0B?badge

</div>

---

## 📖 Descripción

**El Ministerio del Invierno** es un videojuego educativo de simulación y gestión de recursos ambientado en una ciudad distópica afectada por una crisis energética.

El jugador trabaja como analista de créditos y debe procesar solicitudes económicas bajo presión. Al finalizar cada jornada laboral, debe administrar el dinero ganado para cubrir los gastos esenciales de su familia.

Cada decisión tiene consecuencias. Un error durante el trabajo reduce los ingresos, mientras que una mala decisión financiera durante la noche puede afectar la salud familiar o provocar un embargo.

---

## 💡 Concepto y premisa

El jugador representa a un analista que trabaja para una institución burocrática en una ciudad fría y hostil.

Durante el día debe revisar documentos y decidir si corresponde aprobar o denegar cada solicitud de crédito.

Durante la noche debe distribuir el dinero acumulado entre tres necesidades esenciales:

- Alquiler.
- Calefacción.
- Comida.

El propósito es sobrevivir durante cinco días, mantener a la familia con salud y evitar acumular tres avisos de embargo.

---

## 🎯 Objetivo del jugador

El objetivo es sobrevivir los cinco días de trabajo administrando correctamente los ingresos obtenidos.

Para ganar, el jugador debe:

1. Evaluar correctamente las solicitudes de crédito.
2. Obtener dinero mediante decisiones correctas.
3. Evitar multas durante la jornada laboral.
4. Distribuir responsablemente el presupuesto nocturno.
5. Mantener la salud familiar por encima de cero.
6. Evitar acumular tres avisos de embargo.
7. Completar el quinto día.

---

## 🧩 Género

- Simulación de trabajo.
- Gestión de recursos.
- Puzle burocrático.
- Estrategia financiera.
- Videojuego educativo.

---

## 👥 Público objetivo

El videojuego está dirigido principalmente a jóvenes de entre 18 y 25 años.

Busca enseñar conceptos relacionados con:

- Administración del dinero.
- Priorización de necesidades.
- Presupuesto limitado.
- Consecuencias de las decisiones financieras.
- Costo de oportunidad.
- Manejo responsable de gastos esenciales.

---

## 🔄 Estructura de la partida

La partida está dividida en dos fases principales:

```text
FASE DE DÍA
Procesamiento de solicitudes de crédito
              ↓
FASE DE NOCHE
Administración del presupuesto familiar
              ↓
SIGUIENTE DÍA
```

Este ciclo se repite durante cinco días, salvo que el jugador alcance antes una condición de derrota.

---

## 🏢 Fase de día: trabajo de oficina

Durante el día, el jugador debe procesar cinco documentos.

Cada documento muestra:

- Nombre del ciudadano.
- Ingreso mensual.
- Monto solicitado.
- Límite permitido.
- Temporizador.
- Contador de documentos.
- Salario acumulado durante el día.

El jugador debe decidir entre:

- `APROBAR`
- `DENEGAR`

---

## 📋 Regla de evaluación

Una solicitud debe aprobarse únicamente cuando el monto solicitado sea igual o inferior al 30 % del ingreso mensual del ciudadano.

La regla puede expresarse de la siguiente manera:

```text
Monto solicitado ≤ Ingreso mensual × 0.30
```

### Ejemplo de aprobación

```text
Ingreso mensual: $1000
Límite permitido: $300
Monto solicitado: $250

Decisión correcta: APROBAR
```

### Ejemplo de denegación

```text
Ingreso mensual: $1000
Límite permitido: $300
Monto solicitado: $450

Decisión correcta: DENEGAR
```

---

## ⏱️ Temporizador

El jugador dispone normalmente de 10 segundos para evaluar cada documento.

Si no responde antes de que termine el tiempo:

- La decisión se considera incorrecta.
- Se aplica una multa de $15.
- El juego continúa con el siguiente documento.

La barra del temporizador cambia de verde a rojo cuando queda poco tiempo.

Si el jugador no paga la comida durante la noche, el tiempo disponible al día siguiente se reduce de 10 a 7,5 segundos.

---

## 💵 Economía laboral

Las decisiones tomadas durante el día afectan directamente el salario:

```text
Decisión correcta: +$20
Decisión incorrecta: -$15
Tiempo agotado: -$15
```

Cada día contiene cinco documentos.

El dinero obtenido se agrega al fondo acumulado al terminar la jornada. Si el resultado acumulado fuera negativo, el fondo se mantiene en cero.

---

## 🌙 Fase de noche: gestión del presupuesto

Al completar los cinco documentos, comienza la fase nocturna.

En esta etapa se muestran:

- Fondo acumulado.
- Salud familiar.
- Avisos de embargo.
- Gastos disponibles.
- Total seleccionado para pagar.
- Dinero restante.

El jugador selecciona mediante casillas qué gastos desea pagar.

No puede confirmar una selección si su costo es mayor que el dinero disponible.

---

## 🏠 Gastos nocturnos

### Alquiler: $40

El alquiler protege al jugador de los avisos de embargo.

Si no se paga:

```text
+1 aviso de embargo
```

Al acumular tres avisos, la partida termina en derrota.

### Calefacción: $25

La calefacción protege la salud familiar frente al frío.

Si no se paga:

```text
-35 % de salud familiar
```

Si la salud llega a cero, la partida termina.

### Comida: $20

La comida permite mantener el ritmo normal de trabajo.

Si no se paga:

```text
El temporizador del siguiente día disminuye de 10 a 7,5 segundos.
```

Esto dificulta la evaluación de las solicitudes.

---

## ⚖️ Toma de decisiones financieras

En algunas noches, el jugador puede no tener suficiente dinero para pagar todos los gastos.

Debe analizar:

- Cuánto dinero tiene disponible.
- Qué consecuencias produce cada gasto no pagado.
- Cuántos avisos de embargo posee.
- Cuánta salud conserva la familia.
- Si puede trabajar con menos tiempo al día siguiente.

La mecánica muestra que una decisión financiera no solamente afecta el saldo inmediato, sino también las posibilidades futuras del jugador.

---

## 🕹️ Controles

El juego se controla completamente con el mouse o una pantalla táctil.

### Durante el día

- `CLIC EN APROBAR`: aceptar una solicitud válida.
- `CLIC EN DENEGAR`: rechazar una solicitud que supera el límite.

### Durante la noche

- `CLIC EN CASILLAS`: seleccionar los gastos que se desean pagar.
- `CLIC EN PAGAR Y DORMIR`: confirmar el presupuesto y avanzar.
- `CLIC EN INTENTAR DE NUEVO`: reiniciar después de una victoria o derrota.

---

## 📈 Progresión

La versión actual tiene una duración de cinco días.

Cada día contiene:

```text
5 solicitudes de crédito
```

En total, una partida completa puede presentar:

```text
25 solicitudes
```

La dificultad puede aumentar si no se paga la comida, porque el tiempo de evaluación del día siguiente se reduce.

Además, las consecuencias económicas se acumulan:

- Los avisos de embargo permanecen.
- La salud perdida no se recupera automáticamente.
- El dinero restante se conserva.
- Las decisiones anteriores condicionan las siguientes noches.

---

## ✅ Condición de victoria

El jugador gana cuando completa los cinco días sin alcanzar una condición de derrota.

Para sobrevivir debe mantener:

```text
Avisos de embargo < 3
Salud familiar > 0 %
```

Al ganar, el juego muestra el saldo final disponible.

---

## ❌ Condiciones de derrota

Existen dos condiciones principales de derrota.

### Embargo

La partida termina cuando el jugador acumula:

```text
3 avisos de embargo
```

Esto ocurre al no pagar el alquiler durante tres noches.

### Pérdida de salud

La partida termina cuando la salud familiar llega a:

```text
0 %
```

Esto sucede al omitir repetidamente el pago de la calefacción.

---

## 🎓 Componente educativo

El Ministerio del Invierno enseña el uso responsable del dinero mediante decisiones con consecuencias a corto y mediano plazo.

El jugador practica:

- Cálculo de porcentajes.
- Evaluación de límites financieros.
- Administración de ingresos.
- Priorización de necesidades.
- Elaboración de un presupuesto.
- Gestión de recursos escasos.
- Análisis del costo de oportunidad.
- Prevención de deudas y penalizaciones.
- Planificación para días futuros.

El juego muestra que disponer de dinero no significa poder pagar todo. El jugador debe identificar qué necesidades son más urgentes y anticipar las consecuencias de sus decisiones.

---

## 🌐 Ambientación

La historia está situada en una ciudad distópica afectada por el frío y una crisis energética.

El jugador trabaja dentro de un sistema burocrático que exige rapidez y precisión mientras enfrenta dificultades económicas personales.

La ambientación refuerza la presión de las decisiones financieras:

- El trabajo determina los ingresos.
- Los errores producen multas.
- El frío amenaza la salud.
- El alquiler protege la vivienda.
- La alimentación afecta el rendimiento laboral.
- Cada jornada aumenta la tensión acumulada.

---

## 🎨 Estilo visual

El proyecto utiliza una interfaz inspirada en sistemas burocráticos y terminales administrativas.

La identidad visual se compone de:

- Fondo azul oscuro.
- Paneles grises.
- Bordes discretos.
- Texto blanco.
- Detalles en azul gélido.
- Verde para decisiones positivas.
- Rojo para penalizaciones y derrotas.
- Amarillo para advertencias.
- Tipografía monoespaciada.
- Tarjetas de documentos.
- Contadores y barras de estado.

Este diseño transmite una sensación fría, seria y administrativa.

---

## 🖼️ Capturas de pantalla

### Pantalla inicial

La pantalla inicial presenta la ambientación, la regla del 30 %, el sistema de recompensas y multas y el botón para comenzar.

![inicio de ministerio](./screenshots/inicio.jpg)

### Gameplay

Durante la fase de trabajo se muestra la solicitud de un ciudadano, sus datos financieros, el límite permitido, el temporizador y los botones para aprobar o denegar.

![game play de ministerio](./screenshots/gameplay.jpg)

### Pantalla final

La pantalla final presenta la victoria o derrota, una explicación de la causa y la opción para intentar nuevamente.

![fin de ministerio](./screenshots/fin.jpg)

---

## 🛠️ Tecnologías utilizadas

- HTML5.
- CSS3.
- JavaScript.
- Manipulación del DOM.
- Generación aleatoria de documentos.
- Temporizadores con JavaScript.
- Diseño web adaptable.
- GitHub para organización, documentación y publicación.

Todo el videojuego está contenido en un único archivo llamado `index.html`.

No necesita instalación ni dependencias externas y puede ejecutarse directamente en un navegador.

---

## ▶️ Cómo ejecutar el juego

### Ejecución local

1. Descarga el archivo `index.html`.
2. Ábrelo con Chrome, Edge o Firefox.
3. Presiona **INICIAR TURNO**.
4. Revisa el ingreso mensual y el monto solicitado.
5. Compara el monto con el límite del 30 %.
6. Selecciona **APROBAR** o **DENEGAR**.
7. Procesa los cinco documentos.
8. Administra los gastos durante la noche.
9. Sobrevive durante cinco días.

### Versión en línea

La versión jugable se habilitará cuando el portafolio sea publicado mediante GitHub Pages.

<div align="center">

![Jugar próximamente](https://img.shields.io/badge/Jugartyle=for-the-badge

</div>

---

## 📑 Desarrollo basado en un GDD

El proyecto fue planificado mediante un **Game Design Document**, también conocido como GDD.

El documento permitió definir antes de la programación:

- El concepto y la premisa.
- El género.
- El objetivo del jugador.
- La mecánica principal.
- Las reglas.
- La progresión.
- Los personajes.
- El estilo visual.
- El público objetivo.
- Las condiciones de victoria y derrota.
- El propósito educativo.

El GDD funcionó como una guía común para que los integrantes del equipo comprendieran qué debía construirse y cómo debía funcionar el prototipo.

---

## 🧪 Validación del prototipo

El prototipo fue comparado con el GDD para comprobar que:

- Funciona sin errores técnicos importantes.
- La mecánica coincide con el diseño planificado.
- Las fases de día y noche están implementadas.
- Es posible alcanzar la victoria.
- Es posible alcanzar las condiciones de derrota.
- El juego enseña principios de administración del dinero.
- Las reglas económicas tienen consecuencias visibles.

---

## 🤖 Uso de inteligencia artificial

La inteligencia artificial generativa fue utilizada como herramienta de apoyo para producir el prototipo a partir de un prompt basado directamente en el GDD.

El prompt definió:

- El título y la ambientación.
- La estética distópica.
- La regla de aprobación del 30 %.
- La cantidad de documentos y días.
- El temporizador.
- Las recompensas y multas.
- Los gastos nocturnos.
- Las consecuencias de no pagar.
- Las condiciones de victoria y derrota.
- Los requisitos técnicos.

El resultado generado fue revisado, probado y comparado con las especificaciones del GDD.

### Aporte del equipo

El equipo participó en:

- La investigación sobre el GDD.
- La definición del concepto.
- El diseño de las mecánicas.
- La creación de las reglas económicas.
- La selección de la ambientación.
- La elaboración del prompt.
- Las pruebas del prototipo.
- La validación de las condiciones de victoria y derrota.
- La revisión de la coherencia entre el GDD y el videojuego.
- La identificación de mejoras futuras.

---

## 📚 Aprendizajes

Durante este proyecto aprendimos a:

- Comprender la función de un Game Design Document.
- Planificar un videojuego antes de programarlo.
- Mantener coherencia entre el diseño y el prototipo.
- Convertir conceptos financieros en mecánicas jugables.
- Diseñar una experiencia con dos fases complementarias.
- Aplicar porcentajes en una mecánica de decisiones.
- Crear consecuencias acumulativas.
- Administrar estados y recursos mediante JavaScript.
- Implementar temporizadores.
- Validar un prototipo utilizando criterios definidos previamente.
- Trabajar colaborativamente en el diseño de un videojuego.

---

## 🔧 Mejoras futuras

En una siguiente versión nos gustaría:

- Ampliar la partida hasta 30 días.
- Incorporar una deuda inicial que deba pagarse.
- Añadir tasas de interés.
- Incluir documentos falsificados.
- Agregar reglas nuevas en cada jornada.
- Ocultar el límite calculado para aumentar el desafío.
- Incorporar eventos económicos inesperados.
- Permitir recuperar parte de la salud familiar.
- Añadir música ambiental y efectos de sonido.
- Incluir animaciones de sellos.
- Incorporar retratos de los ciudadanos.
- Añadir diálogos y decisiones morales.
- Mostrar un resumen financiero al terminar cada noche.
- Guardar el progreso.
- Mejorar la presentación visual.
- Incorporar diferentes finales.
- Realizar pruebas con jóvenes de 18 a 25 años.

---

## 📂 Estructura del proyecto

```text
ministerio-del-invierno/
├── README.md
├── index.html
└── screenshots/
    ├── inicio.jpg
    ├── gameplay.jpg
    └── fin.jpg
```

- `README.md`: documentación del videojuego.
- `index.html`: archivo completo y ejecutable.
- `screenshots/inicio.jpg`: pantalla inicial.
- `screenshots/gameplay.jpg`: fase de análisis de documentos.
- `screenshots/fin.jpg`: pantalla de victoria o derrota.

---

## 👥 Equipo de desarrollo

- **Americo Oswaldo Ramirez Rocha**
- **Amara Isabel Quintela Ramirez**
- **Cristhian Giovanni Pacsi**

Proyecto desarrollado para la asignatura **Game Development**.

---

<div align="center">

[![Volver a proyectos](https://img.-Proyectos-7B2CBF?style=for-the-badge](../)

[![Volver al portafolio](https://img.shields.io/badge/Volver-Portafolio-e](../../)

</div>
