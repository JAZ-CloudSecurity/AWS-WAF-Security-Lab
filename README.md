# AWS WAF Security Lab: Protección de Infraestructura Web

Este repositorio contiene la documentación y evidencia técnica de la implementación de un **Web Application Firewall (WAF)** en AWS para la protección de un **Application Load Balancer (ALB)**. 

El proyecto fue desarrollado como parte del Diplomado de Arquitectura y Seguridad Cloud (USACH), enfocándose en la mitigación de vulnerabilidades web y la gestión de tráfico malicioso.

## 🎯 Objetivos del Proyecto
* Configurar y desplegar una **Web ACL** (Access Control List).
* Implementar reglas de seguridad para el control de tráfico entrante.
* Asociar el WAF con un balanceador de carga de aplicación (ALB) existente.
* Validar el filtrado de peticiones mediante el monitoreo de tráfico.

## 🛠️ Tecnologías Utilizadas
* **Servicios de AWS:** WAF, Application Load Balancer (ALB), CloudShell.
* **Inteligencia Artificial:** Amazon Q (para diagnóstico y troubleshooting).
* **Seguridad:** Definición de reglas (Managed Rule Groups) para protección contra ataques comunes.

## 🛡️ Implementación Técnica
Se configuró una Web ACL con reglas específicas para analizar las cabeceras de las peticiones HTTP/S. El enfoque principal fue garantizar que solo el tráfico legítimo alcanzara las instancias de backend detrás del balanceador.

### Desafío Técnico y Resolución (Troubleshooting)
Durante el laboratorio, identifiqué una discrepancia en los identificadores (IDs) del balanceador de carga que impedía la asociación correcta con el WAF.

* **Problema:** El ID del balanceador no coincidía con los registros esperados en la consola.
* **Solución:** Utilicé **Amazon Q** para obtener sugerencias de comandos de diagnóstico y ejecuté consultas a través de **AWS CloudShell** para identificar el ARN (Amazon Resource Name) correcto. 
* **Resultado:** Se logró la asociación exitosa del WAF tras rectificar los parámetros mediante CLI, demostrando capacidad de respuesta ante errores en entornos productivos.

## 📸 Evidencia del Laboratorio
*(Aquí insertaremos las imágenes que tienes en tu Word para demostrar el paso a paso)*

---
