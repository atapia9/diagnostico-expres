# Estado actual · Diagnóstico expréss

Actualizado: 19 de octubre de 2026

## Publicación
- **Sitio:** https://atapia9.github.io/diagnostico-expres/
- **Repositorio (público):** https://github.com/atapia9/diagnostico-expres
- **Despliegue:** GitHub Actions, rama `main` → GitHub Pages. Último despliegue exitoso.
- **Formulario (`FORM_URL`):** `https://docs.google.com/forms/d/e/1FAIpQLSdJrWC0J5qKVaIEh0maUr8EmfonQ-8QM-LBSFH3HFvdYf_reA/viewform`

## Qué hay
| Archivo | Estado |
|---|---|
| `index.html` | Completo. Botón de registro al formulario (pestaña nueva); aviso visible; leyenda de demostración |
| `aviso-privacidad.html` | Borrador con datos del formulario, finalidades y correo ARCO; pendiente de revisión legal |
| `css/styles.css` | Mobile first; colores de marca son placeholders |
| `js/config.js`, `js/main.js` | `FORM_URL` y `PRIVACY_URL`; no guarda nada en el navegador |
| `README.md` | Cambio de URL, QR, checklist previo al evento |
| `.github/workflows/pages.yml`, `.gitignore` | Operativos |

Responsable: Jesús Armando Tapia Gallegos y Acambaro.com.mx. Contacto de privacidad y ARCO: privacidad@acambaro.com.mx.

## Pruebas
- **Hecho (navegador integrado):** vertical 375 px y horizontal 1024×768 sin desbordamiento; botón abre `FORM_URL` en pestaña nueva; el aviso se abre desde la página; sin `localStorage` ni cookies; páginas publicadas responden 200.
- **No verificado:** Android e iOS reales, vertical y horizontal. Tampoco se probó el formulario de punta a punta ni en incógnito.

## Revisión del aviso
- **Página de revisión (privada, compartir con Indyra desde el menú Compartir):** https://claude.ai/artifact/9TR8f1CoA46UA5V5wrkCPY
- Cada `[ DATO ]` es una ficha asignada a Indyra o a Armando; las respuestas se guardan en un almacén compartido y cada edición queda firmada.
- La página trae su propia copia de `aviso-privacidad.html`: si el aviso cambia en el repositorio, hay que volver a publicarla.
- Al terminar, Claude lee las respuestas, actualiza el aviso y el Word, y hace el último commit en la rama `aviso-privacidad-v2`.

## Propuesta simplificada del aviso
`aviso-privacidad-simplificado.html` y `.docx`: 619 palabras y 10 datos pendientes, frente a 1,048 palabras y 17 de la versión completa. Indyra elige cuál se publica.

Informe para Indyra y Armando con la comparación, condiciones, pendientes y el texto simplificado: `informe-simplificacion-aviso-privacidad.docx`.

Solo vale si se hacen estos cambios (Armando):
- Quitar del formulario los campos “Ciudad o estado” y “Comentario breve”.
- Quitar la copia oculta a Proton y registrar el envío en la hoja.
- Usar Gemini en nivel de pago.

Y si Indyra confirma que bastan:
- Describir a los encargados por tipo, sin la ubicación de cada uno.
- Un solo plazo de conservación para todos los datos.

La página de revisión trabaja sobre la versión completa; si se elige la simplificada, hay que volver a publicarla.

## Pendientes
**Legales (para revisión de Indyra)**
1. Domicilio completo del responsable (sección 1).
2. Finalidad por ciudad o estado: ¿requiere casilla de consentimiento propia? (sección 3).
3. Transferencias o encargados por el uso de Google Forms (sección 4).
4. Plazo de conservación (sección 5).
5. Fecha de la versión final (sección 7).

**Del sitio**
- Decidir si el botón sigue abriendo en pestaña nueva (hoy sí).
- Dominio propio, solo si aplica.
- `index.html` no tiene `noindex` (el aviso sí); decidir si se desea.

**Formulario de Google:** actualizado (título, correo de privacidad y ajustes). Falta únicamente reflejar en él lo que resuelva la revisión legal.

**Antes del evento (18 al 20 de noviembre de 2026)**
- Generar e imprimir el QR y escanearlo en Android e iOS.
- Tablet con batería y conexión; aviso de privacidad visible en el stand.

---
Este material fue elaborado con asistencia de Claude (Anthropic) y revisado por [nombre].
