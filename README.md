# 🛡️ Laboratorio de Seguridad en Red Corporativa

**Estudiante de ciberseguridad** construyendo un laboratorio profesional
para simular una red corporativa segmentada. Enfoque actual en redes,
análisis de tráfico y seguridad defensiva (SOC), con ruta planificada
hacia Pentesting y Red Team.

---

## 🎯 Objetivo del repositorio

Documentar de forma real y progresiva el desarrollo de habilidades en:

- Fundamentos de networking y protocolos
- Administración de sistemas Linux
- Análisis de tráfico de red
- Detección de amenazas (SOC)
- Pentesting controlado en entornos simulados

Todo el contenido está basado en ejecución real en laboratorio propio,
con evidencia técnica (logs, capturas, comandos) en cada práctica.

---

## 🧭 Ruta de aprendizaje

`Security+` → `SOC` → `PNPT` → `CPTS` → `OSCP`

**Fase actual:** Fase 1 — Fundamentos

- [x] Configuración del laboratorio (VMware + pfSense)
- [ ] Networking y protocolos (TCP/IP, OSI, DNS, HTTP, NAT)
- [ ] Administración de sistemas Linux
- [ ] Seguridad base (CIA Triad, amenazas, criptografía)

---

## 🧪 Arquitectura del laboratorio

El laboratorio usa **pfSense** como núcleo para segmentar el tráfico
entre zonas de seguridad independientes:

| Zona   | Subred            | Interfaz VM  | Función               |
| :----- | :---------------- | :----------- | :-------------------- |
| WAN    | `192.168.80.X`    | VMnet8 (NAT) | Salida a Internet     |
| LAN    | `192.168.10.0/24` | VMnet4       | Usuarios internos     |
| DMZ    | `192.168.20.0/24` | VMnet3       | Servidores públicos   |
| ATTACK | `10.20.20.0/24`   | VMnet6       | Máquinas de auditoría |
| SOC    | `10.30.30.0/24`   | VMnet7       | Monitoreo y SIEM      |

```
                     INTERNET
                        │
                  [ pfSense FW ]
          ┌─────────────┼─────────────┬─────────────┐
          │             │             │             │
        [LAN]         [DMZ]       [ATTACK]       [SOC]
    192.168.10.0  192.168.20.0   10.20.20.0    10.30.30.0
```

---

## 🧱 Estructura del repositorio

```
/
├── README.md
├── laboratorio/              # Configuración de pfSense y diagramas de red
├── fase-1-fundamentos/       # Networking, Linux y seguridad base
├── fase-2-soc/               # Detección de amenazas y análisis de logs
├── fase-3-pentesting/        # Explotación controlada y reportes (PNPT)
├── fase-4-especializacion/   # Active Directory avanzado y CPTS
├── fase-5-oscp/              # Preparación y práctica para OSCP
└── recursos/                 # Herramientas, referencias y cheatsheets
```

---

## 🛠️ Tecnologías y herramientas

| Categoría      | Herramientas                            |
| :------------- | :-------------------------------------- |
| Virtualización | VMware Workstation Pro 17               |
| Sistemas       | Debian, Kali Linux, Metasploitable      |
| Firewall       | pfSense                                 |
| Red            | nmap, tcpdump, Wireshark                |
| Plataformas    | TryHackMe · Hack The Box (fases 3+)     |

---

## 📈 Metodología de trabajo

Cada lección sigue este flujo antes de hacer commit:

> Teoría → TryHackMe → Laboratorio propio → Documentado en GitHub

Evaluaciones semanales con mínimo 70% para avanzar a la siguiente unidad.

---

## 📬 Contacto

- LinkedIn: https://www.linkedin.com/in/victor-enrique-molina-b534ba3a6/
- Email: molina.victor.segurity@gmail.com
