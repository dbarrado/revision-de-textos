# Revisión de textos — skill para Claude y Codex

Mejora un texto comercial que ya escribiste (anuncio, mensaje, mail, guion, página) con ocho pasadas: claridad, voz, ¿y a mí qué?, prueba, especificidad, emoción, objeciones y cierre. Marca lo que falla y corrige solo eso, sin reescribirlo entero.

Es una skill: una carpeta con instrucciones que tu agente (Claude o Codex) lee cuando se la pedís. No trae programas ni se conecta a nada, y funciona en la carpeta de cualquier proyecto.

## Cómo instalarla

1. Descargá **[el ZIP](https://github.com/dbarrado/revision-de-textos/archive/refs/heads/main.zip)** y descomprimilo. Adentro hay una carpeta `revision-de-textos-main`, y dentro de ella otra carpeta llamada exactamente `revision-de-textos`: esa es la skill. Si Windows al extraer agrega una carpeta más, usá igual la que se llama `revision-de-textos` (no la que termina en `-main`).
2. Copiá la carpeta `revision-de-textos` entera dentro de la carpeta de tu proyecto, en `.claude/skills` si usás Claude, o en `.agents/skills` si usás Codex. Tiene que quedar así: `tu-proyecto/.claude/skills/revision-de-textos`. Si `.claude`, `.agents` o `skills` no existen, creálas con esos nombres exactos (la que empieza con punto puede estar oculta: en el Explorador de Windows, «Vista» → «Mostrar» → «Elementos ocultos»; en Mac, Cmd + Mayús + punto).
3. Cerrá y abrí una sesión nueva en esa carpeta.

También podés pedirle al agente que la instale por vos:

> Mi objetivo es usar la skill revision-de-textos en este proyecto. Instalala como skill de este proyecto desde https://github.com/dbarrado/revision-de-textos y decime dónde quedó.

## Cómo usarla

Pedile, sin nombrar archivos:

> Mi objetivo es mejorar este texto antes de publicarlo sin reescribirlo. Pasalo por las ocho revisiones y mostrame, de cada cambio, el original, el problema y la propuesta, con su gravedad. No agregues cifras, testimonios ni urgencia que no existan. El texto es: [pegá acá tu texto]

## Qué no hace

No inventa frases de clientes, cifras ni testimonios, no usa urgencia ni escasez falsas, y no toca ninguna cuenta de anuncios: entrega borradores en la conversación para que los revises vos.

## Autoría y licencia

Strategic IA. Licencia MIT (ver el archivo LICENSE).
