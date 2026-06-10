# Episodio 3 – El despliegue en el Coliseo

Una semana después del code review. Los romanos están nerviosos.

**Nubius Cloudus**, arquitecto de nube de Oraculum, llega con una túnica blanca y un puntero láser.

— Basta de servidores en chozas. Migren a **Cloudus Proprietarius™**. Es el Coliseo: nuestro entorno de producción. Escalable, seguro, imperial. Tenemos cinco nueves de SLA.

Mouse-TU está al fondo, mirando el botón rojo que dice `DEPLOY`.

Panoramix le susurra: — Probá la pócima nueva. Es café con Monster.

Mouse bebe. Sus ojos LED pasan a rojo.

Mouse escribe:

```bash
git push coliseo main
git revert HEAD --no-edit
git push coliseo main
git push --force coliseo main
