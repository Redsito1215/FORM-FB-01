# FORM-FB-01 - Fichas bibliograficas

Actividad individual formativa de la asignatura Aplicaciones Distribuidas. El documento incluye portada, introduccion, criterios de seleccion, cinco fichas bibliograficas, referencias y declaracion de uso de inteligencia artificial.

## Archivos del repositorio

- `main.tex`: documento principal en LaTeX.
- `fuentes.bib`: base bibliografica usada por `biblatex`.
- `FORM_FB_01.pdf`: documento compilado.
- `README.md`: instrucciones de compilacion.

## Requisitos

- Una distribucion LaTeX actual (TeX Live 2024 o posterior, MiKTeX actualizado o equivalente).
- Compilador `pdflatex`.
- `bibtex` para procesar la bibliografia.
- Paquetes: `babel`, `geometry`, `microtype`, `xcolor`, `enumitem`, `hyperref` y `biblatex` con el estilo `ieee`.

## Compilacion

El archivo principal es `main.tex`. Desde la carpeta del repositorio, ejecutar en este orden:

```bash
pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex
```

El resultado sera `main.pdf`; debe renombrarse como `FORM_FB_01.pdf` para mantener el nombre utilizado en este repositorio.

Como alternativa, si `latexmk` esta instalado:

```bash
latexmk -pdf main.tex
```

## Verificacion bibliografica

Los cinco DOI incluidos en `fuentes.bib` fueron comprobados contra las paginas de IEEE, Springer Nature o Elsevier. Antes de entregar, el estudiante debe abrir nuevamente los enlaces y comprobar que los resumenes y notas expresen su propia lectura y voz.

## Entrega

En GitHub deben permanecer publicos los cuatro archivos enumerados arriba. En el LMS/SGA se entrega un PDF diferente, de una sola pagina, con los datos identificativos y la URL completa de este repositorio.
