---
description: Crea, importa y administra perfiles PPPoE y sus límites de velocidad.
---

# Paquetes PPPoE (Profiles)

Los paquetes PPPoE se usan en redes que autentican clientes mediante usuario y contraseña.

MikroTik guarda estos paquetes en **PPP → Profiles**. Desde esta vista puedes administrarlos sin configurar cada perfil manualmente.

<figure><img src="../.gitbook/assets/image (155).png" alt=""><figcaption></figcaption></figure>

### Crear un perfil PPPoE

1. Selecciona **Nuevo paquete de Internet**.
2. Marca la casilla **Es PPPoE Profile**.
3. Define el nombre del plan y el precio mensual.
4. Configura el límite de velocidad y las direcciones IP.
5. Guarda el paquete.

Al marcar la opción PPPoE, verás campos exclusivos para este tipo de perfil.

<figure><img src="../.gitbook/assets/image (156).png" alt=""><figcaption></figcaption></figure>

#### Rate Limit

**Rate Limit** define la regla de velocidad con la sintaxis de MikroTik.

Por ejemplo, usa `5M/5M` para limitar la subida y bajada a 5 Mbps.

#### Asignación automática de IP

Vincula el perfil a un pool de direcciones IP mediante **Local Address** y **Remote Address**.

Cuando un cliente se autentica con este paquete, MikroTik asigna automáticamente una dirección IP desde ese pool.

### Importar perfiles desde MikroTik

Usa **Importar paquetes desde MikroTik** para incorporar perfiles existentes.

El sistema analiza el router y muestra los perfiles PPPoE detectados. Selecciona los perfiles que deseas importar y asigna un precio mensual para cobrarlos desde la plataforma.

<figure><img src="../.gitbook/assets/image (157).png" alt=""><figcaption></figcaption></figure>

### Editar un perfil

Selecciona el botón amarillo con el ícono de lápiz. Puedes actualizar el precio, el límite de velocidad y los pools de IP.

Al guardar, el sistema actualiza el perfil en MikroTik. Los clientes aplicarán los cambios al reiniciar o reconectar su router.

### Eliminar un perfil

Selecciona el botón rojo con el ícono de papelera. El sistema elimina el paquete y el perfil de **PPP → Profiles** en MikroTik.

{% hint style="warning" %}
No puedes eliminar un perfil asignado a clientes activos. Reasigna o desactiva esos clientes antes de eliminarlo.
{% endhint %}
