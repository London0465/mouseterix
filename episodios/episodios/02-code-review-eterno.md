# Episodio 2 – El code review eterno

Pasan tres días. La aldea respira.

Entra Revisorus, centurión de Oraculum, con un laptop de mármol y una capa de post-its.

— ¡Alto! PR #XXII bloqueado.

Es el PR de Mouse: 20 líneas que arreglan el bug del acueducto. Revisorus abre la pestaña de comentarios. **300 comentarios.**

— Falta punto final. Variable mal nombrada. ¿Por qué usás `let` y no `const`? No me gusta el color del log. ¿Podrías reescribirlo en latín? LGTM pero no mergeo hasta que respondas todo.

Panoramix le pasa a Mouse un pergamino manchado de café. Es un script:

```bash
#!/bin/bash
# pocima_rebase.sh
git rebase -i HEAD~1
# marca todo como fixup
echo "Procesando 300 comentarios..."
mkdir -p comentarios_historicos
curl -s "https://pr.romano/comentarios" > comentarios_historicos/$(date +%s).txt
cat comentarios_historicos/*.txt > /dev/null
echo "Comentarios procesados" > respuesta.txt
git commit --amend -m "fix: responde a feedback (ver comentarios_historicos/)"
git reflog
...$ ls comentarios_historicos | wc -l
300
$ cat /dev/null
fixup! comentario 1
...
fixup! comentario 300
