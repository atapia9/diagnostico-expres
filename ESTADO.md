# Estado actual · Diagnóstico exprés

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
| `aviso-privacidad.html` | Versión simplificada; pendiente de revisión legal de 8 temas |
| `css/styles.css` | Mobile first; colores de marca son placeholders |
| `js/config.js`, `js/main.js` | `FORM_URL` y `PRIVACY_URL`; no guarda nada en el navegador |
| `README.md` | Cambio de URL, QR, checklist previo al evento |
| `.github/workflows/pages.yml`, `.gitignore` | Operativos |

Responsable: Jesús Armando Tapia Gallegos y Acambaro.com.mx. Contacto de privacidad y ARCO: privacidad@acambaro.com.mx.

## Pruebas
- **Hecho (navegador integrado):** vertical 375 px y horizontal 1024×768 sin desbordamiento; botón abre `FORM_URL` en pestaña nueva; el aviso se abre desde la página; sin `localStorage` ni cookies; páginas publicadas responden 200.
- **No verificado:** Android e iOS reales, vertical y horizontal. Tampoco se probó el formulario de punta a punta ni en incógnito.

## Aviso de privacidad: versión simplificada (decidido el 5 de noviembre de 2026)
- `aviso-privacidad.html` y `aviso-privacidad-actualizado.docx` son ahora la versión simplificada. La versión completa anterior queda como referencia en `aviso-privacidad-completo.html` y `.docx` (no se publica).
- Ya resueltos: responsable (Jesús Armando Tapia Gallegos), domicilio fiscal y fecha de la última actualización.
- Comparación de las dos versiones: `informe-simplificacion-aviso-privacidad.docx`.

**Antes de publicarla (Armando), para que el aviso coincida con lo que se recaba:**
- Quitar del formulario los campos “Ciudad o estado” y “Comentario breve”.
- Quitar la copia oculta a Proton y registrar el envío en la hoja.
- Usar Gemini en nivel de pago.

**Temas para revisar con Indyra (8):**
1. `[ DATO: confirmar si requiere consentimiento específico o base distinta (Indyra) ]` (sección 3)
2. `[ DATO: plazo de respuesta ARCO según la ley vigente ]` (sección 5)
3. `[ DATO: nombre y datos de contacto de la autoridad vigente ]` (sección 5)
4. `[ DATO: confirmar si BAJA basta como mecanismo de revocación (Indyra) ]` (sección 6)
5. `[ DATO: plazo único de conservación (Indyra) ]` (sección 6)
6. `[ DATO: confirmar si además se avisará por correo a quienes aceptaron contacto (Indyra) ]` (sección 8)
7. `[ DATO: decisión de Indyra sobre la aclaración ]` (correo del diagnóstico)
8. `[ DATO: confirmar obligaciones aplicables ]` (correo comercial y BAJA)

La sección 7 (encargados) la resuelve Armando.

**Página de revisión:** https://claude.ai/artifact/9TR8f1CoA46UA5V5wrkCPY. Trae su propia copia de `aviso-privacidad.html`: si el aviso cambia en el repositorio, hay que volver a publicarla.

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
Este material fue elaborado con asistencia de Claude (Anthropic) y revisado por Jesús Armando Tapia Gallegos.
