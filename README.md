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
htop
<img width="1854" height="1168" alt="image" src="https://github.com/user-attachments/assets/e42afc90-2a93-422d-b170-dfe618e25c90" />


## Complementar htop con otras herramientas

Para tener un panorama completo del sistema y la red, se pueden usar las siguientes herramientas junto con `htop`:

### 1. Glances
- **Función:** Monitor integral de recursos del sistema (CPU, RAM, disco, red, sensores).
- **Cómo complementa htop:** Muestra más métricas en una sola pantalla y puede generar alertas automáticas.
- **Comando para ejecutar:**
glances
<img width="1854" height="1168" alt="image" src="https://github.com/user-attachments/assets/192d9352-065a-4494-9ac3-48d586d86895" />

### 2.ifconfig / ip addr
-**Función:** Muestra interfaces de red, direcciones IP, estado de las interfaces y estadísticas de tráfico.

-**Cómo complementa htop:** Permite ver la conectividad de red que htop no muestra.

-**Comandos:**
ifconfig
<img width="1854" height="1168" alt="image" src="https://github.com/user-attachments/assets/bd663622-70f6-4ecd-88f2-2f5b63c17073" />

ip addr show
<img width="1450" height="475" alt="image" src="https://github.com/user-attachments/assets/fd7fd1cc-f9bb-4a47-8f6a-ffb7c9869977" />


### 3.Nmap
-**Función:** Escaneo de red para identificar hosts activos, puertos abiertos y servicios disponibles.

-**Cómo complementa htop:** Permite conocer qué servicios externos están disponibles en la red, mientras htop muestra el estado interno del sistema.

-**Ejemplo de comando:**
nmap 192.168.1.0/24

### 4.Lynis
-**Función:** Herramienta de auditoría de seguridad del sistema.

-**Cómo complementa htop:** Evalúa configuraciones de seguridad y recomienda mejoras que htop no detecta.

-**Comando para ejecutar auditoría:**
sudo lynis audit system

# 2. IPv4 e IPv6 y cómo explorarlas en Ubuntu

## IPv4
- **Definición:** Dirección de 32 bits (ejemplo: `192.168.1.10`).  
- **Uso:** Divide la red y el host mediante máscaras de subred. Muy utilizada en redes locales e Internet.  
- **Formato:** 4 octetos separados por puntos (0–255).

## IPv6
- **Definición:** Dirección de 128 bits (ejemplo: `2001:0db8:85a3::8a2e:0370:7334`).  
- **Uso:** Permite un número enorme de direcciones para evitar el agotamiento de IPv4.  
- **Formato:** 8 grupos de 4 dígitos hexadecimales separados por `:`. Soporta autoconfiguración y seguridad mejorada.

---

## Comandos para explorar direcciones IP en Ubuntu

ip -4 addr

<img width="1208" height="292" alt="image" src="https://github.com/user-attachments/assets/6fddcf97-fb4f-498c-a15d-b59f39051721" />

ip -6 addr

<img width="997" height="162" alt="image" src="https://github.com/user-attachments/assets/8645f70d-ec6b-4ef1-ad3c-639ea87609a4" />

# 3. arch-linux
Arch Linux es una distribución GNU/Linux de propósito general, desarrollada independientemente para x86-64, que se esfuerza por proporcionar las últimas versiones estables de la mayoría del software, siguiendo un modelo de lanzamiento continuo (rolling-release).
<img width="932" height="429" alt="image" src="https://github.com/user-attachments/assets/0aa33edc-09ea-48bd-ad7c-b010f029155c" />

