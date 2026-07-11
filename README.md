<div align="center">

# ⚡ Simulador · Circuito π Nominal

### Análisis de líneas de transmisión mediante el modelo de cuadripolo ABCD

[![Demo en vivo](https://img.shields.io/badge/🌐_Demo_en_vivo-Abrir_simulador-2ea44f?style=for-the-badge)](https://jesusp2702.github.io/simulador_circuito_pi_nominal/)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)](https://jesusp2702.github.io/simulador_circuito_pi_nominal/)
[![Sin dependencias](https://img.shields.io/badge/dependencias-ninguna-blue?style=flat-square)]()
[![Uso offline](https://img.shields.io/badge/uso-offline_✓-informational?style=flat-square)]()
[![Licencia](https://img.shields.io/badge/licencia-MIT-lightgrey?style=flat-square)](#-licencia)

**[🚀 Probar el simulador](https://jesusp2702.github.io/simulador_circuito_pi_nominal/)**

</div>

---

## 📖 ¿Qué es esto?

Un simulador web, ligero y sin instalación, para el **análisis de líneas de transmisión de longitud media** usando el modelo de **circuito π nominal** y su representación como **cuadripolo (parámetros ABCD)**.

Permite calcular tensiones, corrientes, potencias y reactivos en ambos extremos de la línea, tanto en **valores por unidad (p.u.)** como en **valores reales**, a partir de los datos del sistema, la carga y los parámetros de la línea.

Pensado como herramienta de apoyo para estudiantes y docentes de **Sistemas de Potencia / Líneas de Transmisión**.

---

## ✨ Características

- 🧮 **Cálculo completo del modelo π nominal**: constantes ABCD, tensiones, corrientes, potencias y reactivos del condensador shunt.
- 🔁 **Resultados en p.u. y en valores reales**, sobre la misma plantilla, para comparar de un vistazo.
- 🎛️ **Entrada flexible de parámetros**: valores totales de línea, por kilómetro o por milla.
- ⚡ **Definición del elemento shunt** como susceptancia (B) o como reactancia capacitiva (X꜀).
- 🔌 **Tipo de carga** inductiva (atraso) o capacitiva (adelanto).
- 📊 **Índices de desempeño**: regulación de voltaje y eficiencia de transmisión.
- 🗺️ **Esquemático interactivo** del circuito con tensiones, corrientes, pérdidas y reactivos señalados.
- 🌗 **Modo oscuro** integrado.
- 📱 **Versión de escritorio y versión móvil**, cada una optimizada para su formato.
- 📴 **100% offline**: es un solo archivo HTML, sin backend ni conexión a internet requerida.
- ✅ **Motor de cálculo validado numéricamente** contra una implementación de referencia en Python (Grainger & Stevenson, cap. 6).

---

## 🚀 Cómo usarlo

### Opción 1 — En línea (recomendado)

Entra directamente al simulador, sin instalar nada:

👉 **https://jesusp2702.github.io/simulador_circuito_pi_nominal/**

### Opción 2 — Sin conexión a internet

1. Descarga el archivo HTML correspondiente a tu dispositivo desde este repositorio:
   - 🖥️ `Simulador Circuito PI_Escritorio.html`
   - 📱 `Simulador Circuito PI_Movil.html`
2. Pulsa **Download / Descargar archivo bruto** en GitHub.
3. Abre el archivo descargado con cualquier navegador (Chrome, Edge, Firefox...).
4. Listo — el simulador funciona completamente **sin conexión a internet**.

---

## 🧭 Guía rápida de uso

1. **Define las bases del sistema** (tensión base V_B y potencia base S_B) para el análisis en por unidad.
2. **Ingresa los datos del extremo receptor**: tensión, potencia aparente de la carga, factor de potencia y tipo de carga.
3. **Configura los parámetros de la línea**: longitud, resistencia, reactancia y el elemento shunt (B o X꜀), en valores totales o por unidad de longitud.
4. Revisa los **resultados** organizados en tensiones, corrientes, potencias, reactivos del condensador y constantes ABCD.
5. Usa el botón **"Restablecer caso de ejemplo"** para volver a un caso predefinido y comparar tus propios cálculos.

> 💡 Tip: activa el **modo oscuro** si prefieres trabajar de noche o simplemente te gusta más el estilo.

---

## 🔬 Fundamento teórico

El circuito π nominal modela una línea de transmisión de longitud media mediante una impedancia serie **Z = R + jX** y dos admitancias shunt de **Y/2** en cada extremo. Su comportamiento como cuadripolo se describe con las constantes generalizadas:

```
A = (ZY)/2 + 1        →  relación de tensiones
B = Z                 →  impedancia de transferencia
C = Y·[(ZY)/4 + 1]    →  admitancia de transferencia
D = A                 →  línea simétrica
```

A partir de estas constantes, el simulador obtiene tensión, corriente y potencia en el extremo emisor a partir de las condiciones del extremo receptor (o viceversa), además de la regulación de voltaje y la eficiencia de transmisión.

---

## 🗂️ Estructura del repositorio

```
simulador_circuito_pi_nominal/
├── Simulador Circuito PI_Escritorio.html   # Versión optimizada para PC
├── Simulador Circuito PI_Movil.html        # Versión optimizada para móvil
└── README.md
```

---

## 🛠️ Tecnología

Construido íntegramente con **HTML, CSS y JavaScript puro**, sin frameworks ni dependencias externas — por eso puede ejecutarse abriendo el archivo directamente en el navegador, incluso sin conexión.

---

## 👤 Autor

Desarrollado por **Jesús Peña** — UNEFA Lara.
Con apoyo de **Claude (Anthropic)** para el diseño de la interfaz.

¿Encontraste un error o tienes una idea de mejora? ¡Los recomendaciones y sugerencias son bienvenidos!

---

## 📄 Licencia

Este proyecto se distribuye con fines educativos. Si deseas usarlo, adaptarlo o compartirlo, se agradece dar crédito al autor original.

<div align="center">

⭐ Si te resultó útil, considera darle una estrella al repositorio ⭐

</div>
