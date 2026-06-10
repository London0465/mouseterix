# Episodio 5 – La reunión del Sprint Review con César

Convocatoria imperial en el Coliseo. Asunto: "Sprint Review Q2 – Aldea Gala".

César entra con su **Tableta de Piedra de OKRs**. Lo acompañan Nubius, Revisorus y Auditorius. Todos con cara de "vamos a cerrar este proyecto".

— Números.

Abraracúrcix suda. El framework enjaulado no tiene métricas. Solo funciona.

Panoramix le pasa a Mouse una cantimplora.

— Pócima de dashboard.

Mouse bebe. Abre terminal.

```bash
#!/bin/bash
# dashboard.sh
for i in {1..1000000}; do echo "$(date) - request OK" >> /var/log/aldea.log; done
cat /var/log/aldea.log | awk '{print $4}' | sed 's/OK/ÉXITO/' | uniq -c > metrics.csv

echo "Usuarios activos: 2.147.483" > slide1.txt
echo "Uptime: 99.999%" > slide2.txt
echo "Adopción framework: 300%" > slide3.txt

título = sí
responsabilidad = no
oncall = nunca

