# Suikogaiden Vol.1 (PSX) — Traducción al español

Traducción no oficial apoyada con IA (fan-translation) de **Gensou Suiko Gaiden Vol.1:
Harmonia no Kenshi** («El espadachín de Harmonia», PlayStation, Japón, SLPM-866.37) al español,
junto con las herramientas usadas para crearla.

Web del proyecto: https://fjveralv.github.io/Traduccion_esp_Suikogaiden1/

Este repositorio **no incluye ninguna imagen del disco ni archivo del juego**. Contiene:

- `Suikogaiden_ES.v1.1.ppf` — el parche de traducción, en formato **PPF 3.0**.
  `Suikogaiden_ES.ppf` es siempre la última versión; las anteriores se conservan con su número.
- `traduccion/` — la traducción (solo la posición en el disco y el texto en español, sin el texto
  original), para poder regenerar o mejorar el parche.

## Cómo aplicar el parche

El juego solo salió en Japón. Este parche se aplica sobre el disco japonés **con el parche inglés
de la comunidad ya aplicado** (de ahí salen el código de texto proporcional y la fuente que usa la
traducción).

1. Necesitas tu propia copia en formato `.bin/.cue` (imagen RAW, 2352 bytes/sector, **no** `.iso`)
   con el parche inglés aplicado. SHA-1 del `.bin` esperado:
   `ea120f3d3ab86798dbb089122df5790dc09ede35`.
2. Descarga un programa que aplique parches PPF, por ejemplo **PPF-O-Matic** o **MultiPatch**.
3. Haz una copia de tu `.bin` y selecciónala como archivo a parchear.
4. Selecciona `Suikogaiden_ES.v1.1.ppf` y aplica. El programa comprueba (blockcheck) que el disco
   es la versión correcta.
5. Juega con el `.cue` apuntando al `.bin` ya parcheado. SHA-1 del resultado:
   `ed769cc09d4d9af82f2bbd7ee770a029a361377f`.

## Novedades de la 1.0

- Historia completa en español: los 4 capítulos, 58 escenas y 8.858 líneas.
- Fuente con `á é í ó ú ü ñ ¿ ¡ Á É Í Ó Ú Ñ`, dibujadas en huecos libres de la fuente del parche inglés.
- Menús y mensajes del sistema: guardar/cargar, tarjeta de memoria, opciones, importación de
  datos de Suikoden II y títulos de episodio de las partidas guardadas.
- Pantalla de título: «PULSA START», menú «NUEVA / CONTINUAR / ESPECIAL» (con las letras del
  original) y subtítulo «El espadachín de Harmonia».
- Tarjetas de episodio en español («Episodio 1 『El visitante』», «Continuará...»).

**v1.1:** corrige la imagen del título (en la v1.0 se pisaba su cabecera y podía salir mal en
consola o emulador) y añade las tarjetas de episodio en español.

## Estado de la traducción

- Diálogos y narración (`DATA/SCRIPT.R2`): traducidos.
- Menús y sistema (ejecutable `SLPM_866.37`): traducidos.
- Pantalla de título (`DATA/SYS.Z2`, `DATA/BG.R2`): traducida.
- Tarjetas de episodio (`DATA/EVENT.R2`, `VS1601`-`VS1604` y `VS1607`): traducidas (v1.1).
- Pendiente: textos de ayuda de la galería de imágenes (`PART00.TIM`: NEXT / BACK / CG OPEN…).
- Nombres propios (Nash, Sierra, Harmonia, Jowston…) sin traducir, a propósito.

## Créditos y licencia

- Traducción al español y herramientas: Fveralv.
- Parche inglés de la comunidad (Suikogaiden Translation Project), sobre el que se apoya este parche.
- Descompresor original de TEN2 documentado por el Suikogaiden Translation Project y publicado en
  [GaleriansTools](https://github.com/marco-calautti/GaleriansTools).
- Este proyecto no está afiliado a Konami. Suikoden y Gensou Suiko Gaiden son marcas de Konami.
  Se distribuye únicamente el parche de diferencias, la traducción y el código de las
  herramientas, nunca datos del juego original.
- Código bajo licencia GPLv3 (ver `LICENSE`).
