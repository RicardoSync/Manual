---
description: Centraliza el monitoreo del tráfico de las interfaces MikroTik.
---

# Monitor de Interfaces

### ¿Qué es el Monitor de Interfaces?

El **Monitor de Interfaces** centraliza el tráfico de puertos y enlaces de tus routers MikroTik.

Supervisa las interfaces más importantes de toda la red desde una sola vista. Conserva un historial de su consumo de ancho de banda.

<figure><img src="../.gitbook/assets/image (137).png" alt=""><figcaption></figcaption></figure>

### Importar interfaces

Selecciona **Seleccionar / Importar Interfaces**, identificado con el botón azul superior.

1. Elige el router MikroTik que contiene las interfaces.
2. Espera mientras el sistema obtiene los puertos disponibles.
3. Marca las interfaces que deseas vigilar y selecciona **Guardar**.

La lista incluye puertos como `ether1`, `ether2` y `bridge`. Tras guardar, el sistema comienza a registrar su tráfico.

<figure><img src="../.gitbook/assets/image (138).png" alt=""><figcaption></figcaption></figure>

### Consultar la gráfica de consumo

Selecciona **Gráfica**, identificado con el botón verde de barras, junto a una interfaz.

La vista detallada muestra el historial de tráfico de descarga y subida. Úsala para identificar horarios con alta demanda o enlaces saturados.

<figure><img src="../.gitbook/assets/image (139).png" alt=""><figcaption></figcaption></figure>

### Eliminar una interfaz del monitor

Selecciona **Eliminar**, identificado con el botón rojo de papelera, al final de la fila. Confirma la acción para quitar la interfaz del monitor.

<figure><img src="../.gitbook/assets/image (140).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
Al eliminar una interfaz, el sistema deja de monitorearla. También borra el historial de gráficas almacenado para ese puerto.
{% endhint %}
