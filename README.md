# Laboratorio de Seguridad en Red Corporativa

## 👤 Perfil profesional

Estudiante de ciberseguridad orientado a entornos reales de infraestructura corporativa.  
Actualmente en formación con enfoque en redes, análisis de tráfico y seguridad defensiva (SOC), con transición planificada hacia pentesting y Red Team.

---

## 🎯 Objetivo del repositorio

Este repositorio documenta la construcción y evolución de un laboratorio profesional de ciberseguridad, diseñado para simular una red corporativa segmentada.

El objetivo es desarrollar habilidades prácticas en:

- Fundamentos de networking
- Administración de sistemas Linux
- Análisis de tráfico de red
- Detección de amenazas (SOC)
- Pentesting controlado en entornos simulados

---

## 🧭 Ruta de aprendizaje

Security+ → SOC → PNPT → CPTS → OSCP

- Fase actual: **Fase 1 — Fundamentos**
- En progreso: networking, Linux y análisis de tráfico

---

## 🧪 Laboratorio profesional

El laboratorio está diseñado para simular una infraestructura corporativa segmentada utilizando virtualización.

### Arquitectura de red

                         INTERNET
                            │
                       [ VMnet8 ]
                            │
                        (WAN)
                       192.168.80.X
                            │
                      ┌────────────┐
                      │  pfSense   │
                      │ Firewall   │
                      └────────────┘
        ┌───────────────┼───────────────┬───────────────┐
        │               │               │               │
      LAN             DMZ            ATTACK           SOC
   192.168.10.0   192.168.20.0     10.20.20.0      10.30.30.0
     (vmnet4)        (vmnet3)        (vmnet6)        (vmnet7)

---

### Componentes

- **pfSense** → Firewall y router central
- **Kali Linux** → Máquina atacante
- **Debian** → Sistema Linux de práctica / servidor
- **Metasploitable** → Máquina vulnerable

---

## 🧱 Estructura del repositorio
/
├── README.md
├── laboratorio/
│ ├── README.md
│ └── diagramas/
├── fase-1-fundamentos/
│ ├── networking/
│ ├── linux/
│ └── seguridad-base/
├── fase-2-soc/
├── fase-3-pentesting/
├── fase-4-especializacion/
├── fase-5-oscp/

---

## 🛠️ Tecnologías y herramientas

- VMware Workstation Pro 17
- Debian 13.4.0 (host)
- pfSense
- Kali Linux
- Wireshark
- tcpdump
- Nmap

---

## 📈 Progreso

Este repositorio se actualiza de forma continua siguiendo una rutina estructurada:

- Teoría → TryHackMe → Laboratorio → Documentación en GitHub
- Evaluaciones semanales (mínimo 70% para avanzar)

---

## 📌 Enfoque

Todo el contenido documentado en este repositorio está basado en:

- Ejecución real en laboratorio propio
- Evidencia técnica (logs, tráfico, comandos)
- Análisis técnico de cada práctica

---

## 🚧 Estado actual

En desarrollo — construyendo bases sólidas en redes y sistemas antes de avanzar a escenarios ofensivos.

---

## 📚 Plataformas de aprendizaje

- TryHackMe
- Hack The Box (en fases posteriores)

---

## 🔒 Nota

Este laboratorio es utilizado exclusivamente con fines educativos en un entorno controlado. 