---
description: Crea y administra planes con límites de velocidad para clientes con IP fija.
---

# Paquetes estáticos (Simple Queue)

<figure><img src="../.gitbook/assets/image (150).png" alt="Vista de paquetes de Internet"><figcaption><p>Vista de paquetes de Internet</p></figcaption></figure>

Esta vista es el catálogo de velocidades y precios de tu servicio.

Crea aquí los planes de Internet para tus clientes. Al crear o actualizar un plan, el sistema programa automáticamente las reglas de velocidad en tu MikroTik.

El sistema admite paquetes estáticos mediante **Simple Queue** y perfiles **PPPoE**. Esta guía cubre los paquetes estáticos.

### Paquetes estáticos

Usa paquetes estáticos para clientes con una dirección IP fija. MikroTik crea las reglas limitadoras en **Simple Queues**.

### Crear un paquete

<figure><img src="../.gitbook/assets/image (151).png" alt=""><figcaption></figcaption></figure>

1. Selecciona **Nuevo paquete de Internet**.
2. Deja desmarcada la opción **PPPoE**.
3. Define el **nombre del plan** y el **precio mensual**.
4. Indica la velocidad base de subida y bajada.
5. Configura una ráfaga, si aplica.
6. Guarda el paquete.

#### Velocidad base

La velocidad base define los límites contratados de **upload** y **download**.

Por ejemplo, un plan de 5 Mbps puede tener 5 Mbps de subida y 5 Mbps de bajada.

<figure><img src="../.gitbook/assets/image (152).png" alt=""><figcaption></figcaption></figure>

#### Ráfagas de velocidad

Las ráfagas son opcionales. Aumentan la velocidad durante un periodo corto al iniciar la navegación.

Por ejemplo, puedes ofrecer 15 Mbps durante 10 segundos a un plan de 5 Mbps. Después, la velocidad vuelve al límite contratado. Esto mejora la carga inicial de videos y servicios de streaming.

<figure><img src="../.gitbook/assets/image (153).png" alt=""><figcaption></figcaption></figure>

### Editar un paquete

Selecciona el botón amarillo con el ícono de lápiz. Puedes cambiar el precio, la velocidad base y las ráfagas.

Al guardar, el sistema actualiza en MikroTik todos los clientes asignados al paquete. No necesitas modificarlos uno por uno.

<figure><img src="../.gitbook/assets/image (154).png" alt=""><figcaption></figcaption></figure>

### Eliminar un paquete

Selecciona el botón rojo con el ícono de papelera. El sistema elimina el paquete y su regla de **Simple Queue** en MikroTik.

{% hint style="warning" %}
No puedes eliminar un paquete asignado a clientes activos. Reasigna o desactiva esos clientes antes de eliminarlo.
{% endhint %}
