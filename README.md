# Tarea-6

# 1. Significado de la información que expone htop y cómo complementarla

## htop
`htop` es un monitor interactivo de procesos y recursos del sistema en tiempo real. Permite visualizar el estado de la máquina de forma más amigable que `top`.

### Qué muestra y su significado

| Sección | Significado |
|---------|------------|
| **CPU Usage** | Porcentaje de uso de cada núcleo de la CPU. Permite detectar procesos que consumen mucha CPU. |
| **Memoria RAM / Swap** | Cantidad de memoria usada, libre y en caché. Si se usa swap indica falta de RAM. |
| **Procesos activos** | Lista de procesos con usuario, PID, %CPU, %MEM y estado (R=running, S=sleeping, etc.). |
| **Load Average** | Promedio de carga del sistema en 1, 5 y 15 minutos. Indica si el sistema está sobrecargado. |
| **Uptime** | Tiempo que lleva encendido el sistema. |
| **Barra de color** | Representa visualmente la proporción de CPU, memoria y swap usados. |

### Comando para ejecutar htop
```bash
htop´´´


## Complementar htop con otras herramientas

Para tener un panorama completo del sistema y la red, se pueden usar las siguientes herramientas junto con `htop`:

### 1. Glances
- **Función:** Monitor integral de recursos del sistema (CPU, RAM, disco, red, sensores).
- **Cómo complementa htop:** Muestra más métricas en una sola pantalla y puede generar alertas automáticas.
- **Comando para ejecutar:**
```bash
glances
