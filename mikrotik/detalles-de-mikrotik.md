---
description: Supervisa la salud, el tráfico y las interfaces de cada router.
---

# Detalles de MikroTik

### ¿Qué muestra esta vista?

Abre esta vista desde **Ver detalles**, identificado con el icono azul de microchip. Disponible en cada router de la lista principal.

Supervisa la salud del equipo, el tráfico total y sus interfaces. No necesitas abrir Winbox para consultar esta información.

<figure><img src="../.gitbook/assets/image (131).png" alt="Vista de detalles y monitoreo de un router MikroTik"><figcaption><p>Vista de detalles y monitoreo de un router MikroTik.</p></figcaption></figure>

### Reiniciar el router

Selecciona **Reiniciar Router** en la esquina superior derecha. El sistema envía un comando remoto para reiniciar el equipo.

Úsalo cuando el router no responda correctamente o requiera un reinicio operativo.

<figure><img src="../.gitbook/assets/image (132).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
El reinicio interrumpe temporalmente el servicio de todos los clientes conectados al router.
{% endhint %}

### Consultar la salud del equipo

Las tarjetas de estado muestran los sensores y datos principales del router:

* **Carga de CPU:** uso actual del procesador. Un valor cercano al 100 % puede afectar el rendimiento.
* **Memoria RAM y almacenamiento:** capacidad disponible en el equipo.
* **RouterOS y uptime:** versión instalada y tiempo desde el último reinicio.
*

    <figure><img src="../.gitbook/assets/image (133).png" alt=""><figcaption></figcaption></figure>

### Analizar el tráfico total

Consulta el consumo agregado de entrada y salida del router. Ajusta el filtro para revisar desde la última hora hasta la última semana.

El resumen incluye:

* Velocidad máxima, promedio, descarga y subida.
* Volumen total transferido durante el periodo seleccionado.
* Horas de mayor y menor consumo, junto con la gráfica histórica.

<figure><img src="../.gitbook/assets/image (134).png" alt=""><figcaption></figcaption></figure>

### Consultar las interfaces de red

El catálogo de interfaces muestra los puertos configurados. Incluye interfaces `ether`, bridges y VLAN.

Cada registro indica si la interfaz está activa. También muestra datos técnicos como la dirección MAC y el estado del enlace.

<figure><img src="../.gitbook/assets/image (135).png" alt=""><figcaption></figcaption></figure>

### Monitorear una interfaz en tiempo real

Selecciona **Monitorear** junto a la interfaz requerida. Se abre una ventana que actualiza las métricas cada segundo.

Consulta el tráfico de recepción (**RX**) y transmisión (**TX**) del puerto. La gráfica animada permite identificar el consumo actual de cada enlace.

<figure><img src="../.gitbook/assets/image (136).png" alt=""><figcaption></figcaption></figure>
