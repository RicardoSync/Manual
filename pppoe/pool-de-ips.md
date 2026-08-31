---
description: Administra rangos de direcciones IP y supervisa su capacidad.
---

# Pool de Ips

### ¿Qué es un pool de IPs?

Un **pool de IPs** es un rango de direcciones disponible para asignar a clientes. Por ejemplo, desde `192.168.10.2` hasta `192.168.10.254`.

Esta vista administra los rangos de cada router. También muestra su capacidad para evitar que se agoten las direcciones disponibles.

<figure><img src="../.gitbook/assets/image (144).png" alt="Vista de administración de pools de IPs"><figcaption><p>Vista de administración de pools de IPs.</p></figcaption></figure>

### Crear un pool manual

Selecciona **Crear Nuevo Pool Manual**, identificado con el botón azul. Asigna un nombre y define el rango de direcciones IP.

<figure><img src="../.gitbook/assets/image (145).png" alt=""><figcaption></figcaption></figure>

Al guardar, el sistema crea el pool en el router MikroTik asociado.

<figure><img src="../.gitbook/assets/image (146).png" alt=""><figcaption></figcaption></figure>

### Importar pools desde MikroTik

Selecciona **Importar Pools desde MikroTik**, identificado con el botón verde. El sistema consulta los pools ya configurados en el router.

Selecciona los rangos que deseas guardar en la plataforma. Esta opción evita registrar manualmente una configuración existente.

<figure><img src="../.gitbook/assets/image (147).png" alt=""><figcaption></figcaption></figure>

### Supervisar la capacidad

La columna **Capacidad & Uso** muestra el porcentaje de direcciones ocupadas en cada rango.

El indicador cambia de color según el uso:

* **Verde:** capacidad disponible.
* **Amarillo:** uso elevado.
* **Rojo:** más del 90 % del rango está ocupado.

Amplía el rango o crea un pool antes de que se agoten las direcciones IP.

<figure><img src="../.gitbook/assets/image (148).png" alt=""><figcaption></figcaption></figure>

### Editar o eliminar un pool

Selecciona **Editar**, identificado con el botón amarillo, para actualizar el nombre o los rangos. Úsalo cuando necesites ampliar un bloque existente.

Selecciona **Eliminar**, identificado con el botón rojo, para borrar el pool. Esta acción también lo elimina del router MikroTik y conserva la configuración sincronizada.

<figure><img src="../.gitbook/assets/image (149).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
Elimina un pool solo después de confirmar que ningún cliente use direcciones de ese rango.
{% endhint %}
