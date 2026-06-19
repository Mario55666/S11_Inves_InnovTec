# Gabinete del Detective — Misión Semiótica

> *Expediente principal · Curso de Semiótica de la Imagen 2026 · IUTP Lima*

Experiencia educativa gamificada de análisis semiótico y antropológico de la imagen publicitaria. El estudiante asume el rol de investigador/detective que debe descifrar los códigos, mitos e ideologías ocultos en una campaña cultural de ONG sobre identidad cultural y diversidad. La actividad integra **refuerzo activo del aprendizaje**: cada error desencadena un minijuego de refuerzo antes de continuar.

---

## Descripción general

Un portal de investigación de estilo victoriano-noir que introduce al estudiante en cinco fases de análisis semiológico. La narrativa de "telegrama urgente de la Agencia" contextualiza la misión: detectar los signos, mitos y decisiones de diseño que contradicen el mensaje declarado de una campaña.

La aplicación es un **archivo HTML autocontenido** (single-file app): todo el juego principal (Misión Semiótica) está embebido como base64 dentro del propio `index.html`, lo que permite distribuirlo sin servidor.

---

## Características principales

- **5 fases de investigación** con mecánica de cartas: *escena → indicio → testimonio → evidencia → sospechoso → coartada*
- **Análisis semiológico-antropológico** con marco victoriano y figuras retóricas visuales
- **Refuerzo activo automático**: cada error lanza *Campo de Indicios* (deducción) o *Asteroides del Signo* (identificación de conceptos)
- **Mesa de análisis con IA**: sube la imagen de campaña y genera el prompt de análisis exportable
- **Informe imprimible** y exportable a CSV para entrega al docente
- **PWA-ready**: incluye soporte para `manifest.json` e icono de 192px
- **Diseño responsivo** adaptado a dispositivos móviles (breakpoint 520px)

---

## Tecnologías utilizadas

| Tecnología | Uso |
|---|---|
| HTML5 / CSS3 / JavaScript (vanilla) | Estructura, estilos y lógica completa |
| Bootstrap Icons 1.11.3 | Iconografía de interfaz |
| Google Fonts (Cinzel Decorative, Cinzel, EB Garamond, IM Fell English) | Tipografía victoriana |
| Base64 encoding | Juego principal embebido en el HTML |
| CSS custom properties | Sistema de diseño (paleta burdeos, oro, pergamino) |

---

## Estructura del archivo

```
index.html
├── Portal de investigación (hub de inicio)
│   ├── Telegrama de la Agencia (narrativa introductoria)
│   ├── Tira de pistas iniciales (3 tarjetas orientadoras)
│   └── Portal principal → botón de acceso al expediente
└── Vista del juego (iframe a pantalla completa)
    ├── Barra de navegación con botón "Salir del expediente"
    └── iframe → Misión Semiótica (cargada desde base64)
```

---

## Cómo usar

1. Abrir `index.html` directamente en el navegador (no requiere servidor).
2. Leer el telegrama introductorio y las pistas.
3. Hacer clic en **"Entrar al expediente"** para iniciar la Misión Semiótica.
4. Completar las 5 fases de análisis. Ante cada error, jugar el minijuego de refuerzo hasta superar el umbral de conocimiento.
5. Al cerrar el caso, descargar el informe PDF/CSV para entrega al docente.

> **Nota pedagógica:** Los juegos *Campo de Indicios* y *Asteroides del Signo* no son decorativos; aparecen como consecuencia de deducciones imprecisas y son el mecanismo por el cual el conocimiento se consolida.

---

## Paleta de diseño

| Variable | Valor | Uso |
|---|---|---|
| `--burdeos` | `#5c1a1a` | Color base institucional |
| `--oro` | `#c8a24a` | Acentos y bordes |
| `--oro-claro` | `#e6c878` | Títulos y CTA |
| `--pergamino` | `#efe3c8` | Texto principal |
| `--tinta` | `#1a1410` | Fondo oscuro base |

---

## Autor

**Mg. Mario Quiroz Martínez**  
Curso de Semiótica de la Imagen · 2026  
Instituto de Educación Superior "Diseño y Comunicación" · Lima, Perú

---

## Licencia

Material educativo de uso interno. Todos los derechos reservados © 2026 Mario Quiroz Martínez.
