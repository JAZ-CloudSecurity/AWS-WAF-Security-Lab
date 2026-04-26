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

### Configuración de Reglas en AWS WAF
<img width="1088" height="535" alt="image" src="https://github.com/user-attachments/assets/cb853fd2-4f2f-47a5-9f8f-0c103b9aade4" />

### Resolución de problemas con CloudShell y Amazon Q

<img width="1056" height="866" alt="image" src="https://github.com/user-attachments/assets/b1aa41c5-502f-4032-93bd-3ac5c2a571c1" />
<img width="1026" height="550" alt="image" src="https://github.com/user-attachments/assets/afed0de3-000f-4a87-a13e-77d5dfffe35f" />
<img width="1003" height="398" alt="image" src="https://github.com/user-attachments/assets/3a2812d2-f5bc-4a66-b636-34ce74a61202" />
<img width="973" height="521" alt="image" src="https://github.com/user-attachments/assets/592ac0c6-8de5-4a56-9d55-8b21eab3b1b8" />

### Asociación Final

<img width="804" height="1071" alt="image" src="https://github.com/user-attachments/assets/c78501f8-c3aa-4eb7-afee-b40fabc5215e" />
<img width="1088" height="479" alt="image" src="https://github.com/user-attachments/assets/29b6b42c-eb6c-4097-a32e-46a96497eb03" />
<img width="1088" height="500" alt="image" src="https://github.com/user-attachments/assets/8d78448a-0ece-41c1-a85a-ca8fd40fc648" />
<img width="1088" height="385" alt="image" src="https://github.com/user-attachments/assets/9c1883f0-04d1-4b95-94da-565c8497f6ea" />
<img width="1088" height="616" alt="image" src="https://github.com/user-attachments/assets/e9e43169-880a-429d-abad-311530539369" />




---
