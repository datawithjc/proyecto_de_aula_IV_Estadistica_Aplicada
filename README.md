# Estadística Aplicada · Guía del Proyecto de Aula

Guía web interactiva de **Estadística Aplicada** para el Proyecto de Aula de Cuarto Semestre del programa
de **Tecnología en Control de Calidad** de la Fundación Universitaria Tecnológico Comfenalco.

El sitio desarrolla las temáticas estadísticas que el estudiante necesita para aplicar el instrumento de
diagnóstico integral de procesos, analizar los datos de la empresa y sustentar la propuesta de mejora con
evidencia cuantitativa.

## Contenido

| Sección | Descripción |
|---|---|
| **14 bloques temáticos** | Organizados en 4 fases, según el momento del proyecto en que cada herramienta se necesita |
| **4 ejemplos guiados** | Casos resueltos de principio a fin con datos como los del instrumento diagnóstico |
| **20 ejercicios resueltos** | Procedimiento paso a paso con interpretación técnica |
| **30 ejercicios propuestos** | Con pista y respuesta final oculta tras un botón |
| **Formulario** | Referencia rápida con las 26 fórmulas del curso |

### Las cuatro fases

1. **Fundamentos y recolección** — escalas de medición, recolección de datos, tablas de frecuencia
2. **Descripción y visualización** — gráficos, índices de cumplimiento, tendencia central, dispersión, comparación entre periodos
3. **Relación y priorización** — correlación de Pearson y Spearman, Pareto, matriz de Vester, muestreo
4. **Control y justificación** — distribuciones aplicadas, control estadístico de procesos, capacidad, inferencia

## Publicar en GitHub Pages

1. Cree un repositorio nuevo en GitHub (por ejemplo `estadistica-aplicada`).
2. Suba los tres archivos de esta carpeta: `index.html`, `README.md` y `.nojekyll`.
3. Vaya a **Settings → Pages**.
4. En *Source* elija **Deploy from a branch**, rama `main` y carpeta `/ (root)`.
5. Guarde. En uno o dos minutos el sitio queda publicado en
   `https://<usuario>.github.io/<repositorio>/`

El archivo `.nojekyll` evita que GitHub Pages procese el sitio con Jekyll; sin él, cualquier carpeta que
empiece por guion bajo sería ignorada.

### Subir desde la línea de comandos

```bash
git init
git add index.html README.md .nojekyll
git commit -m "Guía de Estadística Aplicada · Proyecto de Aula"
git branch -M main
git remote add origin https://github.com/<usuario>/<repositorio>.git
git push -u origin main
```

## Detalles técnicos

- **Un solo archivo.** `index.html` es autocontenido: estilos y scripts van embebidos. No hay dependencias
  de compilación ni instalación.
- **Notación matemática.** Se renderiza con [MathJax 3](https://www.mathjax.org/) desde CDN, con respaldo
  automático a un segundo CDN si el primero falla. Requiere conexión a internet la primera vez que se
  abre la página.
- **Sin almacenamiento local.** La página no guarda datos del usuario ni usa cookies.
- **Responsivo.** Funciona en escritorio, tableta y celular. Las fórmulas anchas se desplazan
  horizontalmente en pantallas pequeñas.
- **Imprimible.** Al imprimir o exportar a PDF desde el navegador, los paneles de ejercicios y todas las
  respuestas se muestran automáticamente.
- **Accesibilidad.** Navegación por teclado, contraste conforme a WCAG AA y etiquetas ARIA en los gráficos SVG.

## Verificación de los resultados

Los 50 ejercicios fueron calculados y verificados computacionalmente con NumPy y SciPy antes de
publicarse: cada media, desviación, coeficiente de correlación, probabilidad, límite de control e índice
de capacidad proviene de un cálculo ejecutado, no de una estimación.

## Créditos

Material docente elaborado por **Juan Carlos Acosta Jiménez, PhD.**
Facultad de Ingeniería · Fundación Universitaria Tecnológico Comfenalco · Cartagena de Indias

Construido a partir del Instructivo del Proyecto de Aula de Cuarto Semestre, el Instrumento de
Diagnóstico Integral de Procesos y la Estructura del Informe Diagnóstico Empresarial del programa.

## Licencia

Contenido educativo de uso libre para fines académicos, con atribución al autor.
