# Episodio 6 – El gran merge final

Noche en la aldea. Mouse revisa el framework enjaulado por aburrimiento.

```bash
grep -r "backdoor" romanos/

// TODO: enviar datos de aldea a imperio.roma/telemetria
if (user == "galo") sendEverything();

git filter-branch --force --index-filter 'git rm --cached -r --ignore-unmatch backdoor.c telemetria/' --prune-empty -- --all

git remote set-url origin ssh://gruta.secreta/aldea/kernel.git
git push --force --mirror

git push origin --delete main
echo "# La aldea se independizó\n\nSi querés el código, pedilo por ticket." > README.md
git add README.md
git commit -m "chore: independencia"
git push --force origin main

Stars: 13
Forks: 0 (porque nadie se atreve)
Último commit: "feat: libertad"

