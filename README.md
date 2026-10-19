# Diseño arquitectónico: Repensando los parquímetros

Tarea 3 de **Análisis y Diseño de Sistemas 2** (Sección A, Escuela de Ingeniería en Ciencias y
Sistemas, USAC). Caso 4: *Repensando los parquímetros, un acercamiento al diseño de interfaces
desde la perspectiva del usuario* (Morales Zaragoza, UAM Cuajimalpa, 2015).

**SIEP** (Sistema Integrado de Estacionamiento en la vía Pública) es nuestra propuesta: el pago
queda ligado a la placa, el parquímetro que ya existe cobra con tarjeta y avisa si lo dañan, la
multa solo nace cuando un oficial confirma la evidencia, y todo lo que se cobra se publica. La
solución se plantea desde las cuatro perspectivas que pide la consigna (arquitectura del
software, calidad del software, arquitectura en el ciclo de vida y arquitectura de la
información) y se trae al contexto de Guatemala, incluidos los cobros de cuidacarros.

## Qué hay en el repositorio

| Carpeta | Contenido |
|---|---|
| `documento/` | El documento completo en PDF (con carátula, índice y referencias) y su `.docx` editable |
| `presentacion/` | La presentación animada (`.pptx`) y su versión en PDF, el guion general y un guion por integrante en `guiones/` |
| `sitio/` | El sitio del proyecto (`index.html`) y el prototipo interactivo del parquímetro (`prototipo.html`) |
| `diagramas/` | Las láminas en SVG y en Excalidraw editable: caso de negocio, casos de uso, bloques, despliegue y capturas del prototipo |

## Cómo verlo

- **Documento:** abrir `documento/Grupo2_CasoParquimetros.pdf`.
- **Presentación:** abrir `presentacion/Grupo2_CasoParquimetros_Presentacion.pptx` en PowerPoint
  2019 o posterior, o en Keynote. Las transiciones usan Morph (en Keynote se reproducen como
  Movimiento mágico) y cada tarjeta entra con un clic.
- **Sitio:** servir la raíz del repositorio y abrir `sitio/`:

  ```bash
  python3 -m http.server 8000
  # http://localhost:8000/sitio/
  ```

  El prototipo funciona solo, sin servidor: `sitio/prototipo.html`.

## Equipo (Grupo 2)

| Integrante | Rol |
|---|---|
| Santiago Julián Barrera Reyes | Scrum Master / coordinador |
| Jemima Solmaira Chavajay Quiejú | Product Owner |
| Byron Josué Par Rancho | Equipo de desarrollo |

## Flujo de trabajo: GitFlow

- `main`: solo versiones entregadas, cada una con su etiqueta (`v1.0.0`).
- `develop`: integración.
- `feature/*`: una rama por entregable (`feature/documento-caratula`, `feature/presentacion`,
  `feature/sitio-web`), integradas en `develop` con `--no-ff`.
- `release/*`: preparación de la versión; se fusiona en `main` y de vuelta en `develop`.

## Créditos

Íconos [Lucide](https://lucide.dev) (licencia ISC). Las cifras de Guatemala salen de notas de
La Hora, Soy502, Emisoras Unidas y Prensa Libre, citadas en el documento (sección 10).
Trabajo académico.
