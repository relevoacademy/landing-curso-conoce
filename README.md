# Landing — Curso de Claude · Relevo

Página de venta del **01 CONOCE — Claude: chat, Proyectos y Artefactos**.
Sitio estático, sin build ni dependencias.

```
index.html          la landing completa
assets/             logo de la marca
PENDIENTES.md       lo que falta antes de publicar
```

## Desplegar

Subir la carpeta tal cual. En Vercel: framework **Other**, sin build command,
output directory la raíz. Todas las rutas son relativas — no hay nada que
apunte fuera de esta carpeta.

Para verla en local:

```bash
python -m http.server 8840
```

## Identidad

Sigue el `RELEVO_MANUAL DE IDENTIDAD`, igual que los talleres
[`perfil-forense`](https://github.com/relevoacademy/perfil-forense) y `modulo-conoce`.

| Token | Valor |
|---|---|
| Negro | `#050505` |
| Carbón | `#131415` |
| Turquesa | `#1FE6AB` |
| Gris | `#A7ABAF` |
| Títulos y cuerpo | Instrument Sans |

**El ámbar `#E8A33D` es solo para advertencias**, y en esta página se usa
únicamente en los avisos de contenido pendiente.

> El manual trae dos erratas: el hex del gris figura como `#67A6A3` pero sus
> valores RGB (167, 171, 175) dan `#A7ABAF`; y la tipografía aparece como
> "Instrumental Sans" cuando la real es **Instrument Sans**.

## Estructura de la página

| # | Sección | Qué hace en el argumento de venta |
|---|---|---|
| 1 | Portada | Promesa + prueba social + primer CTA |
| 2 | Herramientas | Qué te llevas puesto: 7 prompts reutilizables |
| 3 | Lo que vas a construir | 4 entregables concretos, no apuntes |
| 4 | Empezamos desde cero | Derriba la objeción de "no sé nada" |
| 5 | Temario | 5 módulos con duración + CTA |
| 6 | Precio | Oferta, medios de pago, garantía |
| 7 | Certificado | Por qué vale algo (hay examen) |
| 8 | Testimonios | Prueba social **— pendiente** |
| 9 | Modalidad | Cómo funciona en la práctica |
| 10 | Preguntas | 11 objeciones, en orden de aparición |
| 11 | Cierre | Último CTA + garantía repetida |

El CTA aparece **5 veces**: portada, temario, precio, cierre y la barra
superior fija.

## Reglas de contenido

**No se publican cifras que no se puedan verificar.** Esta página no dice
cuántos alumnos hay porque es la primera edición y no habría cómo sostenerlo.
En su lugar usa una escasez que sí es real: *primera edición en vivo, cupos
limitados*.

Los números de la página tienen que coincidir con el taller que se entrega
(`modulo-conoce`):

| Dato | Valor |
|---|---|
| Duración | 4 horas en vivo |
| Herramientas | 7 |
| Módulos | 5 (00 a 04) |
| Certificado | Con examen aprobado |

Si cambia el taller, **hay que cambiar la landing en el mismo commit**.

## Checkout

El botón abre una hoja con el resumen de compra y las casillas de
aceptación de términos y tratamiento de datos. **Todavía no está conectado a
una pasarela** — ver `PENDIENTES.md`.
