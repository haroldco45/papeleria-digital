# Papelería Digital · Vibras Positivas HM

Plataforma para que las empresas dejen de mandar a imprimir talonarios a la tipografía.
Cada documento sale con el logo, el NIT, el color y el consecutivo propio de la empresa. Se firma en pantalla y se envía por WhatsApp o se imprime / guarda en PDF.

## Formatos incluidos (9)
| Formato | Prefijo | Tipo |
|---|---|---|
| Remisión (con o sin valores) | REM | Renglones |
| Orden de pedido | PED | Renglones |
| Cotización (con IVA, 19 % por defecto, editable) | COT | Renglones |
| Cuenta de cobro | CC | Renglones |
| Recibo de caja | RC | Valor |
| Comprobante de egreso | CE | Valor |
| Vale de caja menor | VAL | Valor |
| Acta de entrega (con estado) | ACT | Renglones |
| Orden de servicio | OS | Renglones |

## Funciones
- **Mi empresa**: razón social, NIT, dirección, teléfono, correo, logo, color de marca, tamaño de hoja (carta o media carta), texto al pie, aviso de datos y PIN de administrador. Prefijo y consecutivo inicial por formato.
- **Nuevo documento**: hoja en vivo mientras se llena, valor en letras automático, firmas con el dedo o el mouse, fecha y hora de Colombia (America/Bogota).
- **Talonario en blanco**: imprime de 1 a 100 hojas en blanco, cada una con su consecutivo reservado (reemplaza el talonario de la tipografía).
- **Historial**: búsqueda, filtro por formato, duplicar, reimprimir, enviar por WhatsApp y anular con motivo (el consecutivo nunca se reutiliza).
- **Respaldo**: descarga y restauración en .json.
- Español / inglés.
- PWA instalable, funciona sin internet.

## Datos personales (Ley 1581 de 2012)
- Aviso de tratamiento de datos en el formulario (editable por la empresa).
- En el historial, la cédula/NIT y el teléfono salen enmascarados; se ven completos solo con el PIN de administrador. Anular también pide PIN.

## Aviso legal en cada hoja
"Documento interno de control. No reemplaza la factura electrónica de venta ni el documento soporte electrónico ante la DIAN."

## Dónde se guarda la información
En el navegador del dispositivo (localStorage, ≈ 5 MB). Recomendar a cada cliente descargar el respaldo cada semana. Siguiente fase: servidor propio en Hostinger (PHP + MySQL) con usuarios por empresa.

## Publicar
1. Subir a GitHub (repo `haroldco45/papeleria-digital`): `index.html`, `manifest.json`, `sw.js`, `icon-192.png`, `icon-512.png`, `og-image.png`, `README.md`.
2. Conectar el repo en Netlify con el nombre de sitio **papeleria-digita** → `https://papeleria-digita.netlify.app/`.
3. Si el nombre del sitio cambia, cambiar la URL en las etiquetas `og:url`, `og:image` y `twitter:image` de `index.html`.

---
Desarrollada por Vibras Positivas HM — Derechos de Autor Reservados
