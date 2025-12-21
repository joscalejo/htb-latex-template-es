# 🛡️ Professional Pentesting Report Template (LaTeX)

Plantilla en LaTeX diseñada para generar reportes de auditoría de seguridad y write-ups de máquinas CTF (Hack The Box, TryHackMe) con un acabado profesional.

Este proyecto nace como una iniciativa personal para estandarizar la documentación técnica de mis ejercicios en Hack The Box, consolidando al mismo tiempo mis habilidades en LaTeX y la redacción de informes técnicos.

## 🚀 Características Principales

* **Diseño Profesional:** Portada corporativa "Full Bleed" y maquetación limpia.
* **Matriz CVSS v3.1:** Tabla de riesgos automatizada con alineación visual perfecta.
* **Hallazgos Modulares:** Bloques de `tcolorbox` para presentar vulnerabilidades con severidad crítica, alta, media, baja e info.
* **Fácil Personalización:** Variables globales para cambiar el nombre de la empresa, auditor, cliente y fechas en un solo lugar.
* **Secciones Estándar:**
  
 <p align="center">
  <img src="https://github.com/user-attachments/assets/56ff24dc-2baf-48d3-b25f-b0823a1eaa61" alt="Portada del Reporte" width="70%">
</p>
  <p align="center">
  <img src="https://github.com/user-attachments/assets/5b147017-8fd8-49dd-a41a-68f92d394786" alt="Índice del Reporte" width="70%">
</p>    
 <p align="center">
  <img src="https://github.com/user-attachments/assets/554feb7f-ee87-42eb-8b5f-583acc377b41" alt="Seccion de Hallazgos del Reporte" width="70%">
</p> 


## 📋 Requisitos

Para compilar esta plantilla necesitas una distribución de LaTeX instalada:

* **Windows:** [MiKTeX](https://miktex.org/) o TeX Live.
* **Linux:** `texlive-full` (Recomendado).
* **Editor Sugerido:** Visual Studio Code con la extensión "LaTeX Workshop" u [Overleaf](https://www.overleaf.com/).

## 🛠️ Instrucciones de Uso

1.  **Clonar el repositorio:**
    ```bash
    git clone [https://github.com/TU_USUARIO/htb-latex-report.git](https://github.com/TU_USUARIO/htb-latex-report.git)
    ```
2.  **Configurar Variables:**
    Abre el archivo `plantilla.tex` y edita el bloque de variables al inicio:
    ```latex
    \newcommand{\empresa}{MiEmpresa Sec}
    \newcommand{\miUser}{TuNombre}
    \newcommand{\maquinaNombre}{NombreMaquina}
    \newcommand{\maquinaIP}{10.10.10.X}
    ```
3.  **Añadir Imágenes:**
    Coloca tus capturas y logos en la carpeta `images/` y actualiza las rutas en el código.
4.  **Compilar:**
    Ejecuta `pdflatex plantilla.tex` o usa tu editor preferido para generar el PDF.

## 📂 Estructura del Proyecto

```text
.
├── images/             # Carpeta para logos y capturas de evidencia
├── plantilla.tex       # Código fuente principal
├── ejemplo.pdf         # (Opcional) Ejemplo de cómo se ve el reporte final
├── LICENSE             # Licencia
└── README.md           # Este archivo
