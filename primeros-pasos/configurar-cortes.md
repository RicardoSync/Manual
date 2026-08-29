# Configurar cortes

<figure><img src="../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

En **Cortes automáticos**, definimos cuándo el sistema suspende servicios por falta de pago.

También definimos el horario de suspensión y los días de gracia.

### Configuración general

Los **días de gracia** son el plazo adicional para que un cliente realice su pago. Por ejemplo, si vence el día 15 y configuramos tres días, podrá pagar hasta el día 18.

El **horario de corte** define la hora en que el sistema revisa y suspende servicios con adeudos. Recomendamos usar un horario laboral. Así podrá atender consultas de los clientes.

### Cortes por fecha vencida

<figure><img src="../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>

Este método usa la fecha de próximo pago y los días de gracia configurados.

| Dato                  | Valor                |
| --------------------- | -------------------- |
| Cliente               | Denisse Saucedo      |
| Fecha de próximo pago | 15 de agosto de 2026 |
| Días de gracia        | 5 días               |
| Fecha límite de pago  | 20 de agosto de 2026 |

Si Denisse no paga el 15 de agosto, su estado cambia a **Adeudo**. Su servicio permanece activo durante los cinco días de gracia.

El período de gracia finaliza el 20 de agosto. Si el pago sigue pendiente, el sistema suspende el servicio en el horario configurado.

Este método es útil cuando la fecha de próximo pago controla la suspensión.

### Cortes por factura vencida

<figure><img src="../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

Este método suspende a los clientes con una factura vencida y pendiente de pago.

| Dato                 | Valor                |
| -------------------- | -------------------- |
| Cliente              | Denisse Saucedo      |
| Día de corte         | 15 de cada mes       |
| Días de gracia       | 5 días               |
| Fecha límite de pago | 20 de agosto de 2026 |

El 15 de agosto, si Denisse no paga, su estado cambia a **Adeudo**. El sistema también genera una factura con esa fecha de emisión.

La fecha de vencimiento suma los días de gracia al día de corte. En este ejemplo, la factura vence el 20 de agosto de 2026.

<figure><img src="../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>

El sistema no suspende el servicio antes del vencimiento de la factura. En la fecha de vencimiento, suspende al cliente si la factura está **Pendiente**.

Si la factura está **Pagada**, el sistema no realiza el corte. Si está **Anulada**, el sistema ignora esa factura.

### Recomendación

Elija el método que coincida con su proceso de cobranza. Si tiene dudas, recomendamos **Cortes por fecha vencida**. Es la opción más simple de administrar.
