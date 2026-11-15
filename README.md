# FORM-AC-01 — Análisis de Caso: Fallo Real en un Sistema Distribuido (Facebook, Octubre 2021)

Repositorio del **Equipo EJPZ** correspondiente a la actividad formativa **FORM-AC-01** de la asignatura **Aplicaciones Distribuidas** (Carrera de Ingeniería en Software, Paralelo A — Universidad Técnica Estatal de Quevedo).

El informe analiza la interrupción global de servicios de Facebook/Meta ocurrida el 4 de octubre de 2021, sus causas raíz modeladas mediante un árbol de fallos, su relación con los fundamentos de la Unidad 1 (transparencias de distribución, teorema CAP y tolerancia a fallos) y las medidas preventivas proyectadas para nuestro Proyecto Fin de Curso (**JobFinder — Bolsa de Empleos para Graduados UTEQ**).

## Integrantes del Equipo (EJPZ)

* **España Vera Kenny Isaías**
* **Jaramillo Acosta Luis Jeremy**
* **Paca Pilataza Luis Alberto**
* **Zambrano Ronquillo Heiner Ariel**

## Estructura del Repositorio

* `main.tex`: Código fuente del informe técnico en LaTeX bajo formato IEEE (máximo 2 páginas de desarrollo).
* `referencias.bib`: Base bibliográfica verificada con fuentes oficiales y académicas gestionada mediante `biber`.
* `Arbol_Fallos_Facebook2021.drawio`: Archivo fuente editable del diagrama de árbol de fallos elaborado en draw.io.
* `arbol_fallos_facebook2021.png`: Exportación gráfica del árbol de fallos integrada en el documento LaTeX.
* `FORM_AC_01___Análisis_de_Caso___Fallo_en_Sistemas_Distribuidos.pdf`: Versión final compilada del informe técnico.
* `README.md`: Documentación general, listado de integrantes e instrucciones de compilación.
* `evaluaciones_pares/` *(se incorporará tras la sesión presencial)*: Rúbricas de evaluación entre pares recibidas durante la exposición en clase.

## Instrucciones de Compilación

### Compilación en Overleaf
1. Subir `main.tex`, `referencias.bib` y `arbol_fallos_facebook2021.png` al mismo directorio raíz del proyecto.
2. En **Menu > Compiler**, seleccionar `pdfLaTeX`.
3. Ejecutar **Recompile** para procesar automáticamente la bibliografía con `biber`.

### Compilación Local (TeX Live / MiKTeX)
Desde la terminal ubicada en la raíz del repositorio, ejecutar la secuencia completa para resolver citas y referencias cruzadas:

```bash
pdflatex main.tex
biber main
pdflatex main.tex
pdflatex main.tex
