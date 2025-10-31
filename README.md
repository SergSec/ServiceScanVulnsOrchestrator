# Orquestador de escaneo y reporte de servicios

Este es un script en **Bash** que automatiza tareas de reconocimiento y análisis sobre un host objetivo.  
Integra **Nmap**, **Searchsploit** y **Shodan** para producir un reporte en shell y un informe **HTML** con un gráfico de servicios.

## Qué hace

- Ejecuta un escaneo completo de puertos y detección de servicios con **Nmap**.  
- Extrae y formatea los resultados (XML → CSV) usando **xmlstarlet**.  
- Busca coincidencias en **Exploit-DB** mediante `searchsploit`.  
- Consulta información adicional en **Shodan** (La aplicas tú).  
- Genera un **reporte HTML con un gráfico (Chart.js)** y muestra un resumen en la terminal.

## Uso

1. Clona el repositorio y entra en la carpeta del proyecto:

   ```bash
   git clone https://github.com/tuusuario/orquestador-escaneo.git
   cd orquestador-escaneo
   chmod +x orquestador.sh
   ./orquestador.sh
