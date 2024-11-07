# Proyecto de Pruebas Automatizadas para Urban Routes

## Descripción del Proyecto

Este proyecto contiene pruebas automatizadas para verificar la funcionalidad de la aplicación Urban Routes, que permite a los usuarios solicitar taxis, configurar tarifas, agregar métodos de pago y realizar otras acciones relacionadas con la gestión de viajes en taxi.

Las pruebas están implementadas utilizando Selenium WebDriver para automatizar la interacción con la aplicación web, cubriendo escenarios como la configuración de la dirección, la selección de tarifas, la adición de tarjetas de crédito y la solicitud de artículos adicionales.

## Tecnologías Utilizadas

- **Selenium WebDriver**: Para automatizar las pruebas de la interfaz de usuario.
- **Python**: Lenguaje de programación utilizado para escribir las pruebas y manejar la lógica de automatización.
- **pytest**: Framework de pruebas para ejecutar y gestionar las pruebas automatizadas.
- **WebDriverWait**: Para esperar a que los elementos estén presentes antes de interactuar con ellos.

## Estructura del Proyecto

El proyecto está dividido en los siguientes archivos principales:

- **`data.py`**: Contiene las configuraciones de datos necesarias, como las direcciones, el número de teléfono y la tarjeta de crédito.
- **`main.py`**: Contiene la lógica de pruebas, incluidas las interacciones con la aplicación (por ejemplo, establecer la dirección, seleccionar la tarifa, agregar el método de pago, etc.).
- **`retrieve_phone_code()`**: Función para interceptar el código de confirmación enviado al teléfono del usuario.

## Instrucciones para Ejecutar las Pruebas

1. **Instalar las dependencias**:
   - Asegúrate de tener Python 3.x instalado.
   - Instala las dependencias necesarias utilizando el siguiente comando:

   ```bash
   pip install -r requirements.txt
   ```

2. **Configuración de Selenium**:
   - Asegúrate de tener el controlador adecuado para el navegador que deseas usar (por ejemplo, `chromedriver` para Chrome).

3. **Ejecutar las pruebas**:
   - Puedes ejecutar las pruebas utilizando pytest de la siguiente manera:

   ```bash
   pytest main.py
   ```

4. **Resultado esperado**:
   - Las pruebas deben cubrir varios escenarios, como la configuración de direcciones, la selección de tarifas y el proceso de pago.
   - Asegúrate de que todos los tests pasen correctamente para validar la funcionalidad de la aplicación.

## Descripción de las Pruebas

Las pruebas automatizadas cubren el proceso completo de pedir un taxi, incluyendo:

- **Configurar las direcciones**: Establecer la dirección de origen y destino.
- **Seleccionar la tarifa Comfort**: Validar la opción de tarifa.
- **Agregar un número de teléfono**: Ingresar un número de teléfono válido y obtener el código de confirmación.
- **Agregar una tarjeta de crédito**: Ingresar los datos de la tarjeta de crédito y el código de seguridad.
- **Escribir un mensaje para el conductor**: Ingresar un mensaje en el campo correspondiente.
- **Solicitar artículos adicionales**: Pedir mantas, pañuelos y helados.
- **Esperar la asignación del conductor**: Verificar la aparición del modal con la información del conductor y la cuenta regresiva.

