# Estado actual · Diagnóstico exprés

Actualizado: 25 de noviembre de 2026

## Publicación
- **Uso:** opción permanente de entrada para Acambaro.com.mx (desde el 25 de noviembre de 2026 ya no está ligado a ningún evento).
- **Sitio:** https://atapia9.github.io/diagnostico-expres/
- **Repositorio (público):** https://github.com/atapia9/diagnostico-expres
- **Despliegue:** GitHub Actions, rama `main` → GitHub Pages. Último despliegue exitoso.
- **Formulario (`FORM_URL`):** `https://docs.google.com/forms/d/e/1FAIpQLSdJrWC0J5qKVaIEh0maUr8EmfonQ-8QM-LBSFH3HFvdYf_reA/viewform`

## Qué hay
| Archivo | Estado |
|---|---|
| `index.html` | Completo. Botón de registro al formulario (pestaña nueva); aviso visible; leyenda de que el sitio no recaba datos |
| `aviso-privacidad.html` | Versión simplificada; pendiente de revisión legal de 8 temas |
| `css/styles.css` | Mobile first; colores de marca son placeholders |
| `js/config.js`, `js/main.js` | `FORM_URL` y `PRIVACY_URL`; no guarda nada en el navegador |
| `README.md` | Cambio de URL, QR, checklist de operación |
| `.github/workflows/pages.yml`, `.gitignore` | Operativos |

Responsable: Jesús Armando Tapia Gallegos y Acambaro.com.mx. Contacto de privacidad y ARCO: privacidad@acambaro.com.mx.

## Pruebas
- **Hecho (navegador integrado):** vertical 375 px y horizontal 1024×768 sin desbordamiento; botón abre `FORM_URL` en pestaña nueva; el aviso se abre desde la página; sin `localStorage` ni cookies; páginas publicadas responden 200.
- **No verificado:** Android e iOS reales, vertical y horizontal. Tampoco se probó el formulario de punta a punta ni en incógnito.

## Aviso de privacidad: versión simplificada (decidido el 5 de noviembre de 2026)
- `aviso-privacidad.html` y `aviso-privacidad-actualizado.docx` son ahora la versión simplificada. La versión completa anterior queda como referencia en `aviso-privacidad-completo.html` y `.docx` (no se publica).
- Ya resueltos: responsable (Jesús Armando Tapia Gallegos), domicilio fiscal y fecha de la última actualización.
- Comparación de las dos versiones: `informe-simplificacion-aviso-privacidad.docx`.

**Para que el formulario y el script coincidan con el aviso (Armando):** desde el 25 de noviembre de 2026 el aviso ya no lista “Ciudad o estado” ni “Comentario breve”, y Proton solo recibe las solicitudes de privacidad.
- Quitar del formulario los campos “Ciudad o estado” y “Comentario breve”.
- Quitar la copia oculta a Proton y registrar el envío en la hoja.
- Usar Gemini en nivel de pago.

**Temas de Indyra resueltos en el aviso (7 de noviembre de 2026, commit `c93b175`):**
1. ~~Consentimiento de la casilla de contacto comercial~~ (sección 3): finalidad secundaria y opcional; la casilla viene desmarcada y la negativa no condiciona el diagnóstico.
2. ~~Plazo de respuesta ARCO~~ (sección 5): 20 días hábiles desde el día hábil siguiente a la solicitud y 15 días hábiles más para hacerlo efectivo.
3. ~~Autoridad vigente~~ (sección 5): Secretaría Anticorrupción y Buen Gobierno (SABG), www.gob.mx/buengobierno.
4. ~~BAJA como mecanismo de revocación~~ (sección 6): sí, como mecanismo ágil y gratuito, además del correo de privacidad.
5. ~~Plazo único de conservación~~ (sección 6): 6 meses desde el registro; después solo se guardan el correo y la fecha en una lista de exclusión interna.
6. ~~Aviso por correo de cambios~~ (sección 8): sí, además de publicarlos con su fecha, se avisa por correo a los contactos activos.

La sección 7 (encargados) la resolvió Armando: Google (Formularios y Hojas), Google AI Studio, Resend y Proton (solo para las solicitudes de privacidad), con servidores que pueden estar fuera de México.

**Temas de Indyra pendientes (fuera del aviso):**
7. `[ DATO: decisión de Indyra sobre la aclaración ]` (correo del diagnóstico)
8. `[ DATO: confirmar obligaciones aplicables ]` (correo comercial y BAJA)

**Página de revisión:** https://claude.ai/artifact/9TR8f1CoA46UA5V5wrkCPY. Trae su propia copia del aviso: es el borrador del 5 de noviembre con sus 7 marcadores `[ DATO ]`, sin la referencia al evento y con fecha del 25 de noviembre de 2026 (versión 4). No incluye las resoluciones de arriba; se dejó así a propósito el 25 de noviembre para que sus fichas sigan funcionando.

## Pendientes
**Legales (para revisión de Indyra)**
- Los temas 7 y 8 de arriba (correo del diagnóstico y correo comercial).
- Ya resueltos de la lista anterior: domicilio del responsable, encargados por el uso de Google Forms, plazo de conservación y fecha del aviso. La finalidad por ciudad o estado ya no aplica: la versión simplificada no le da una finalidad propia.

**Del sitio**
- Decidir si el botón sigue abriendo en pestaña nueva (hoy sí).
- Dominio propio, solo si aplica.
- `index.html` no tiene `noindex` (el aviso sí); decidir si se desea.

**Formulario de Google:** actualizado (título, correo de privacidad y ajustes). Falta únicamente reflejar en él lo que resuelva la revisión legal.

**Como entrada permanente**
- Enlazar el Diagnóstico exprés desde Acambaro.com.mx.
- Generar el QR y escanearlo en Android e iOS.

---
Este material fue elaborado con asistencia de Claude (Anthropic) y revisado por Jesús Armando Tapia Gallegos.
