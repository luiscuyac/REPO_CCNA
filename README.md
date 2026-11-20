# Cisco Packet Tracer Labs

Colección de **33 laboratorios prácticos de redes** desarrollados en Cisco Packet Tracer para trabajar fundamentos de enrutamiento, conmutación, servicios de red, seguridad y nociones iniciales de automatización.

Cada laboratorio cuenta con su archivo de topología (`.pkt`) y notas o configuraciones de referencia.

## Estructura del repositorio

- **`01-routing-ipv4-ipv6/`**: Rutas estáticas, RIPv2, OSPF v2 (área única y multiárea), rutas estáticas IPv6, RIPng y OSPFv3 (área única y multiárea).
- **`02-switching-redundancia/`**: Direccionamiento IPv6 (SLAAC, DHCPv6), VLANs, trunking y VLAN nativa, Router on a Stick, STP básico, PortFast y BPDU Guard, EtherChannel (LACP) y redundancia con HSRP.
- **`03-servicios-y-nat/`**: DHCP en router y DHCP Relay, NAT estático, PAT y Pool, NAT avanzado con Dual ISP, NTP, Syslog y DNS básico.
- **`04-seguridad-acceso-wireless/`**: Gestión y acceso (consola, SSH/Telnet, copia/restauración, acceso seguro), ACLs estándar y extendidas, Port Security, DHCP Snooping + Dynamic ARP Inspection y wireless básico con AP autónomo.
- **`05-automatizacion-y-apis/`**: Salidas JSON en IOS y conceptos de RESTCONF, NETCONF y DNA Center.

## Nota de uso y limitaciones

- Este repositorio reúne prácticas de aprendizaje y repaso técnico; los escenarios y notas se revisan y amplían de forma progresiva a medida que avanzo en mi formación en redes y automatización.
- **Limitaciones de Packet Tracer:** Algunos laboratorios avanzados o de automatización (como ciertos comportamientos de protocolos/redundancia, opciones de consola o escenarios de JSON, RESTCONF, NETCONF y controladores) están limitados o simulados de forma parcial por las capacidades propias de Cisco Packet Tracer frente a hardware real o entornos de virtualización más completos.