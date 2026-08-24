# 🚀 Landing — Curso de Claude · Relevo

![Relevo](https://img.shields.io/badge/Relevo-Academia%20de%20IA-1FE6AB?labelColor=050505)
![Estado](https://img.shields.io/badge/Estado-en%20preparaci%C3%B3n-E8A33D?labelColor=050505)
![HTML](https://img.shields.io/badge/HTML5-est%C3%A1tico-E34F26?logo=html5&logoColor=white)
![Sin dependencias](https://img.shields.io/badge/Dependencias-ninguna-6E7376?labelColor=050505)
![Peso](https://img.shields.io/badge/P%C3%A1gina-71%20KB-1FE6AB?labelColor=050505)
![Vercel](https://img.shields.io/badge/Deploy-Vercel-000000?logo=vercel&logoColor=white)
![Hecho en Colombia](https://img.shields.io/badge/Hecho%20en-Colombia%20🇨🇴-FCD116)

> Página de venta del **01 CONOCE**, el primer curso de la ruta de Relevo. Una sola página, sin build, sin dependencias y **sin una sola cifra que no se pueda sostener**.

**[🌐 relevo.academy](https://relevo.academy)** · **[📸 @relevo.academy](https://instagram.com/relevo.academy)** · **[✉️ relevoacademy@gmail.com](mailto:relevoacademy@gmail.com)**

---

## 📑 Tabla de contenidos

- [✨ Qué es](#-qué-es)
- [🧱 Cómo está armada](#-cómo-está-armada)
- [🎯 El argumento de venta](#-el-argumento-de-venta)
- [🛡️ Reglas de contenido](#️-reglas-de-contenido)
- [🎨 Identidad](#-identidad)
- [🚀 Correr localmente](#-correr-localmente)
- [📁 Estructura](#-estructura)
- [🖼️ Sobre las fotos](#️-sobre-las-fotos)
- [⚠️ Estado](#️-estado)
- [🔗 Piezas relacionadas](#-piezas-relacionadas)

---

## ✨ Qué es

Una landing de venta larga, de las que se leen de arriba abajo. El visitante llega sin saber qué es Claude y tiene que salir sabiendo tres cosas: **qué se lleva**, **por qué le sirve** y **qué pasa si no le gusta**.

Todo el contenido vive en un solo `index.html`. No hay framework, no hay paso de compilación y no hay nada que instalar para trabajar en ella.

---

## 🧱 Cómo está armada

```mermaid
flowchart TD
  P["🏠 Portada<br/><sub>promesa + prueba social</sub>"] --> H["🧰 Herramientas<br/><sub>qué te llevas puesto</sub>"]
  H --> C["🎁 Lo que vas a construir<br/><sub>4 entregables concretos</sub>"]
  C --> Z["🌱 Empezamos desde cero<br/><sub>derriba: no sé nada</sub>"]
  Z --> T["📚 Temario<br/><sub>5 módulos con duración</sub>"]
  T --> PR["💳 Precio<br/><sub>oferta + medios + garantía</sub>"]
  PR --> CE["🎓 Certificado<br/><sub>por qué vale algo</sub>"]
  CE --> TE["💬 Testimonios"]
  TE --> M["📡 Modalidad"]
  M --> F["❓ Preguntas<br/><sub>11 objeciones</sub>"]
  F --> FIN["✅ Cierre<br/><sub>último CTA + garantía</sub>"]

  P -.->|CTA| PR
  T -.->|CTA| PR
  FIN -.->|CTA| PR
```

**Decisiones clave:**

- **El CTA aparece 5 veces**: barra fija, portada, después del temario, en el precio y en el cierre. El del temario es deliberado — es el punto donde la persona ya sabe qué incluye y todavía no ha visto el precio.
- **La garantía se presenta dos veces**, junto al precio y en el cierre. Una garantía que solo aparece una vez se pierde en el scroll.
- **Las objeciones van en orden de aparición mental**, no en orden temático: primero "no sé nada", después "cuánto dura", después "ya uso ChatGPT", y al final "desde qué país".
- **La grilla usa `grid-auto-rows: 1fr`.** En CSS Grid cada fila se mide por su cuenta, así que un bloque de 4 tarjetas que cae 3+1 deja la última más baja. Esto lo iguala.

---

## 🎯 El argumento de venta

| Bloque | Qué resuelve |
|--------|--------------|
| 🏠 **Portada** | Promesa concreta: *sales con algo tuyo funcionando* |
| 🧰 **Herramientas** | Combate el "y esto para qué me sirve después" |
| 🎁 **Lo que vas a construir** | 4 entregables, no apuntes |
| 🌱 **Desde cero** | Sin conocimientos, sin cuenta paga, sin perfil técnico |
| 📚 **Temario** | Transparencia total: cada módulo con su duración |
| 💳 **Precio** | Pago único, medios locales, garantía de 7 días |
| 🎓 **Certificado** | *Se aprueba, no se regala* — hay examen |
| ❓ **Preguntas** | 11 objeciones, desplegables |

---

## 🛡️ Reglas de contenido

**No se publica una cifra que no se pueda verificar.**

Esta página **no dice cuántos alumnos hay**, porque es la primera edición y no habría cómo sostenerlo si alguien pregunta. En su lugar usa una escasez que sí es real: *primera edición en vivo, cupos limitados*.

Tampoco usa contador regresivo, ni descuento inventado, ni campaña de temporada. Un contador que se reinicia solo es mentira, y una vez que el visitante lo nota **todo lo demás de la página queda bajo sospecha**.

Los números de la página tienen que coincidir con el [taller que se entrega](https://github.com/relevoacademy/modulo-conoce):

| Dato | Valor |
|------|-------|
| Duración | 4 horas en vivo |
| Módulos | 5 (01 a 05) |
| Herramientas | 7 |
| Certificado | Con examen aprobado |

> Si cambia el taller, **la landing cambia en el mismo commit**. El certificado también dice "4 horas" — son tres piezas que se mueven juntas.

---

## 🎨 Identidad

Sigue el `RELEVO_MANUAL DE IDENTIDAD`, igual que las otras piezas de la marca.

| Token | Valor |
|-------|-------|
| Negro | `#050505` |
| Carbón | `#131415` |
| Turquesa | `#1FE6AB` |
| Gris | `#A7ABAF` |
| Títulos y cuerpo | Instrument Sans |

**El ámbar `#E8A33D` es solo para advertencias.** En esta página se usa únicamente en los avisos de contenido pendiente — y esos avisos son visibles a propósito, para que nadie publique sin resolverlos.

> ⚠️ El manual trae **dos erratas**. El hex del gris figura como `#67A6A3` pero sus propios valores RGB (167, 171, 175) dan `#A7ABAF`. Y la tipografía aparece como *"Instrumental Sans"* cuando la real es **Instrument Sans**.

---

## 🚀 Correr localmente

```bash
python -m http.server 8841
```

**Desplegar:** subir la carpeta tal cual. En Vercel, framework **Other**, sin build command, output directory la raíz. Todas las rutas son relativas — no hay nada que apunte fuera de esta carpeta.

> ⚠️ Conectar desde la cuenta de Vercel **de Relevo**. Verificar la cuenta activa antes de importar, no después.

---

## 📁 Estructura

| Ruta | Contenido |
|------|-----------|
| `index.html` | La landing completa |
| `assets/relevo-lockup.png` | Logo de la marca |
| `assets/alumnos/` | 7 retratos en WebP, 28 KB en total |

---

## 🖼️ Sobre las fotos

Los siete retratos de la portada son **generados con IA**, no fotografías de personas reales. Se eligieron sobre fondo oscuro para que se asienten en el negro de la marca sin recorte visible.

Del original de 1254×1254 px se recorta el rostro y se exporta a WebP de 160 px: **28 KB las siete, contra 14,5 MB de los originales**. En pantallas de menos de 420 px se muestran solo cinco, para que la fila no apriete el texto.

**Los testimonios no llevan rostro.** Una cita solo lleva cara cuando es de una persona real que dio su permiso. Un retrato generado junto a un testimonio le presta una credibilidad que la cita todavía no se ganó.

---

## ⚠️ Estado

**Esta página todavía no está lista para vender.** Hay contenido de maquetación
pendiente de reemplazo y el checkout no está conectado a una pasarela.

Los puntos abiertos están marcados **dentro de la propia página** con un aviso
ámbar visible, y el detalle se lleva aparte del repositorio.

> Mientras haya un aviso ámbar en pantalla, la URL no se comparte para vender.

---

## 🔗 Piezas relacionadas

| Repositorio | Qué es |
|-------------|--------|
| [`modulo-conoce`](https://github.com/relevoacademy/modulo-conoce) | El taller que esta página vende |
| [`perfil-forense`](https://github.com/relevoacademy/perfil-forense) | Taller de diagnóstico DISC, cortesía del Cripto Latin Fest |

---

Hecho con 💜 en Colombia 🇨🇴 · **Relevo — IA que trabaja contigo**
