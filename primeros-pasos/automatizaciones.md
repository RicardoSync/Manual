# Automatizaciones

Las automatizaciones ejecutan tareas recurrentes y reducen el trabajo manual.

Para acceder, vaya a **Ajustes del sistema → Automatizaciones**.

<figure><img src="../.gitbook/assets/image (9).png" alt=""><figcaption></figcaption></figure>

### Aviso de suspensión

<figure><img src="../.gitbook/assets/image (11).png" alt=""><figcaption></figcaption></figure>

Esta automatización envía un mensaje de WhatsApp cuando se suspende un servicio. La suspensión puede ocurrir por fecha de pago o factura vencida.

El mensaje se define mediante una plantilla.

<figure><img src="../.gitbook/assets/image (10).png" alt=""><figcaption></figcaption></figure>

Para usar esta función, conecte una sesión de WhatsApp y active el aviso.

### Recordatorio previo

<figure><img src="../.gitbook/assets/image (12).png" alt=""><figcaption></figcaption></figure>

Esta automatización notifica al cliente antes de su día de corte. Configure uno, dos o los días de anticipación que necesite.

El sistema envía el mensaje definido en la plantilla. También puede adjuntar un PDF con el importe estimado a pagar.

Este PDF es un recibo informativo. No es una factura generada.

![](<../.gitbook/assets/image (14).png>)

Active la opción 6 para incluir el PDF informativo.

<figure><img src="../.gitbook/assets/image (15).png" alt=""><figcaption></figcaption></figure>

En la parte inferior, defina los días de anticipación y la hora de envío.

| Cliente   | Día de corte | Días de anticipación |
| --------- | ------------ | -------------------- |
| Fabiola M | 15           | 1                    |

En este ejemplo, Fabiola recibe el recordatorio el día 14 de cada mes.

### Historial de consumo

<figure><img src="../.gitbook/assets/image (16).png" alt=""><figcaption></figcaption></figure>

Esta función recopila el tráfico de los clientes cada cinco minutos. Incluye clientes de `Simple Queue` y conexiones `PPPoE Active` de MikroTik.

{% hint style="warning" %}
El nombre del cliente debe coincidir en ambos sistemas. Debe coincidir con `Simple Queue` o con el usuario PPPoE en MikroTik.
{% endhint %}

<figure><img src="../.gitbook/assets/image (18).png" alt=""><figcaption></figcaption></figure>

Consulte el historial de cada cliente desde su perfil. Use los filtros para encontrar períodos específicos.

### Envío de cortes de caja

<figure><img src="../.gitbook/assets/image (19).png" alt=""><figcaption></figcaption></figure>

Esta función envía los cortes de caja por correo electrónico. Requiere un servidor SMTP y una dirección de correo empresarial configurados.

### Cola de mensajes

<figure><img src="../.gitbook/assets/image (20).png" alt=""><figcaption></figcaption></figure>

La cola define el intervalo entre los mensajes de WhatsApp. Recomendamos usar un intervalo de 5 a 40 segundos.

Un intervalo mayor reduce el riesgo de restricciones en la cuenta por envíos frecuentes.
