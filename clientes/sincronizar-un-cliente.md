# Sincronizar un cliente

<figure><img src="../.gitbook/assets/image (82).png" alt="Opción Sincronizar en el perfil de un cliente"><figcaption><p>Sincroniza la configuración del cliente</p></figcaption></figure>

La sincronización crea o actualiza la configuración del cliente en MikroTik.

Úsala después de modificar la IP, la velocidad o el plan del cliente.

### Requisitos

Antes de sincronizar, verifica lo siguiente:

* **Simple Queue:** el nombre del cliente debe coincidir con el nombre de la cola en MikroTik.
* **PPPoE:** el usuario debe coincidir con el usuario registrado para ese cliente.
* **Plan PPPoE:** el perfil del paquete debe existir en MikroTik con el mismo nombre.

### Sincronizar el cliente

1. Abre el perfil del cliente.
2. Selecciona **Sincronizar**.
3. Confirma la acción, si el sistema lo solicita.

### Resultado de la sincronización

<figure><img src="../.gitbook/assets/image (83).png" alt="Mensaje de sincronización exitosa del cliente"><figcaption><p>Sincronización completada</p></figcaption></figure>

Al sincronizar, ocurre una de estas acciones:

* Si el cliente ya existe, el sistema actualiza la velocidad, IP u otros cambios.
* Si no existe, el sistema crea una nueva cola Simple Queue o un secreto PPPoE.

<figure><img src="../.gitbook/assets/image (84).png" alt="Configuración del cliente actualizada en MikroTik"><figcaption><p>Configuración actualizada en MikroTik</p></figcaption></figure>

### Ejemplo: actualizar una dirección IP

<figure><img src="../.gitbook/assets/image (85).png" alt="Cliente con la dirección IP anterior antes de sincronizar"><figcaption><p>Dirección IP antes de la actualización</p></figcaption></figure>

El cliente tenía asignada la IP `172.16.20.233`.

Después de cambiar la IP en el sistema, selecciona **Sincronizar**. El sistema actualiza la dirección en la cola Simple Queue.

<figure><img src="../.gitbook/assets/image (86).png" alt="Opción para sincronizar el cliente después de modificar su dirección IP"><figcaption><p>Inicia la sincronización</p></figcaption></figure>

<figure><img src="../.gitbook/assets/image (87).png" alt="Dirección IP actualizada correctamente en la cola Simple Queue"><figcaption><p>Dirección IP actualizada</p></figcaption></figure>

La nueva dirección IP queda aplicada correctamente en MikroTik.
