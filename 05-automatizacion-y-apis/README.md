# Automatización de Redes y APIs (Limitaciones en Packet Tracer)

Esta carpeta documenta el alcance de los laboratorios de automatización previstos dentro del itinerario CCNA (**salidas JSON en IOS, RESTCONF, NETCONF y controladores tipo DNA Center**).

## ¿Por qué no hay archivos `.pkt` funcionales en este bloque?

Cisco Packet Tracer está diseñado principalmente para simular protocolos tradicionales de enrutamiento, conmutación y servicios de red, por lo que **no soporta de forma nativa** las capacidades necesarias para ejecutar prácticas reales de programabilidad y automatización moderna:

- **Formateo estructurado en CLI:** Comandos como `| json` o `| xml` (por ejemplo, `show ip interface brief | json`) no están implementados en el parser de IOS de Packet Tracer.
- **Protocolos basados en modelos de datos:** No dispone de agentes funcionales para **NETCONF** (sobre SSH/XML) ni **RESTCONF** (sobre HTTPS/JSON/YANG).
- **Controladores empresariales:** Las funciones de **Cisco DNA Center** (APIs norte/sur, aseguramiento y aprovisionamiento programático) requieren un entorno de controlador real o virtualizado.

## Alternativas para practicar estos laboratorios

Para ejecutar estas prácticas en un entorno funcional se emplean plataformas con imágenes reales o virtualizadas de IOS XE / NX-OS:

- **Cisco DevNet Sandbox** (entornos gratuitos de acceso remoto con dispositivos IOS XE y sandboxes de DNA Center).
- **Cisco Modeling Labs (CML)**, **EVE-NG** o **GNS3** con imágenes virtuales (CSR1000v / Catalyst 8000v) conectadas a scripts locales en **Python** (`requests`, `ncclient`, `netmiko`).