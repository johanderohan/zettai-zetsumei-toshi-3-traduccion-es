# Zettai Zetsumei Toshi 3 — Traducción al español

[![Invítame a un café en Ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/johanderohan)

Ficha del proyecto, capturas y más traducciones al castellano en **[Parches en Castellano](https://parchesencastellano.com/traducciones/psp/zettai-zetsumei-toshi-3)**.

Traducción al **español de España** de *Zettai Zetsumei Toshi 3: Kowareyuku Machi to Kanojo no Uta*
(絶体絶命都市3 ─壊れゆく街と彼女の歌─, PSP, Irem, 2009), la tercera entrega de la saga conocida en
Occidente como *Disaster Report*. Nunca salió de Japón.

La traducción está hecha **directamente desde el japonés** y se reparte como **parche**: no incluye
el juego. Necesitas tu propia copia para aplicarlo.

## Estado

Última versión: **[v1.1](../../releases/tag/v1.1)**.

| Parte | Estado |
|---|---|
| Guion, menús de texto, objetos, manual de desastres, diario y misiones | **6.234 mensajes traducidos** (100 %) |
| Texto dentro de imágenes | **271 rótulos**: menú del título, menú de pausa, opciones, manual, fichas de personaje, instalación y las 97 pantallas de carga |
| Mensajes del ejecutable | Resultados de usar/equipar/tirar objetos, guardado y estadísticas |
| Caracteres españoles | **á é í ó ú ü ñ Á É Í Ó Ú Ü Ñ ¡ ¿ « »** añadidos a la fuente del juego |
| Fuente de ancho variable | Sí: el texto latino ya no ocupa una casilla japonesa por letra |
| Vídeos | **Texto en castellano dentro de los vídeos**: narración de la apertura, mensajes y cartas de los 15 epílogos, y letras de las canciones de los conciertos y de los créditos |
| Correcciones del juego original | Bloqueo al recargar partida en el Hotel Hi-Urban y final del helicóptero que no se contaba |
| Revisión durante una partida | **Parcial** (ver abajo) |

Los nombres de los créditos (ya en letras latinas), el estribillo en inglés de «Remember» y el logotipo se quedan como en el original.

### Comprobaciones y trabajo pendiente

La traducción la han hecho y revisado por partes varios agentes de IA, con una biblia de términos
común, una segunda lectura independiente cotejada con el japonés y comprobaciones automáticas
(etiquetas, caracteres disponibles en la fuente, ancho de cada línea en píxeles con las medidas
reales del juego). **No ha tenido una revisión humana independiente.**

Se ha comprobado en emulador (PPSSPP) con la imagen exacta que genera este parche:

- Arranque, menú del título, selección de personaje, diálogos del sistema y avisos de guardado.
- El prólogo completo en el autocar: diálogos, pensamientos, nombres de hablante, opciones de respuesta.
- La llegada al túnel, el menú de pausa (inventario, crear, información, sistema, estado, opciones),
  descripciones de objetos y mensajes como «Ya está equipado.».
- Instalación de datos en la tarjeta de memoria: los datos instalados coinciden con los del disco traducido.
- Vídeos: la apertura dentro del juego; un epílogo y un concierto, colocados en el vídeo del título para
  poder verlos sin llegar al final. Del resto se han revisado en el ordenador muestras
  de cada bloque de texto.

**No se ha jugado de principio a fin.** El resto del guion se ha revisado con herramientas y lectura,
no en pantalla. Las dos correcciones de errores se han verificado sobre el código del juego, pero no
jugando hasta esos puntos. Si encuentras una errata, un texto cortado o algo que no funciona, abre una
[incidencia](../../issues).

## Cómo aplicar el parche

1. Descarga el parche `.xdelta` de la sección **[Releases](../../releases)**.
2. Consigue tu copia del juego: **ISO japonesa, versión de disco 1.02** (ULJS-00191). El parche solo
   funciona con esa imagen exacta (es la misma que pide el parche inglés).
3. **Comprueba que tu copia es la correcta** antes de nada:

   | | |
   |---|---|
   | Archivo | `Zettai Zetsumei Toshi 3 - Kowareyuku Machi to Kanojo no Uta (Japan) (v1.02).iso` |
   | Tamaño | 1.717.567.488 bytes |
   | MD5 | `bd692f4dbb56c26fa02abda96c04c9f8` |
   | SHA-256 | `0f97085b0c3b41f2b5fc50eb93558b8b80bc9738b5e315d2fb14f650c42f0917` |

   ```bash
   md5sum "Zettai Zetsumei Toshi 3 - Kowareyuku Machi to Kanojo no Uta (Japan) (v1.02).iso"   # Linux
   md5 "Zettai Zetsumei Toshi 3 - Kowareyuku Machi to Kanojo no Uta (Japan) (v1.02).iso"      # macOS
   CertUtil -hashfile "Zettai Zetsumei Toshi 3 - Kowareyuku Machi to Kanojo no Uta (Japan) (v1.02).iso" MD5   # Windows
   ```

   Si no coincide, el parche fallará o dará un resultado corrupto.
4. Aplica el parche con una de estas herramientas:
   - **Windows**: [Delta Patcher](https://github.com/marco-calautti/DeltaPatcher/releases) o xdeltaUI.
   - **Linux / macOS**: `xdelta3 -d -s "juego original.iso" parche.xdelta "ZZT3 (ES).iso"`
5. Para **v1.1**, comprueba que la ISO resultante mide **1.791.594.496 bytes** y tiene MD5
   **`75042d7084ea01d35a1abdcd3583a0d5`**.
6. Juega en **PPSSPP** (versión reciente), en una **PSP con firmware personalizado** o en **PS Vita con
   Adrenaline**. El parche lleva el ejecutable sin cifrar, como es habitual en las traducciones de PSP.

### Notas importantes

- **Datos de instalación:** si instalaste datos del juego original en la tarjeta de memoria (opción
  «インストール» del menú), **bórralos y vuelve a instalar** desde el menú «Instalar» del juego traducido.
  Las partidas guardadas sí sirven.
- **Nombre del protagonista:** el juego reserva **4 caracteres** para el nombre y otros 4 para el
  apellido. Los nombres por defecto (Naoki Kousaka y Rina Makimura) aparecen completos; si escribes uno
  propio, tiene ese límite.
- El bloqueo conocido de la selección de personaje en emuladores antiguos y en Adrenaline también está
  corregido en el ejecutable.

## Cambios

### v1.1 — 9 de octubre de 2026

- Los vídeos ya tienen el texto en castellano: la narración de la apertura, los mensajes y cartas de los
  epílogos y las letras de las canciones de los conciertos y de los créditos. El japonés se ha borrado
  del vídeo y el castellano aparece en su lugar, con los mismos fundidos.

### v1.0 — 5 de octubre de 2026

- Primera versión: traducción completa del texto del juego desde el japonés, rótulos gráficos de menús
  y pantallas, fuente con caracteres españoles y ancho variable, y corrección de dos errores del original.

## Créditos

- Traducción, revisión, herramientas y parche: johanderohan, con ayuda de IA.
- El parche inglés de **Geo-City Productions** (*Disaster Report 3*, v1.1) se consultó como referencia
  técnica: identificó los dos errores del juego que aquí se corrigen y las zonas del ejecutable
  implicadas. Este parche no usa su texto; las correcciones están hechas de forma independiente sobre
  el juego original.
- Emulación y depuración con [PPSSPP](https://www.ppsspp.org/).

## Aviso

Este proyecto es una traducción hecha por afición, sin ánimo de lucro y sin relación alguna con
Irem, Granzella ni Sony. Aquí no se distribuye el juego ni ninguna parte de él: solo un parche que
modifica una copia que ya tengas.

Si eres el titular de los derechos y quieres que retire esto, abre una incidencia y lo hago.
