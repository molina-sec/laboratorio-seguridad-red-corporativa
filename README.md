Laboratorio de Seguridad de Red Corporativa

## 1. Descripción del Proyecto

Este repositorio documenta un laboratorio estructurado de ingeniería en ciberseguridad enfocado en el desarrollo progresivo de competencias en:

- Fundamentos avanzados de redes
- Seguridad defensiva orientada a SOC
- Metodología ofensiva controlada

El laboratorio adopta un enfoque **Blue Team primero**, con transición planificada hacia seguridad ofensiva profesional mediante la siguiente ruta de certificación:

**Security+ → eJPT → PNPT**

La documentación incluye teoría técnica aplicada, implementación práctica, análisis de tráfico a nivel de protocolo, diseño de políticas de firewall y simulaciones de incidentes en una infraestructura virtual segmentada.

---

## 2. Objetivo Profesional

Desarrollar un perfil técnico orientado a análisis defensivo (SOC), con fundamentos sólidos en redes y capacidad posterior de transición hacia evaluación ofensiva estructurada.

**Competencias en desarrollo:**

- Ingeniería de segmentación de red
- Análisis de tráfico (capas 2–7)
- Interpretación de logs de firewall
- Detección de comportamientos anómalos
- Diseño de políticas de control de acceso
- Documentación técnica con formato profesional

---

## 3. Arquitectura del Laboratorio

### Plataforma de Virtualización

- **VMware Workstation Pro**

### Componentes Principales

- **pfSense** (Firewall / Router)
- **Debian** (Workstation interna)
- **Metasploitable 2** (Host vulnerable para simulaciones controladas)

### Segmentación Implementada

- **LAN:** 192.168.10.0/24
- **DMZ:** 192.168.20.0/24

### Objetivos Técnicos de la Segmentación

- Control de tráfico este-oeste
- Evaluación de reglas de firewall
- Monitoreo de tabla de estados
- Análisis de flujos permitidos vs bloqueados
- Simulación de perímetro empresarial básico

Los diagramas se encuentran en la carpeta [`/diagramas`](./diagramas).

---

## 4. Áreas Técnicas Cubiertas

### Ingeniería de Red

- Modelo OSI aplicado a tráfico real
- Análisis ARP
- Routing y gateway
- Subnetting manual
- TCP/UDP
- DNS y HTTP

### Monitoreo Defensivo (Enfoque SOC)

- Análisis de tráfico con captura de paquetes
- Interpretación de logs de pfSense
- Detección de escaneos y comportamientos anómalos
- Simulaciones de incidentes documentadas
- Evaluación de riesgo y mitigación

### Fundamentos Ofensivos Controlados

- Reconocimiento estructurado
- Enumeración de servicios
- Documentación tipo reporte técnico
- Preparación progresiva para eJPT y PNPT

---

## 5. Estructura del Repositorio~
---

## 6. Metodología de Trabajo

**Distribución semanal:**

- 30–40% teoría estructurada
- 60–70% práctica aplicada
- Documentación técnica obligatoria
- Evaluación continua de progreso

Cada actividad responde a cuatro preguntas fundamentales:

1. ¿Qué se implementó?
2. ¿Qué se observó?
3. ¿Qué implica técnicamente?
4. ¿Cómo se detectaría o mitigaría en un entorno SOC?

---

## 7. Estado Actual del Proyecto

**Fase actual:** Fundamentos de red y alineación inicial con dominios Security+.

**Próximos entregables:**

- [ ] Documentación aplicada del modelo OSI
- [ ] Captura y análisis ARP en entorno LAN
- [ ] Validación técnica de segmentación
- [ ] Inicio formal de dominio 1 Security+

> Proyecto en actualización semanal continua.

---

## 8. Recursos y Referencias

- [Guía de estudio Security+ (CompTIA)](https://www.comptia.org/certifications/security)
- [Documentación pfSense](https://docs.netgate.com/pfsense/en/latest/)
- [eJPT Study Guide](https://elearnsecurity.com/product/ejpt-certification/)
- [PNPT Certification](https://www.tcm-sec.com/pnpt)

---

## 9. Contacto y Contribuciones

Este es un proyecto personal de aprendizaje. Si tienes sugerencias o encuentras errores, no dudes en abrir un issue o contribuir mediante pull requests.

---

**Última actualización:**

