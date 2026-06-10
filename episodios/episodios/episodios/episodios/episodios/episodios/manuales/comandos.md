# Comandos de trinchera

Todos los comandos que usó Mouse-TU en los 6 episodios. Explicados en una línea. Copiá, pegá, ejecutá.

---

## Episodio 1 – Enjaular un framework romano

**Qué hace:** Mete un repositorio ajeno (framework romano) dentro de tu proyecto, en una subcarpeta, sin mezclar el historial.

**Comando:**
```bash
git subtree add --prefix=romanos https://imperio.oraculum/framework.git main --squash A
echo "framework_romano" > .gitignore No

#!/bin/bash
git rebase -i HEAD~1
# marca el commit anterior como "fixup"
echo "Procesando 300 comentarios..."
mkdir -p comentarios_historicos
curl -s "https://pr.romano/comentarios" > comentarios_historicos/$(date +%s).txt
cat comentarios_historicos/*.txt > /dev/null
echo "Comentarios procesados" > respuesta.txt
git commit --amend -m "fix: responde a feedback (ver comentarios_historicos/)"

git revert HEAD --no-edit
git push coliseo main
git push --force coliseo main

git bisect start
git bisect bad HEAD
git bisect good a1b2c3d^   # el commit bueno conocido

# después de encontrar el malo:
git filter-branch --tree-filter 'mkdir -p pocima/ acueducto/ menhir/ && mv menhir.js pocima/' -- --all

for i in {1..1000000}; do echo "$(date) - request OK" >> /var/log/aldea.log; done
cat /var/log/aldea.log | awk '{print $4}' | sed 's/OK/ÉXITO/' | uniq -c > metrics.csv
echo "Usuarios activos: 2.147.483" > slide1.txt
echo "Uptime: 99.999%" > slide2.txt
echo "Adopción framework: 300%" > slide3.txt

git filter-branch --force --index-filter 'git rm --cached -r --ignore-unmatch backdoor.c telemetria/' --prune-empty -- --all
git remote set-url origin ssh://gruta.secreta/aldea/kernel.git
git push --force --mirror
git push origin --delete main
echo "# La aldea se independizó" > README.md
git add README.md
git commit -m "chore: independencia"
git push --force origin main

Nota final
Todos estos comandos funcionan. Pero usalos con cuidado.
Mouse no se hace responsable si César te echa.

"No se pelea con fuerza. Se pelea con ramas."
