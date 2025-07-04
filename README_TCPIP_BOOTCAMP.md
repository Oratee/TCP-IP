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

🌐 TCP/IP: La Autopista Digital en Dos Voces
📦 Las 4 Capas del Modelo TCP/IP
🚀 Capa de Aplicación (HTTP, HTTPS, DNS)
📋 Técnico: Proporciona servicios de red directamente a aplicaciones del usuario final.
🎈 Conversacional: Es donde vives tu día a día - Instagram, WhatsApp, Google, etc.
🚛 Capa de Transporte (TCP vs UDP)
📋 Técnico: Gestiona comunicación extremo a extremo; TCP garantiza entrega, UDP prioriza velocidad.
🎈 Conversacional: TCP es correo certificado (lento pero seguro), UDP es gritar al vecino (rápido pero no garantizado).
🗺️ Capa de Internet (IP, Routing)
📋 Técnico: Maneja direccionamiento lógico y enrutamiento de paquetes a través de múltiples redes.
🎈 Conversacional: Es el GPS de Internet que encuentra la mejor ruta para tu mensaje.
🔌 Capa de Acceso a Red (Ethernet, Wi-Fi)
📋 Técnico: Define especificaciones físicas para transmisión en medios como Ethernet o Wi-Fi.
🎈 Conversacional: Los cables y ondas radio - Ethernet es tu auto propio, Wi-Fi es como Uber.
🌍 Direccionamiento IP: IPv4 vs IPv6
🏠 ¿Qué es una dirección IP?
📋 Técnico: Identificador numérico único asignado a cada dispositivo en una red IP.
🎈 Conversacional: La dirección postal de tu dispositivo en Internet.
🏗️ IPv4 vs IPv6
📋 Técnico: IPv4 usa 32 bits (4.3 mil millones direcciones), IPv6 usa 128 bits (340 sextillones).
🎈 Conversacional: IPv4 son números de teléfono de 4 partes que se están agotando, IPv6 son direcciones súper largas que nunca se acabarán.
🏠 IP Pública vs Privada
📋 Técnico: IP pública es enrutable globalmente, IP privada es para redes locales.
🎈 Conversacional: IP pública es tu dirección de casa, IP privada son los cuartos dentro de tu casa.

Internet = oficina postal de 4 departamentos que hacen que tu meme llegue al otro lado del mundo 😄

## 🛠️ Protocolos Clave en el Día a Día Web

### HTTP/HTTPS
- **HTTP (HyperText Transfer Protocol):**  
  Protocolo que permite la comunicación entre navegadores y servidores web. No es seguro, los datos viajan sin cifrar.
- **HTTPS (HyperText Transfer Protocol Secure):**  
  Es la versión segura de HTTP, cifra los datos para proteger la información que viaja entre el navegador y el servidor.

---

### DNS (Domain Name System)
- Es el sistema que traduce nombres de dominio (como `google.com`) en direcciones IP.
- Permite que los navegadores encuentren la ubicación real de los sitios web en Internet.

---

### DHCP (Dynamic Host Configuration Protocol)
- Protocolo que asigna automáticamente direcciones IP a los dispositivos cuando se conectan a una red.
- Evita que tengamos que configurar la IP de forma manual.

---

### TCP vs UDP

| Característica              | TCP                             | UDP                             |
|-----------------------------|---------------------------------|---------------------------------|
| Fiabilidad                  | Alta (asegura entrega ordenada)  | Baja (pueden perderse datos)    |
| Velocidad                   | Más lento                       | Más rápido                      |
| Uso típico                  | Navegación web, descarga de archivos | Streaming, videollamadas, juegos |
| Control de errores          | Sí                              | No                              |

- **Ejemplo de TCP:** Cargar una página web, descargar un archivo.
- **Ejemplo de UDP:** Streaming de video, videollamadas, juegos en línea.


## 🛠️ Protocolos Clave en el Día a Día Web - Resumen Simple

### HTTP/HTTPS
- **HTTP (HyperText Transfer Protocol):**  
  Protocolo que permite la comunicación entre navegadores y servidores web. No es seguro.
- **HTTPS (HyperText Transfer Protocol Secure):**  
  Igual que HTTP, pero con seguridad y cifrado de datos.

---

### DNS (Domain Name System)
- Es como la "agenda" de Internet.
- Traduce nombres web (como `google.com`) en direcciones IP que los navegadores pueden entender y localizar.

---

### DHCP (Dynamic Host Configuration Protocol)
- Asigna automáticamente direcciones IP a los dispositivos en una red.
- Permite que los equipos se conecten sin configurar manualmente la IP.

---

### TCP vs UDP

| Característica              | TCP                            | UDP                             |
|-----------------------------|--------------------------------|---------------------------------|
| Fiabilidad                  | Alta (asegura entrega ordenada) | Baja (pueden perderse datos)    |
| Velocidad                   | Más lento                      | Más rápido                      |
| Uso típico                  | Navegación web, descarga de archivos | Streaming, videollamadas, juegos |
| Control de errores          | Sí                             | No                              |

- **TCP Ejemplo:** Abrir una página web, descargar un archivo.
- **UDP Ejemplo:** Streaming de video, videollamadas, juegos en línea.

---


# 🧭 Proceso básico de conexión en la web

## De tu navegador a un servidor web: ¿qué ocurre paso a paso?

Cuando escribes una URL en tu navegador y presionas Enter, se inicia una secuencia de eventos que permite que tu dispositivo se conecte con un servidor web en cualquier parte del mundo. Este proceso, aunque parece instantáneo, involucra varios pasos técnicos precisos.

### 1. **Análisis de la URL**
El navegador descompone la URL en sus componentes:
- **Protocolo**: `http://` o `https://`
- **Dominio**: `ejemplo.com`
- **Puerto**: (por defecto 80 para HTTP, 443 para HTTPS)
- **Ruta**: `/pagina/index.html`

### 2. **Verificación de caché**
El navegador revisa si ya tiene una copia reciente de la página solicitada en su caché local. Si la encuentra y está vigente, puede mostrarla directamente sin necesidad de contactar al servidor.

### 3. **Resolución DNS**
Si necesita contactar al servidor, el navegador debe convertir el nombre de dominio legible (como `google.com`) en una dirección IP numérica que las computadoras puedan entender.

### 4. **Establecimiento de conexión TCP**
Una vez que tiene la dirección IP, el navegador establece una conexión confiable con el servidor usando el protocolo TCP.

### 5. **Intercambio de seguridad (si es HTTPS)**
Si la conexión es segura, se establece un canal cifrado entre el navegador y el servidor.

### 6. **Envío de la petición HTTP**
El navegador envía una petición HTTP al servidor, especificando qué recurso necesita.

### 7. **Procesamiento y respuesta del servidor**
El servidor procesa la petición y envía de vuelta el contenido solicitado junto con metadatos sobre la respuesta.

### 8. **Renderizado de la página**
El navegador recibe el contenido y lo convierte en la página web visual que ves en tu pantalla.

## Resolución DNS

El **Sistema de Nombres de Dominio (DNS)** funciona como la "guía telefónica" de internet. Cuando escribes `google.com`, tu computadora no sabe automáticamente dónde encontrar ese sitio web.

### ¿Cómo funciona la resolución DNS?

1. **Consulta local**: Tu dispositivo primero revisa su caché DNS local para ver si ya conoce la dirección IP de ese dominio.

2. **Consulta al resolver DNS**: Si no la encuentra localmente, contacta al servidor DNS configurado en tu red (generalmente proporcionado por tu proveedor de internet).

3. **Consulta recursiva**: Si tu resolver DNS tampoco conoce la dirección, inicia una búsqueda recursiva:
   - Consulta a los **servidores raíz** (.)
   - Estos redirigen a los servidores del **dominio de nivel superior** (.com, .org, etc.)
   - Finalmente llega a los **servidores autoritativos** del dominio específico

4. **Respuesta en cascada**: La dirección IP se devuelve siguiendo el mismo camino en reversa, y cada servidor guarda la información en su caché para futuras consultas.

### Ejemplo práctico:
```
Usuario escribe: www.ejemplo.com
DNS devuelve: 192.168.1.100
El navegador ahora sabe a qué servidor conectarse
```

## Establecimiento de conexión TCP (Handshake)

TCP (Transmission Control Protocol) es el protocolo que garantiza que los datos lleguen de manera confiable y ordenada entre tu navegador y el servidor web.

### El Three-Way Handshake

Antes de que cualquier dato web pueda transferirse, el navegador y el servidor deben establecer una conexión TCP mediante un proceso de tres pasos:

1. **SYN (Synchronize)**
   - El navegador envía un paquete SYN al servidor
   - Mensaje: "Hola, quiero establecer una conexión contigo"
   - Incluye un número de secuencia inicial

2. **SYN-ACK (Synchronize-Acknowledge)**
   - El servidor responde con un paquete SYN-ACK
   - Mensaje: "Recibido, yo también quiero conectarme contigo"
   - Confirma el número de secuencia del cliente y envía el suyo

3. **ACK (Acknowledge)**
   - El navegador envía un paquete ACK final
   - Mensaje: "Perfecto, conexión establecida"
   - Confirma que recibió la respuesta del servidor

### ¿Por qué es importante este proceso?

- **Confiabilidad**: Garantiza que ambos extremos estén listos para comunicarse
- **Sincronización**: Establece números de secuencia para ordenar los datos
- **Control de flujo**: Permite manejar la velocidad de transmisión
- **Detección de errores**: Identifica si hay problemas en la conexión

Una vez completado el handshake, la conexión TCP está lista para transferir datos HTTP de manera confiable.

---

# 🔐 Seguridad y capa de transporte

## Introducción rápida a SSL/TLS

**SSL (Secure Sockets Layer)** y su sucesor **TLS (Transport Layer Security)** son protocolos criptográficos que proporcionan seguridad en las comunicaciones a través de una red. Aunque SSL está técnicamente obsoleto, el término se sigue usando coloquialmente para referirse a TLS.

### ¿Qué problemas resuelve SSL/TLS?

1. **Confidencialidad**: Cifra los datos para que solo el destinatario pueda leerlos
2. **Integridad**: Garantiza que los datos no fueron modificados durante la transmisión
3. **Autenticación**: Verifica la identidad del servidor (y opcionalmente del cliente)

### ¿Cómo funciona el cifrado?

SSL/TLS utiliza una combinación de cifrado simétrico y asimétrico:

- **Cifrado asimétrico**: Usa un par de claves (pública y privada) para el intercambio inicial seguro
- **Cifrado simétrico**: Usa una clave compartida (más eficiente) para cifrar la comunicación posterior

### El handshake SSL/TLS

Cuando estableces una conexión HTTPS, ocurre un proceso adicional después del handshake TCP:

1. **Cliente Hello**: El navegador envía sus capacidades criptográficas
2. **Servidor Hello**: El servidor selecciona los algoritmos y envía su certificado
3. **Verificación del certificado**: El navegador verifica que el certificado sea válido
4. **Intercambio de claves**: Se establece una clave de sesión compartida
5. **Confirmación**: Ambos confirman que el canal seguro está establecido

## Qué cambia cuando usamos HTTPS

La diferencia entre HTTP y HTTPS va mucho más allá de simplemente agregar una "s" al final.

### Cambios técnicos fundamentales:

**Puerto por defecto**:
- HTTP: Puerto 80
- HTTPS: Puerto 443

**Proceso de conexión**:
- HTTP: Solo handshake TCP
- HTTPS: Handshake TCP + handshake SSL/TLS

**Datos en tránsito**:
- HTTP: Texto plano, completamente visible
- HTTPS: Cifrados, ilegibles para interceptores

### Beneficios de seguridad:

1. **Protección contra espionaje**: Nadie puede leer tus datos mientras viajan por la red
2. **Protección contra manipulación**: Los datos no pueden ser modificados sin detectarse
3. **Autenticación del servidor**: Te aseguras de que estás hablando con el servidor correcto
4. **Protección contra ataques man-in-the-middle**: Previene que alguien se interponga en tu comunicación

### Indicadores visuales en el navegador:

- **Candado verde/gris**: Conexión segura establecida
- **Advertencia**: Problemas con el certificado
- **"No seguro"**: Conexión HTTP sin cifrar

### Consideraciones de rendimiento:

**Costos adicionales**:
- Tiempo extra para el handshake SSL/TLS
- Procesamiento adicional para cifrar/descifrar datos
- Ligeramente más ancho de banda

**Beneficios compensatorios**:
- HTTP/2 (que requiere HTTPS) es más eficiente
- Mejor SEO (Google favorece sitios HTTPS)
- Confianza del usuario

En la práctica moderna, HTTPS se ha convertido en el estándar, y muchos navegadores ya marcan los sitios HTTP como "no seguros" por defecto.

9. **🧪 Herramientas básicas para ver el protocolo en acción**

   - `ping`, `tracert`/`traceroute`
   - `netstat`, `nslookup`, `curl`, `telnet`

10. **📝 Glosario esencial de términos**

- IP, DNS, Gateway, NAT, Subred, Paquete, etc.

---

Este material es parte de tu formación como desarrollador/a web. Entender TCP/IP te da una base sólida para comprender cómo funciona la web en sus niveles más fundamentales.
