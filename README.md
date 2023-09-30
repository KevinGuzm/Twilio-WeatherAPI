# Automated Text Messaging Project with WeatherAPI

This is a Python application that automates sending text messages using the WeatherAPI and a phone number provided by WeatherAPI. The application queries the current weather information and then sends a text message with the data to the specified phone number.

## Requirements

Make sure you have the following elements installed before running the application:

- Python 3.x
- Required Python packages (can be installed using `twilio==7.14.0`, `pandas==1.3.4`, `requests==2.22.0`, `tqdm==4.62.3`):
  - requests: For making HTTP requests to the WeatherAPI.
  - twilio: For sending text messages via the Twilio platform.

## Configuration

Before running the application, make sure to configure the following parameters properly:

1. Obtain an API key from WeatherAPI by registering at [https://www.weatherapi.com/](https://www.weatherapi.com/). Replace `YOUR_API_KEY` in the code with your API key.

2. Register at [Twilio](https://www.twilio.com/) and set up an account. Get your Account SID and Auth Token from Twilio.

3. Configure Twilio authentication information in the code, replacing `TWILIO_ACCOUNT_SID`, `TWILIO_AUTH_TOKEN`, `TWILIO_PHONE_NUMBER`, and `DESTINATION_PHONE_NUMBER` with the appropriate values.

## Usage

Once you have configured the parameters, you can manually run the application with the following command:
`python3 twilio_script.py`

## Automation with crontab (Optional)

If you want to automate the execution of the application to send text messages regularly, you can use crontab. You can add a cron task on your system to run the script `python3 twilio_script.py` at specific times.

For example, if you want the application to run every day at 8:00 AM, you can set up a cron task as follows:

`0 8 * * * /usr/bin/python3 /path/to/your/project/twilio_script.py >> /path/to/your/project/log.txt 2>&1`

──────────────────────

# Proyecto de Automatización de Mensajes de Texto con WeatherAPI

Este proyecto es una aplicación de Python que automatiza el envío de mensajes de texto utilizando la API de WeatherAPI y un número de teléfono proporcionado por WeatherAPI. La aplicación consulta la información meteorológica actual y luego envía un mensaje de texto con los datos al número de teléfono especificado.

## Requisitos

Asegúrate de tener instalados los siguientes elementos antes de ejecutar la aplicación:

- Python 3.x
- Paquetes Python requeridos (se pueden instalar usando `twilio==7.14.0` `pandas==1.3.4` `requests==2.22.0` `tqdm==4.62.3`):
  - requests: Para realizar solicitudes HTTP a la API de WeatherAPI.
  - twilio: Para enviar mensajes de texto a través de la plataforma Twilio.

## Configuración

Antes de ejecutar la aplicación, asegúrate de configurar adecuadamente los siguientes parámetros:

1. Obtén una clave API de WeatherAPI registrándote en [https://www.weatherapi.com/](https://www.weatherapi.com/). Reemplaza `TU_API_KEY` en el código con tu clave API.

2. Regístrate en [Twilio](https://www.twilio.com/) y configura una cuenta. Obten tu SID de cuenta y token de autenticación de Twilio.

3. Configura la información de autenticación de Twilio en el código, reemplazando `TWILIO_ACCOUNT_SID`, `TWILIO_AUTH_TOKEN`, `TWILIO_PHONE_NUMBER` y `DESTINATION_PHONE_NUMBER` con los valores adecuados.

## Uso

Una vez que hayas configurado los parámetros, puedes ejecutar la aplicación manualmente con el siguiente comando:
`python3 twilio_script.py`

## Automatización con crontab (Opcional):

Si deseas automatizar la ejecución de la aplicación para que envíe mensajes de texto de forma regular, puedes usar crontab, puedes agregar una tarea cron en tu sistema para que ejecute el script `python3 twilio_script.py` en un horario específico.

Por ejemplo, si deseas que la aplicación se ejecute todos los días a las 8:00 AM, puedes configurar una tarea cron de la siguiente manera:

`0 8 * * * /usr/bin/python3 /ruta/a/tu/proyecto/twilio_script.py >> /ruta/a/tu/proyecto/log.txt 2>&1`
