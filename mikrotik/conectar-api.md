---
description: Conecta y administra los routers MikroTik de tu red.
---

# Conectar API

### ¿Qué es el módulo MikroTik?

El módulo **MikroTik** conecta la plataforma con los routers de tu red.

Registra clientes en el router y asigna planes de velocidad. También suspende clientes morosos y los reactiva tras un pago.

<figure><img src="../.gitbook/assets/image (124).png" alt="Vista principal del módulo MikroTik"><figcaption><p>Vista principal del módulo MikroTik.</p></figcaption></figure>

### Registrar un router MikroTik

Selecciona **Registrar Router MikroTik**. Ingresa la dirección IP, el usuario y la contraseña del equipo.

Antes de registrarlo, prepara el router desde Winbox:

#### 1. Habilitar la API

Ve a **IP** → **Services**. Habilita el servicio `api`, que usa el puerto `8728` por defecto.

<figure><img src="../.gitbook/assets/image (125).png" alt="Servicio API habilitado en MikroTik"><figcaption><p>Habilita el servicio API antes de conectar el router.</p></figcaption></figure>

#### 2. Permitir el acceso en el Firewall

Ve a **IP** → **Firewall** → **Filter Rules**. Permite las conexiones entrantes al puerto `8728`.

<figure><img src="../.gitbook/assets/image (126).png" alt="Regla de Firewall para la API de MikroTik"><figcaption><p>Permite conexiones autorizadas al puerto de la API.</p></figcaption></figure>

#### 3. Crear un usuario para la plataforma

Ve a **System** → **Users**. Crea un usuario exclusivo con el grupo `full`.

<figure><img src="../.gitbook/assets/image (127).png" alt="Usuario de MikroTik con permisos de administración"><figcaption><p>Crea un usuario dedicado para la conexión de la plataforma.</p></figcaption></figure>

{% hint style="warning" %}
Protege el acceso a la API. Permite conexiones solo desde las direcciones autorizadas.
{% endhint %}

### Comprobar la conexión

La tabla muestra el **Estado API** de cada router. Selecciona el botón celeste con el icono de WiFi en **Acciones** para ejecutar una prueba.

La prueba usa las credenciales guardadas. Confirma que el router responda correctamente.

<figure><img src="../.gitbook/assets/image (128).png" alt="Acción para comprobar la conexión API"><figcaption><p>Ejecuta una prueba para confirmar la conexión con el router.</p></figcaption></figure>

### Instalar reglas de corte

Selecciona el botón verde con el escudo y la palomita. Esta acción instala reglas de Firewall en el MikroTik.

Las reglas bloquean el tráfico de clientes suspendidos. También redirigen las conexiones según la configuración del sistema.

<figure><img src="../.gitbook/assets/image (129).png" alt="Acción para instalar reglas de corte"><figcaption><p>Instala las reglas de corte desde la plataforma.</p></figcaption></figure>

#### Verificar las reglas instaladas

Tras la instalación, verifica las reglas en el Firewall del MikroTik.

<figure><img src="../.gitbook/assets/image (130).png" alt="Reglas de corte instaladas en el Firewall de MikroTik"><figcaption><p>Reglas de corte instaladas en el Firewall de MikroTik.</p></figcaption></figure>

### Bloquear contenido para adultos

Selecciona **Instalar Reglas Adultos**, identificado con el botón gris de candado. El sistema instala filtros en el Firewall del MikroTik.

Estos filtros usan listas de DNS e IP. Bloquean el acceso a sitios con contenido explícito para los clientes de ese router.

### Editar o eliminar un router

Selecciona **Editar**, identificado con el botón amarillo de lápiz, para actualizar la IP, el puerto API o las credenciales.

Selecciona **Eliminar**, identificado con el botón rojo de papelera, para quitar el router de la plataforma.

{% hint style="warning" %}
Al eliminar un router, pierdes la administración automática de sus clientes vinculados.
{% endhint %}
