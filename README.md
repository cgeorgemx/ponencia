# De la idea a la ponencia

Aplicación web desarrollada para apoyar la elaboración de **ponencias teóricas tipo ensayo** mediante una ruta de trabajo organizada en tres módulos: estructuración de la propuesta, orientación para la escritura académica y análisis automatizado de consistencia interna.

## Propósito

La aplicación acompaña al usuario desde la delimitación inicial de un tema hasta la revisión de una ponencia en formato PDF. Está orientada a participantes del microtaller **“De la idea a la ponencia: organizar, argumentar y comunicar”**.

## Funcionalidades

### 1. Del tema a la estructura teórica

Permite ingresar:

- Tema de investigación.
- Contexto de análisis.
- Constructo central.
- Dos dimensiones.
- Vacío, tensión o problema conceptual.
- Tipo de aporte teórico esperado.

A partir de estos datos, la aplicación genera:

- Tres posibles títulos.
- Pregunta orientadora.
- Objetivo académico.
- Tesis argumentativa.
- Posible aporte novedoso.
- Relación entre constructo, dimensiones y variables.
- Estructura sugerida para la ponencia.
- Opción para copiar o descargar la propuesta en formato TXT.

### 2. Escritura y argumentación académica

Incluye orientaciones para:

- Introducción.
- Formulación del problema teórico.
- Construcción de argumentos.
- Uso de contraargumentos.
- Integración de citas.
- Elaboración de conclusiones.
- Estilo académico.

También permite pegar un fragmento y revisar de forma automatizada:

- Número de palabras.
- Número de oraciones.
- Número de párrafos.
- Uso de conectores.
- Extensión de las oraciones.
- Extensión de los párrafos.
- Presencia de tesis explícita.
- Posibles citas.
- Expresiones poco precisas.

### 3. Análisis de consistencia interna

Permite subir una ponencia en formato **PDF** y revisar:

- Presencia de introducción, desarrollo y conclusiones.
- Existencia de pregunta orientadora.
- Existencia de objetivo académico.
- Presencia de tesis argumentativa.
- Uso de citas.
- Sección de referencias.
- Conectividad discursiva.
- Continuidad del constructo y sus dimensiones.
- Claridad de las oraciones.
- Puntaje global de consistencia.
- Recomendaciones prioritarias.
- Descarga del informe en formato TXT.

## Tecnologías utilizadas

- HTML5
- CSS3
- JavaScript
- PDF.js

La aplicación funciona completamente en el navegador y no requiere una base de datos.

## Estructura del proyecto

```text
/
├── index.html
└── README.md
```

## Ejecución local

1. Descarga o clona el repositorio.
2. Abre el archivo `index.html` en un navegador web actualizado.
3. Utiliza el menú superior para acceder a los tres módulos.

También puede ejecutarse mediante un servidor local. Por ejemplo, con Python:

```bash
python -m http.server 8000
```

Después, abre en el navegador:

```text
http://localhost:8000
```

## Publicación con GitHub Pages

1. Sube `index.html` y `README.md` a la rama `main`.
2. Abre la sección **Settings** del repositorio.
3. Entra en **Pages**.
4. En **Build and deployment**, selecciona:
   - Source: `Deploy from a branch`
   - Branch: `main`
   - Folder: `/root`
5. Guarda los cambios.
6. Espera a que GitHub genere la URL pública del sitio.

## Requisitos para analizar archivos PDF

El módulo de consistencia funciona con archivos PDF que contienen **texto seleccionable**.

No procesa correctamente:

- PDF escaneados como imagen.
- Documentos protegidos con contraseña.
- Archivos dañados.
- Documentos sin una capa de texto.

Los PDF escaneados requieren un proceso previo de reconocimiento óptico de caracteres, conocido como OCR.

## Privacidad

El archivo PDF se procesa directamente en el navegador del usuario. La versión actual no almacena ni envía el documento a un servidor externo.

## Limitaciones

El análisis es automatizado y orientativo. No sustituye:

- La revisión de un especialista.
- La evaluación de la calidad de las fuentes.
- El análisis profundo de la originalidad.
- La valoración de la solidez epistemológica.
- La revisión formal de normas editoriales.
- La evaluación por pares.

## Recomendaciones de uso

- Definir con precisión el constructo central.
- Utilizar dimensiones conceptualmente relacionadas.
- Formular una tesis discutible y sustentable.
- Integrar literatura científica pertinente.
- Mantener coherencia entre pregunta, objetivo, desarrollo y conclusiones.
- Revisar manualmente todas las sugerencias generadas.

## Laboratorio de Escritura Científica

La aplicación incluye un acceso directo al GPT:

[Laboratorio de Escritura de Textos Científicos](https://chatgpt.com/g/g-6a3db41bb3948191ba30ca4ec8df6bf5-laboratorio-de-escritura-de-textos-cientificos)

## Autor

**Carlos Enrique George-Reyes**

ORCID: [0000-0002-2529-9155](https://orcid.org/0000-0002-2529-9155)

## Licencia

Este proyecto puede utilizarse con fines académicos y formativos, siempre que se reconozca la autoría correspondiente.
