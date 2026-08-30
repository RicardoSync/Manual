# Suspensión de cliente

<figure><img src="../.gitbook/assets/image (64).png" alt="Opciones para suspender el servicio de un cliente"><figcaption><p>Suspensión manual de un cliente</p></figcaption></figure>

Suspende manualmente el servicio de un cliente desde la lista o su perfil.

La suspensión se aplica de inmediato. Puedes realizarla desde:

1. La **Lista de clientes**.
2. El **Perfil del cliente**.

### Suspender desde la lista de clientes

<figure><img src="../.gitbook/assets/image (65).png" alt="Menú de acciones con la opción Suspender"><figcaption><p>Acción Suspender en la lista de clientes</p></figcaption></figure>

1. Busca al cliente en **Clientes**.
2. Abre el menú de acciones de su fila.
3. Selecciona el ícono amarillo de **pausa**.
4. Confirma la suspensión.

<figure><img src="../.gitbook/assets/image (67).png" alt="Ventana de confirmación para suspender un cliente"><figcaption><p>Confirma la suspensión</p></figcaption></figure>

Al confirmar, el sistema suspende el servicio inmediatamente.

{% hint style="warning" %}
Verifica los datos del cliente antes de confirmar. La suspensión afecta su conexión de inmediato.
{% endhint %}

### Suspensión confirmada

<figure><img src="../.gitbook/assets/image (68).png" alt="Mensaje de confirmación de suspensión exitosa"><figcaption><p>Servicio suspendido correctamente</p></figcaption></figure>

El sistema muestra un mensaje al completar la suspensión.

Para clientes con dirección IP, el sistema agrega la IP a la lista de direcciones `corte` de MikroTik.

{% hint style="warning" %}
Configura previamente las reglas de corte en cada MikroTik. Sin estas reglas, agregar la IP a `corte` no bloqueará el acceso.
{% endhint %}

<figure><img src="../.gitbook/assets/image (69).png" alt="Dirección IP del cliente incluida en la lista corte de MikroTik"><figcaption><p>IP agregada a la lista de corte</p></figcaption></figure>

<figure><img src="../.gitbook/assets/image (70).png" alt="Notificación enviada sobre la suspensión del servicio"><figcaption><p>Notificación de suspensión</p></figcaption></figure>

Si activaste el **Aviso de suspensión** y conectaste WhatsApp, el sistema notifica al cliente. Consulta [automatizaciones.md](../primeros-pasos/automatizaciones.md "mention") para configurarlo.

### Suspender desde el perfil del cliente

<figure><img src="../.gitbook/assets/image (71).png" alt="Opción Suspender en el perfil del cliente"><figcaption><p>Suspensión desde el perfil del cliente</p></figcaption></figure>

1. Abre el perfil del cliente.
2. Selecciona **Suspender**.
3. Confirma la acción.

El resultado es el mismo que desde la lista de clientes.
