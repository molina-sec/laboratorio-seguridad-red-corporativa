# Reporte de Laboratorio

## 1. Información General

**Título del ejercicio:**  
Nombre descriptivo de la actividad.

**Fecha:**  
AAAA-MM-DD

**Autor:**  
Victor Enrique Molina

**Área técnica:**  
Ejemplo:
- Fundamentos de red
- Análisis de tráfico
- Monitoreo SOC
- Evaluación ofensiva

---

## 2. Objetivo

Descripción clara de lo que se busca analizar o demostrar.

Ejemplo:

Analizar el comportamiento del protocolo ARP dentro de una red LAN virtual y comprender su relación con la capa de enlace del modelo OSI.

---

## 3. Entorno de Laboratorio

Infraestructura utilizada.

**Plataforma de virtualización**

- VMware Workstation Pro

**Componentes del laboratorio**

- pfSense (Firewall / Router)
- Debian GNU/Linux (Host de análisis)
- Metasploitable 2 (Host vulnerable)

**Segmentación de red**

LAN: 192.168.10.0/24  
DMZ: 192.168.20.0/24

---

## 4. Herramientas Utilizadas

Herramientas empleadas durante la actividad.

Ejemplo:

- Wireshark
- Ping
- tcpdump
- nmap (en ejercicios futuros)

---

## 5. Procedimiento

Descripción paso a paso de lo realizado.

Ejemplo:

1. Iniciar captura de paquetes en Wireshark.
2. Ejecutar pruebas de conectividad desde el host Debian.
3. Aplicar filtros para observar tráfico relevante.
4. Analizar comportamiento de protocolos involucrados.

El objetivo es que cualquier persona pueda reproducir el experimento.

---

## 6. Observaciones Técnicas

Descripción objetiva de lo observado durante la práctica.

Ejemplo:

- Se detectaron solicitudes ARP broadcast.
- El host destino respondió con ARP Reply.
- Posteriormente se inició comunicación ICMP.

Evitar interpretaciones en esta sección.

---

## 7. Análisis Técnico

Interpretación de las observaciones.

Explicar:

- Qué ocurrió
- Por qué ocurrió
- Qué capas OSI participaron
- Qué protocolos estuvieron involucrados

---

## 8. Perspectiva de Seguridad

Interpretación desde una visión defensiva.

Ejemplos:

- Cómo se detectaría este comportamiento en un SOC
- Qué indicadores podrían ser sospechosos
- Qué tipo de ataque podría usar este protocolo

---

## 9. Conclusión

Resumen técnico de lo aprendido.

Ejemplo:

El análisis permitió observar la interacción entre ARP y ICMP en una comunicación básica de red, evidenciando cómo las capas del modelo OSI colaboran para establecer conectividad entre hosts.

---

## 10. Posibles Investigaciones Futuras

Ideas para profundizar el ejercicio.

Ejemplo:

- Simular ARP spoofing en laboratorio controlado
- Analizar comportamiento en redes más grandes
- Capturar tráfico durante un escaneo de puertos
