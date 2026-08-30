# Activación de cliente

<figure><img src="../.gitbook/assets/image (72).png" alt="Opción para activar un cliente suspendido"><figcaption><p>Activación manual de un cliente</p></figcaption></figure>

Activa nuevamente el servicio de un cliente con estado **Suspendido**.

1. Ve a **Clientes** y localiza al cliente suspendido.
2. Abre el menú de acciones de su fila.
3. Selecciona el ícono verde de **Activar**.

<figure><img src="../.gitbook/assets/image (73).png" alt="Menú de acciones con la opción Activar"><figcaption><p>Acción Activar para un cliente suspendido</p></figcaption></figure>

4. Confirma la activación en la ventana de confirmación.

<figure><img src="../.gitbook/assets/image (74).png" alt="Ventana de confirmación para activar un cliente"><figcaption><p>Confirma la activación</p></figcaption></figure>

Al confirmar, el sistema reactiva el servicio del cliente.

### Activación confirmada

<figure><img src="../.gitbook/assets/image (75).png" alt="Mensaje de confirmación de activación exitosa"><figcaption><p>Servicio activado correctamente</p></figcaption></figure>

El sistema realiza estas acciones:

* Elimina la dirección IP del cliente de la lista `corte` en MikroTik.
* Habilita nuevamente el secreto PPPoE para clientes con este tipo de conexión.
* Envía una notificación por WhatsApp si el **Aviso de suspensión** está configurado.

{% hint style="info" %}
Configura las reglas de corte en MikroTik antes de suspender clientes con dirección IP.
{% endhint %}

Consulta [suspension-de-cliente.md](suspension-de-cliente.md "mention") para conocer el proceso inverso.
