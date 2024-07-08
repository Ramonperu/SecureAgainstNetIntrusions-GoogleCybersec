# SecureAgainstNetIntrusions

Las redes están constantemente en riesgo de ser atacadas por hackers maliciosos vamos a ver una introducción de los ataques mas comunes así como la forma de identificarlos mitigarlos y protegernos. 

**Impactos de los ataques de red:**

- **Financieros:** Tiempo de inactividad del sistema, costos de recuperación de datos, posibles demandas y pérdida de ingresos.
- **Reputación:** Pérdida de confianza del cliente y posible daño a la imagen de marca.
- **Seguridad pública:** Daño potencial a los ciudadanos si se compromete la infraestructura crítica.

------

**Ataques de interceptación de red:**

Implican interceptar el tráfico de red para robar información o interrumpir la transmisión. Se pueden lograr a través de herramientas de hardware o software para "olfatear paquetes". Los atacantes pueden modificar los datos interceptados para causar daños, por ejemplo, cambiando los detalles de la transferencia bancaria. Los módulos posteriores profundizarán en el rastreo de paquetes maliciosos y otros tipos de interceptación.

**Ataques de puerta trasera:**

Explotan las debilidades intencionales dejadas por los programadores o administradores para eludir los controles de acceso. Destinados a la resolución de problemas o tareas administrativas, pero pueden ser utilizados por los atacantes. Una vez dentro, los atacantes pueden instalar malware, lanzar ataques DoS, robar datos o cambiar la configuración de seguridad. Pueden ser difíciles de detectar y eliminar, causando daños significativos.

## DOS o Ataque de Denegación de Servicio

-  **DoS:** Inunda una red o servidor con tráfico, haciéndolo inaccesible para los usuarios legítimos.
- **DDoS:**  Utiliza múltiples dispositivos para abrumar al objetivo con tráfico.

- **Ataques DoS a nivel de red:** Se dirigen al ancho de banda de la red para ralentizar el tráfico.

Ataques DoS comunes a nivel de red:

- **Ataque de inundación SYN:** Explota el proceso de enlace TCP enviando solicitudes SYN excesivas, sobrecargando el servidor.
- **Ataque de inundación ICMP:** Envía paquetes ICMP excesivos, consumiendo ancho de banda y provocando que el servidor se bloquee.
- **Ataque Ping of Death o ping de la meurte:** Envía paquetes ICMP de gran tamaño(>64kb), bloqueando el servidor.

------

## **Network Protocol Analyzer o Analizadores de protocolos de red **

Caracteristicas

- Se utilizan para capturar y analizar el tráfico de red.
- Para solucionar problemas de red e identificar amenazas de seguridad.

Tipos:

- SolarWinds NetFlow Traffic Analyzer.
-  ManageEngine OpManager.
- Azure Network Watcher.
- Wireshark.
- tcpdump.

Uso común:

- Establecer una línea de base para los patrones de tráfico de red y las métricas de utilización.
- Detectar e identificar el tráfico malicioso.
- Crear alertas personalizadas para problemas de red o amenazas de seguridad.
- Localizar el tráfico de mensajería instantánea no autorizado o los puntos de acceso inalámbricos.

### **TCPDUMP**

Características

- Tcpdump es un analizador de protocolos de red de línea de comandos.
- Popular, ligero y utiliza la biblioteca de código abierto libpcap.
- Compatible con Linux/Unix y macOS®.
- Proporciona un breve análisis de paquetes y convierte la información clave sobre el tráfico de red en formatos legibles por humanos.
- Muestra las direcciones IP de origen y destino, los números de puerto y otra información relevante.

Salida de un tcpdump:

<img align="center" src="/img/1ºimagenn.PNG"  />

Podemos observar la información de la transmision del paquete, desde la hora en que se realizo, ip y puerto de origen y ip y puerto de destino