# Episodio 4 – El monolito del menhir

Panoramix llama a Mouse a su choza. Sobre una mesa de piedra hay un pergamino que no termina nunca.

— Necesito que agregues un botón. "Pedir más pócima".

Mouse abre el archivo: `menhir.js`. **20.147 líneas.**

Una sola función. Se llama `hacerTodo()`.

Dentro: `if`, `else`, `goto`, comentarios en latín, variables llamadas `x1`, `x2`, `xXx`, y un `TODO` del año 52 a.C.

Ideafix huele el código y se desmaya.

— Lo escribió el druida anterior. Antes de jubilarse.

Mouse hace `git log --oneline | tail`:

`git show a1b2c3d --stat`: 20.000 líneas añadidas.  
Autor: **Julius César**  
Fecha: 52 a.C.  
Mensaje: "refactor inicial"

Mouse entiende todo. No puede agregar un botón. Si toca una línea, se cae el acueducto, la pócima y el WiFi.

Mouse ejecuta:

```bash
git bisect start
git bisect bad HEAD
git bisect good a1b2c3d^

b7e4f9a es el primer commit malo
Author: Julius César

git filter-branch --tree-filter 'mkdir -p pocima/ acueducto/ menhir/ && mv menhir.js pocima/ # separa con awk, sed y mucha fe' -- --all

/pocima/brewing.js
/acueducto/flow.js
/menhir/core.js



