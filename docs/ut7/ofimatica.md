# 7.3. Documentación técnica y herramientas ofimáticas

## 1. Principios de la documentación técnica

La documentación técnica recoge la información necesaria para comprender, utilizar, instalar y mantener un programa o sistema informático.

Para que sea útil, debe cumplir cinco principios fundamentales:

1. **Actualizada:** debe modificarse cuando cambian las versiones, rutas o comandos.
2. **Bien organizada:** debe incluir índices, apartados y una estructura lógica.
3. **Lenguaje claro:** debe evitar ambigüedades y explicar correctamente los procedimientos.
4. **Fácil de entender:** debe adaptarse al tipo de lector, ya sea usuario o técnico.
5. **Consistente:** debe mantener el mismo formato, terminología y estilo.

### Tipos de documentación técnica

| Tipo | Finalidad |
|---|---|
| Manual de usuario | Explica cómo utilizar un programa paso a paso. |
| Manual de administración | Describe la instalación, configuración, mantenimiento y recuperación del sistema. |
| README / Wiki | Presenta el proyecto, su estructura y cómo ejecutarlo. |
| Changelog | Registra los cambios y mejoras de cada versión. |
| Registro de incidencias | Documenta problemas, sus causas y las soluciones aplicadas. |

## 2. Ofimática tradicional, texto plano y Markdown

Existen diferentes formas de crear y editar documentos. Las más habituales son:

| Enfoque | Características | Ventajas | Utilización |
|---|---|---|---|
| Ofimática (WYSIWYG) | Permite editar directamente el aspecto visual del documento. | Fácil de utilizar y permite una maquetación avanzada. | Informes, presupuestos y presentaciones. |
| Texto plano (.txt) | Almacena texto sin formato visual. | Ligero, sencillo y compatible. | Notas, registros y archivos de configuración. |
| Markdown (.md) | Utiliza símbolos sencillos para dar formato al texto. | Fácil de leer, editar y compartir. | Manuales, documentación técnica y README. |

WYSIWYG significa *What You See Is What You Get* (lo que ves es lo que obtienes). Es el sistema utilizado por muchos procesadores de texto tradicionales.

### Suites ofimáticas y equivalencias

Las suites ofimáticas agrupan herramientas para crear documentos, hojas de cálculo y presentaciones.

| Función | Microsoft 365 | LibreOffice | Google Workspace |
|---|---|---|---|
| Texto | Word | Writer | Documentos |
| Hoja de cálculo | Excel | Calc | Hojas de cálculo |
| Presentaciones | PowerPoint | Impress | Presentaciones |
| Bases de datos | Access | Base | Sin equivalente directo |

### Formatos de archivo

Los documentos ofimáticos utilizan diferentes extensiones:

- **ODF:** formatos abiertos como `.odt`, `.ods` y `.odp`.
- **OOXML:** formatos como `.docx`, `.xlsx` y `.pptx`.
- **PDF:** formato utilizado para compartir documentos manteniendo su presentación.

ODF y OOXML son familias de formatos estandarizados internacionalmente. PDF es especialmente útil para entregar documentos terminados sin depender del programa utilizado para crearlos.

> [!TIP]
> Para entregar un informe o trabajo académico, es recomendable exportarlo a PDF. Así se conserva mejor su presentación y se reducen los problemas de compatibilidad entre programas.

## 3. Guía práctica de Markdown

Markdown es un lenguaje de marcado ligero que permite dar formato a documentos utilizando texto plano y símbolos sencillos.

Se utiliza habitualmente en GitHub, GitLab y herramientas de documentación como Docsify.

### Sintaxis básica

| Elemento | Sintaxis | Resultado |
|---|---|---|
| Título principal | `# Título` | Encabezado H1 |
| Subtítulo | `## Sección` | Encabezado H2 |
| Negrita | `**texto**` | **texto** |
| Cursiva | `*texto*` | *texto* |
| Código en línea | `` `comando` `` | `comando` |
| Lista | `- Elemento` | Lista con viñetas |
| Enlace | `[Web](https://ejemplo.org)` | Enlace web |
| Imagen | `![Descripción](imagen.png)` | Imagen insertada |

### Listas y organización

Markdown permite organizar información mediante listas numeradas y listas con viñetas.

Ejemplo:

```markdown
# Instalación de un programa

1. Descargar el instalador.
2. Ejecutar el archivo.
3. Seguir las instrucciones.

- Requisito: conexión a Internet.
- Requisito: permisos de instalación.
```

### Tablas y bloques de código

También permite incluir tablas y fragmentos de código para documentar procedimientos técnicos.

Ejemplo de bloque de código:

```bash
# Actualizar los paquetes del sistema
sudo apt update

# Instalar el servidor Nginx
sudo apt install -y nginx
```

Ejemplo de tabla:

| Parámetro | Valor | Descripción |
|---|---|---|
| Puerto | `80` | Tráfico HTTP |
| Puerto | `443` | Tráfico HTTPS |

## 4. Herramientas para trabajar con Markdown

Existen diferentes herramientas que facilitan la creación y conversión de documentos Markdown.

### Visual Studio Code

Visual Studio Code permite editar archivos Markdown y visualizar el resultado sin necesidad de abrir un navegador externo.

Sus principales funciones son:

- Edición de archivos `.md`.
- Resaltado de sintaxis.
- Vista previa del documento.
- Organización de archivos y carpetas.

Para abrir la vista previa se pueden utilizar estos atajos:

| Acción | Atajo |
|---|---|
| Vista previa en la pestaña actual | `Ctrl + Shift + V` |
| Vista previa lateral | `Ctrl + K`, después `V` |

### Pandoc

Pandoc es una herramienta que permite convertir documentos entre distintos formatos, como Markdown, Word y HTML.

Ejemplo de conversión:

```bash
# Convertir Markdown a Word
pandoc manual.md -o manual.docx

# Convertir Markdown a HTML
pandoc manual.md -s -o manual.html
```

Estas conversiones permiten reutilizar la documentación en diferentes formatos sin tener que redactarla desde cero.

## 5. Conclusión

La documentación técnica es fundamental para explicar el funcionamiento y mantenimiento de los sistemas informáticos. Las herramientas ofimáticas facilitan la creación de documentos, mientras que Markdown ofrece una alternativa sencilla, ligera y especialmente útil para proyectos tecnológicos.

Con herramientas como Visual Studio Code, Docsify y Pandoc es posible crear, organizar, visualizar y distribuir documentación técnica de forma eficiente.
