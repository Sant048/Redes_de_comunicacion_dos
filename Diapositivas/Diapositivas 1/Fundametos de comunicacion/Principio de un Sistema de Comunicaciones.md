#  Sistemas de Comunicación e Información

> [!ABSTRACT] Objetivo Común
> Reunir, procesar y distribuir la información de la manera más rápida y eficiente posible, optimizando el uso de la infraestructura de comunicaciones disponible.

---

##  Fundamentos y Tipologías

### Fases de Desarrollo
El desarrollo de cualquier sistema es un proceso integral dividido en:
1. **Análisis:** Identificación de necesidades y condiciones del entorno.
2. **Diseño:** Arquitectura lógica y física de la solución.
3. **Construcción:** Implementación técnica de los mecanismos de transmisión.

### Clasificación de Sistemas
- **Sistema de Comunicación General:** Mecanismo base para enviar/recibir información de una **fuente** a un **destinatario**.
- **Sistema de Comunicaciones en Red:** Conjunto de **dispositivos y protocolos** para el intercambio de información entre computadoras o terminales.

> [!IMPORTANT] Dualidad Infraestructural
> Toda comunicación en red depende de la interacción entre:
> - **Hardware:** Equipos físicos (Routers, switches, cables, tarjetas).
> - **Software:** Programas y protocolos que gestionan el flujo de datos.

---

##  Elementos del Proceso Comunicativo

| Elemento     | Definición Técnica                                   | Ejemplos / Detalles         |
| :----------- | :--------------------------------------------------- | :-------------------------- |
| **Emisor**   | Procesa la señal de la fuente y la adecua al canal.  | Persona, empresa, software. |
| **Código**   | Sistema de signos o protocolos de construcción.      | Idiomas, Binario, TCP/IP.   |
| **Mensaje**  | La información bruta o paquetes de datos.            | Voz, texto, video.          |
| **Canal**    | Medio eléctrico/físico que cubre la distancia.       | Aire, Fibra, Cable, WiFi.   |
| **Receptor** | Decodifica, demodula y elimina el ruido de la señal. | Usuario, servidor, nodo.    |

###  Contexto e Infraestructura
El proceso no es lineal; está condicionado por la **Situación, Intención y Estructura**.

![[Pasted image 20260217233600.png]]

#### Clasificación de Medios
- **Medios Guiados (Hardware):** Cable de cobre, Fibra óptica.
- **Medios No Guiados:** Ondas de radio (Aire), Microondas.
- **Capa Logística (Software):** Protocolos de mensajería, Clientes de Email.

---

## Procesamiento de Señales

###  Análisis del Modelo de Comunicación
Este diagrama detalla los tres componentes esenciales que operan entre la **Fuente** y el **Destino**:

> [!NOTE] Flujo de Señal
> 1. **Transmisor:** Adecuación de la señal de la fuente al medio.
> 2. **Canal:** Puente eléctrico/físico sujeto a ruido y atenuación.
> 3. **Receptor:** Filtrado, decodificación y reconstrucción de la información.

![[Pasted image 20260217235050.png]]

Las señales de **voz, video, audio y datos** son originalmente analógicas. Para ser transmitidas digitalmente, requieren un proceso de conversión:

> [!NOTE] Proceso de Conversión A/D
> 1. **Muestreo**
> 2. **Cuantificación**
> 3. **Codificación**
> 

## Evolución Histórica de los Sistemas

### 1. Inicios (Finales del Siglo XIX)
La comunicación comenzó con sistemas análogos fundamentales.

| Tecnología               | Conceptos Clave                                 |
| :----------------------- | :---------------------------------------------- |
| **Comunicación Análoga** | Radio, Telefonía convencional, TV, Antenas.     |
| **Espectro**             | **BB** (Banda Base) y **RF** (Radiofrecuencia). |
## Arquitectura de Transmisión

### Modelo General

> [!INFO] Definición
> El sistema actúa como un puente entre la **Fuente** y el **Destino**, transformando la información en señales aptas para el **Canal**.

![[Pasted image 20260217235137.png]]

### Sistema Analógico y RF
Para transmisiones de largo alcance, se requiere el uso de frecuencias portadoras:

| Concepto                 | Función                                                   |
| :----------------------- | :-------------------------------------------------------- |
| **BB (Banda Base)**      | Señal original de baja frecuencia.                        |
| **RF (Radiofrecuencia)** | Señal de alta frecuencia apta para el canal analógico.    |
| **Portadora**            | Onda auxiliar que "carga" la información en el modulador. |

![[Pasted image 20260217235137.png]]

> [!WARNING] Vulnerabilidad
> En el **Canal Analógico**, factores externos como la lluvia o la distancia degradan la señal RF, haciendo que el rol del **Receptor** (filtrado y demodulación) sea fundamental para la integridad de los datos.
### 2. Transición y Era Digital
Evolución hacia la transmisión de señales digitales sobre canales digitales.

| Etapa                       | Servicios                                                          |
| :-------------------------- | :----------------------------------------------------------------- |
| **Digitalización Base**     | Radio digital, Telefonía digital, Difusión de TV.                  |
| **Comunicación IP Moderna** | Móvil IP, Telefonía IP, IPTV, Streaming, Gaming, Videoconferencia. |
##  Transmisión Digital sobre Canal Digital

> [!INFO] Concepto Clave
> En la transmisión digital, la prioridad es la **reconstrucción exacta** de los datos. El uso de **Regeneradores** permite mantener la integridad de la señal a largas distancias eliminando el ruido.

![[Pasted image 20260217235201.png]]
### Bloques Técnicos

| Componente | Función Principal |
| :--- | :--- |
| **Codificador de Línea** | Transforma bits en niveles de tensión o pulsos de luz. |
| **Regenerador** | Re-muestrea y reconstruye la señal digital para eliminar el ruido. |
| **Canal Digital** | Soporte físico optimizado para el transporte de señales discretas. |
| **Decodificador** | Convierte los pulsos recibidos de vuelta a formato binario (0/1). |
### Servicios Modernos (Era Digital)
Esta arquitectura permite el despliegue de servicios de alta demanda que mencionamos anteriormente:
- **Voz sobre IP (VoIP)** y Telefonía IP.
- **Streaming** de video y IPTV.
- **Gaming** online y Videoconferencias en tiempo real.

