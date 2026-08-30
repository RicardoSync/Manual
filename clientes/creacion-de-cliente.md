# Creación de cliente

<figure><img src="../.gitbook/assets/Captura de Pantalla 2026-08-29 a la(s) 20.38.09.png" alt="Formulario para crear un cliente"><figcaption><p>Formulario de creación de clientes</p></figcaption></figure>

### Datos personales

Antes de registrar un cliente, define su método de conexión.

Para **SimpleQueue**, necesitas una dirección IP fija. Si usas DHCP, identifica la IP asignada.

Para **PPPoE**, necesitas el usuario, la contraseña y el perfil asociado. El módulo también admite paquetes de SimpleQueue.

Completa los siguientes datos:

1. **Nombre:** escribe el nombre completo del cliente.
2. **DNI / RFC:** ingresa el identificador fiscal o personal. Usa `NA` si no lo tienes.
3. **Código de país:** selecciona el código del número telefónico. El valor predeterminado es `+52` para México.
4. **Teléfono:** ingresa los 10 dígitos de WhatsApp, sin lada.
5. **Dirección:** ingresa el domicilio físico del cliente.

### Conexión

<figure><img src="../.gitbook/assets/Captura de Pantalla 2026-08-29 a la(s) 20.43.13.png" alt="Configuración de conexión del cliente"><figcaption><p>Configuración de conexión</p></figcaption></figure>

Define el tipo de conexión y cómo administrarás el servicio del cliente.

#### Cliente SimpleQueue con IP

<figure><img src="../.gitbook/assets/Captura de Pantalla 2026-08-29 a la(s) 20.45.27.png" alt="Configuración de un cliente SimpleQueue"><figcaption><p>Cliente SimpleQueue con IP</p></figcaption></figure>

Registra la dirección IP fija asignada al cliente.

Después, selecciona el MikroTik donde se administrará la conexión.

#### Cliente PPPoE

<figure><img src="../.gitbook/assets/Captura de Pantalla 2026-08-29 a la(s) 20.46.12.png" alt="Configuración de un cliente PPPoE"><figcaption><p>Cliente PPPoE</p></figcaption></figure>

Ingresa el usuario y la contraseña PPPoE configurados en la ONU, antena o equipo del cliente.

### Planes

<figure><img src="../.gitbook/assets/Captura de Pantalla 2026-08-29 a la(s) 20.47.18.png" alt="Selección de planes para el cliente"><figcaption><p>Configuración de planes</p></figcaption></figure>

Selecciona la comunidad y la antena AP del cliente.

Deja los valores predeterminados si estos datos no aplican.

En **Paquete / plan**, elige el plan correspondiente al tipo de conexión:

* **\[SimpleQueue]:** paquete de internet para clientes SimpleQueue.
* **\[PPPoE]:** nombre del perfil configurado en MikroTik.

Usa **Servicios extra** para cargos independientes del internet. Por ejemplo, la renta de un dispositivo.

### Facturacion

<figure><img src="../.gitbook/assets/Captura de Pantalla 2026-08-29 a la(s) 20.49.53.png" alt="Configuración de facturación del cliente"><figcaption><p>Configuración de facturación</p></figcaption></figure>

Selecciona el día de corte del cliente, entre el 1 y el 31 de cada mes.

Define el mes en que iniciará el pago mensual. En este ejemplo, se usa agosto.

Ingresa las coordenadas de latitud y longitud del domicilio.

### Resumen

<figure><img src="../.gitbook/assets/Captura de Pantalla 2026-08-29 a la(s) 20.51.33.png" alt="Resumen de datos antes de crear el cliente"><figcaption><p>Resumen de la configuración</p></figcaption></figure>

Revisa toda la información antes de registrar al cliente.

Verifica la IP o las credenciales PPPoE, el paquete, el día de corte y los días de gracia.

Cuando todo sea correcto, confirma y guarda el cliente.

### Posibles Avisos

<figure><img src="../.gitbook/assets/Captura de Pantalla 2026-08-29 a la(s) 20.53.10.png" alt="Aviso de conflicto al crear un cliente"><figcaption><p>Aviso de conflictos detectados</p></figcaption></figure>

El sistema detecta direcciones IP y usuarios PPPoE que ya pertenecen a otro cliente.

Si existe un conflicto, no podrás registrar el cliente. Corrige los datos y vuelve a intentarlo.
