# 🛡️ Plantilla para reportes de pentesting en LaTeX
Recientemente he estado estudiando LaTex de manera autodidacta y me propuse crear una plantilla para poder realizar mis reportes de las maquinas de Hack The Box de manera un poco más profesional y algo más cercano a lo que seria en una auditoria real. De tal manera que, les comparto la plantilla que hice por si les es de utilidad y quién sabe, quizá les motive de alguna manera a aprender LaTex.

## 🚀 Características Principales

* **Diseño Profesional:** Portada corporativa y maquetación limpia.
* **Matriz CVSS v3.1:** Tabla de riesgos automatizada con alineación visual perfecta.
* **Hallazgos Modulares:** Bloques de `tcolorbox` para presentar vulnerabilidades con severidad crítica, alta, media, baja e info.
* **Fácil Personalización:** Variables globales para cambiar el nombre de la empresa, auditor, cliente y fechas en un solo lugar.
* **Secciones:**
  
 <p align="center">
  <img src="https://github.com/user-attachments/assets/68946cb9-a849-476a-81c8-08791f668ada" alt="Portada del Reporte" width="70%">
</p>
  <p align="center">
  <img src="https://github.com/user-attachments/assets/1ab757d5-937a-472e-a754-f6560c3d1f93" alt="Índice del Reporte" width="70%">
</p>    
 <p align="center">
  <img src="https://github.com/user-attachments/assets/efdc217b-8aa1-4fd2-8c21-ced95268074b" alt="Seccion de Hallazgos del Reporte" width="70%">
</p> 


## 📋 Requisitos

Para compilar esta plantilla necesitas una distribución de LaTeX instalada:

* **Windows:** [MiKTeX](https://miktex.org/) o TeX Live.
* **Linux:** `texlive-full` (Recomendado).
* **Editor Sugerido:** Visual Studio Code con la extensión "LaTeX Workshop" u [Overleaf](https://www.overleaf.com/).

## 🛠️ Instrucciones de Uso

1.  **Clonar el repositorio:**
    ```bash
    git clone https://github.com/joscalejo/htb-latex-report.git
    ```
2.  **Configurar Variables:**
    Abre el archivo `plantilla.tex` y edita el bloque de variables al inicio:
    ```latex
    \newcommand{\empresa}{MiEmpresa Sec}
    \newcommand{\miUser}{MiNombre}
    \newcommand{\maquinaNombre}{NombreMaquina}
    \newcommand{\maquinaIP}{10.10.10.X}
    ```
3.  **Añadir Imágenes:**
    Coloca tus capturas y logos en la carpeta `images/` y actualiza las rutas en el código.
4.  **Compilar:**
    Ejecuta `pdflatex plantilla.tex` o usa tu editor preferido para generar el PDF.

## 📂 Estructura de los archivos

```text
.
├── images/             # Carpeta para logos y capturas de evidencia
├── plantilla.tex       # Código fuente principal
├── ejemplo.pdf         # Ejemplo de cómo se ve el reporte final
├── LICENSE             # Licencia
└── README.md           # Este archivo
