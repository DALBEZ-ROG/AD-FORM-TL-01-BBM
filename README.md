# FORM-TL-01: Modelado de comunicación entre procesos distribuidos

Universidad Técnica Estatal de Quevedo, Carrera de Software.
Aplicaciones Distribuidas (ISR-701), séptimo nivel, paralelo B.
Docente: Gleiston Guerrero Ulloa, PhD.

## Integrantes

- Benites Pérez Dariem Alberto
- Bueno Troya Erwin Daniel
- Mendoza Villarroel Elian Jossue

## Escenario

Sistema de reservas de vuelos con cuatro procesos:

- cliente;
- servidor de aplicación;
- servicio de pagos;
- base de datos.

El cliente se comunica con el servidor por sockets TCP, y el servidor llama al servicio de pagos con gRPC. Este diseño es la base de la práctica PE-U1.

## Contenido del repositorio

| Carpeta | Archivos |
|---|---|
| `caratula/` | `caratula.tex` y `caratula.pdf` |
| `diagrama/` | `diagrama-comunicacion.drawio` (editable, se abre en draw.io o en app.diagrams.net) y `diagrama-comunicacion.pdf` |
| `notas/` | `notas.tex`, `interacciones.tex` (tabla y justificación de cada interacción) y `notas.pdf` |

## Cómo compilar

Se necesita MiKTeX o TeX Live con `pdflatex`. No hay bibliografía, así que no hace falta `biber`.

**Notas**

`notas.tex` incluye el PDF del diagrama y el archivo `interacciones.tex`, así que se compila con el repositorio completo y desde la carpeta `notas`. Se corre dos veces para que la figura quede bien numerada:

```
cd notas
pdflatex notas.tex
pdflatex notas.tex
```

**Carátula**

```
cd caratula
pdflatex caratula.tex
```

## Uso de IA

Para que se uso: Para encontrar el diseño de la comunicación: qué mecanismo, protocolo y middleware usa cada interacción y por qué. Hizo un diagrama de referencia que redibujamos en draw.io, ayudo a corregir la tabla de interacciones, las justificaciones y las preguntas preparadas de estas notas.
