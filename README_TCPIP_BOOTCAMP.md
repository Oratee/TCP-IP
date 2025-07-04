# 🧠 Conceptos Básicos del Protocolo TCP/IP

Este documento forma parte del módulo introductorio de redes en el bootcamp de desarrollo web. Estos son los fundamentos esenciales del protocolo TCP/IP, necesario para entender cómo viajan los datos por Internet y cómo funcionan los servicios web.

---

## 📚 Tabla de Contenidos

1. # Protocolo TCP/IP: Fundamentos y Comparación con OSI

## 🌐 ¿Qué es el protocolo TCP/IP y por qué es importante?

### Breve historia y propósito

TCP/IP (Transmission Control Protocol/Internet Protocol) es una suite de protocolos desarrollada en los años 1970 para el proyecto ARPANET del Departamento de Defensa de Estados Unidos. Creado por Vint Cerf y Bob Kahn, su propósito era establecer un sistema de comunicación robusto que permitiera la interconexión de redes diferentes y garantizara la entrega confiable de datos incluso si partes de la red fallaran.

### Su rol en el funcionamiento de Internet

TCP/IP es el "idioma universal" de Internet. Define cómo los datos se dividen en paquetes, se envían a través de la red, y se reensamblan en el destino. Proporciona direccionamiento único para cada dispositivo (direcciones IP), determina las rutas óptimas para los datos, y controla errores y flujo de información. Sin TCP/IP, no existiría la comunicación global que conocemos hoy.

## 🏗️ Modelo TCP/IP vs Modelo OSI

### Comparación de capas

El modelo TCP/IP tiene 4 capas prácticas, mientras que el modelo OSI tiene 7 capas teóricas. TCP/IP combina las funciones de OSI de manera más simple: la capa de Aplicación de TCP/IP engloba las capas de Aplicación, Presentación y Sesión de OSI; la capa de Transporte es equivalente; la capa de Internet corresponde a la capa de Red de OSI; y la capa de Acceso a Red combina las capas Física y Enlace de datos.

### ¿Por qué usamos TCP/IP en la web?

TCP/IP se adoptó como estándar de Internet porque fue desarrollado antes que OSI y ya estaba funcionando cuando Internet comenzó a expandirse. Su simplicidad (menos capas), flexibilidad para diferentes tecnologías, y robustez probada en el crecimiento masivo de Internet lo convirtieron en la elección práctica. Mientras OSI quedó como marco teórico de referencia, TCP/IP se convirtió en la realidad operativa de las comunicaciones globales.

## 📋 Ejemplos Prácticos

### Ejemplo 1: Navegación web con HTTP
Cuando escribes "www.google.com" en tu navegador, TCP/IP actúa en todas sus capas: la capa de Aplicación usa HTTP para solicitar la página web, la capa de Transporte usa TCP para garantizar que todos los datos lleguen correctamente, la capa de Internet usa IP para encontrar la ruta hacia los servidores de Google, y la capa de Acceso a Red usa tu conexión WiFi o Ethernet para enviar físicamente los datos.

### Ejemplo 2: Envío de correo electrónico
Al enviar un email, tu cliente de correo usa SMTP (capa de Aplicación) para formatear el mensaje, TCP (capa de Transporte) divide el correo en paquetes y asegura su entrega completa, IP (capa de Internet) enruta cada paquete hacia el servidor de correo del destinatario posiblemente por diferentes caminos, y tu conexión a Internet (capa de Acceso a Red) transmite físicamente cada paquete hacia su destino.

3. **📦 Las 4 capas del modelo TCP/IP (de forma sencilla)**

   - Capa de Aplicación (HTTP, HTTPS, DNS, etc.)
   - Capa de Transporte (TCP vs UDP)
   - Capa de Internet (IP, direcciones IP, routing)
   - Capa de Acceso a Red (Ethernet, Wi-Fi)

4. **🌍 Direccionamiento IP: IPv4 vs IPv6**

   - Qué es una dirección IP
   - Estructura básica de una IP
   - Diferencia entre IP pública y privada

5. **📶 Puertos y Protocolos Comunes para Desarrolladores Web**

   - ¿Qué es un puerto?
   - Puertos típicos: 80 (HTTP), 443 (HTTPS), 22 (SSH), 3306 (MySQL)

6. **🛠️ Protocolos clave en el día a día web**

   - HTTP/HTTPS
   - DNS
   - DHCP
   - TCP vs UDP (con ejemplos como streaming vs navegación)

7. **🧭 Proceso básico de conexión en la web**

   - De tu navegador a un servidor web: ¿qué ocurre paso a paso?
   - Resolución DNS
   - Establecimiento de conexión TCP (Handshake)

8. **🔐 Seguridad y capa de transporte**

   - Introducción rápida a SSL/TLS
   - Qué cambia cuando usamos HTTPS

9. **🧪 Herramientas básicas para ver el protocolo en acción**

   - `ping`, `tracert`/`traceroute`
   - `netstat`, `nslookup`, `curl`, `telnet`

10. **📝 Glosario esencial de términos**

- IP, DNS, Gateway, NAT, Subred, Paquete, etc.

---

Este material es parte de tu formación como desarrollador/a web. Entender TCP/IP te da una base sólida para comprender cómo funciona la web en sus niveles más fundamentales.
