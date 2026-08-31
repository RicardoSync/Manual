---
description: Consulta y administra las sesiones PPPoE activas por router.
---

# PPPoE Active

### ¿Qué son las sesiones PPPoE activas?

Esta vista muestra los clientes conectados actualmente mediante PPPoE.

Consulta si un cliente está en línea, la IP asignada y el tiempo continuo de conexión.

<figure><img src="../.gitbook/assets/image (142).png" alt="Vista de sesiones PPPoE activas"><figcaption><p>Vista de sesiones PPPoE activas.</p></figcaption></figure>

### Consultar clientes por router

Selecciona el equipo desde **Seleccionar Router MikroTik**. El sistema consulta el router y carga sus sesiones activas en la tabla.

Cada consulta muestra solo los clientes conectados en ese momento.

### Revisar los datos de una sesión

La tabla muestra información clave para cada cliente en línea:

* **Usuario PPPoE:** credencial usada para iniciar la sesión.
* **MAC / Caller ID:** dirección física del equipo que estableció la conexión.
* **Dirección IP asignada:** IP entregada por el MikroTik.
* **Uptime:** tiempo que lleva conectada la sesión.

### Desconectar una sesión

Selecciona el botón rojo de **Acción** junto al cliente. El sistema solicita al MikroTik que cierre la sesión inmediatamente.

El cliente puede conectarse de nuevo de forma automática. Usa esta acción para renovar su IP, aplicar cambios de velocidad o resolver problemas de conexión.

<figure><img src="../.gitbook/assets/image (143).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
Desconectar una sesión interrumpe temporalmente el servicio del cliente.
{% endhint %}

