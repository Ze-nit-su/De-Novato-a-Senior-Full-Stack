# Rescue & Mining Robot Technical Specification & Emergency Protocol Hub

## Descripción General

Una plataforma web estática destinada a los ingenieros de campo y rescatistas en Japón (por ejemplo, para el Departamento de Bomberos de Tokio o empresas mineras en Hokkaido).

Esta alojará la documentación técnica de la flota de robots de rescate ante terremotos y minería subterránea, además de los formularios estáticos para reportar averías de los droides tras una misión.

## Objetivos

* Presentar de manera clara y ultra-legible las especificaciones de hardware del robot insignia.

* Crear una guía visual rápida de los protocolos de rescate que el robot ejecuta de forma autónoma.

* Diseñar un formulario estático estructurado para que el operario reporte piezas dañadas.

## Solicitud Cliente

> *Hola, soy la Directora de Operaciones de J-RARM (Japan Robotic Rescue & Mining).*
>
> *Tras el último sismo en la región de Tohoku, nuestros ingenieros notaron que los manuales en PDF son difíciles de leer en las tablets de campo bajo condiciones de polvo o poca luz.*
>
>*Necesitamos un sitio web interno, extremadamente limpio, donde se listen las especificaciones de nuestro robot de rescate 'Kyuu-01' (救).*
>
>*Queremos ver sus dimensiones, tipos de sensores, y un formulario donde los técnicos reporten qué partes del robot fallaron (sensores, orugas, brazos hidráulicos) al salir de la mina o la zona de desastre.*
>
>*El diseño debe ser impecable, transmitir seriedad, alta tecnología japonesa y tener un esquema de color que resalte las alertas.*

## Especificaciones Proyecto

El sitio web debe contar con las siguientes secciones y características, haciendo únicamente uso de HTML5 y CSS3:

* **Estructura Semántica Obligatoria**
  * Usar de forma correcta ``<header>``, ``<nav>``, ``<main>``, ``<section>``, ``<article>``, ``<aside>``, y ``<footer>``.

* **Página Principal / Dashboard Técnico**
  * Encabezado con el logo simulado de la organización.
  * Hora actual (estática).
  * Estado del sistema (un indicador visual de "Flota Operativa").

* **Una sección dedicada al Robot "Kyuu-01"**
  * Descripción de su propósito (búsqueda de sobrevivientes en túneles colapsados).
  * Lista de sus componentes clave.

* **Ficha Técnica (Tabla)**
  * Una tabla HTML perfectamente estilizada que compare las especificaciones del robot en dos entornos:
    * "Modo Minería" vs "Modo Rescate Urbano".
  * Debe incluir filas para:
    * Peso.
    * Autonomía de batería.
    * Sensores activos (LIDAR, Térmico, Gases).
    * Resistencia a la presión.

* **Sección de Protocolos de Emergencia**
  * Un sistema de tarjetas (Cards) maquetado con CSS Grid que muestre los 3 pasos clave en caso de pérdida de conexión con el robot en el subsuelo.
  * Cada tarjeta debe tener un borde o color que indique la severidad del paso.

* **Formulario de Reporte de Daños en Campo (Crucial)**
  * Un formulario HTML completo que contenga:
    * Campo de texto para el ID del Operario y el ID del Robot.
    * Un menú desplegable (``<select>``) para elegir el área del robot afectada (Sistema de Locomoción, Bloque de Sensores, Batería, Brazo Manipulador).
    * Botones de opción (``<input type="radio">``) para marcar el nivel de daño:
      * Crítico.
      * Moderado.
      * Leve.
    * Un área de texto (``<textarea>``) para que el técnico describa detalladamente el incidente en la mina o zona de desastre.
    * Un botón de envío (``<button type="submit">``) estilizado con un efecto visual al pasar el cursor por encima (hover).

* **Diseño Visual y CSS (Estilo Monozukuri)**
  * Paleta de colores:
    * Fondo oscuro o gris industrial muy limpio, con acentos en colores de seguridad industrial (como el naranja de rescate #FF4500 o el amarillo de advertencia).
  * Las tipografías deben ser de tipo sans-serif, muy legibles.
  * Diseño Responsivo:
    * El diseño debe cambiar fluidamente si se mira en una pantalla de computadora de escritorio o en una pantalla vertical de una tablet de campo.
  * Variables CSS al inicio del archivo de estilos para definir los colores principales, facilitando si en el futuro el deseo colocar un "Modo Nocturno".

## Créditos

| | |
| :---: | :---: |
| **Autor** | Hikari, Ren |
| **Día Creación** | 02 |
| **Mes Creación** | 07 |
| **Año Creación** | 2026 |
| **Día Finalización** | xx |
| **Mes Finalización** | xx |
| **Año Finalización** | 20xx |
| **Licencia** | [MIT](/LICENSE) |
