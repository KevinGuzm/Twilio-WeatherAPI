# Proyecto de Automatización de Mensajes de Texto con WeatherAPI

Este proyecto es una aplicación de Python que automatiza el envío de mensajes de texto utilizando la API de WeatherAPI y un número de teléfono proporcionado por WeatherAPI. La aplicación consulta la información meteorológica actual y luego envía un mensaje de texto con los datos al número de teléfono especificado.

## Requisitos

Asegúrate de tener instalados los siguientes elementos antes de ejecutar la aplicación:

- Python 3.x
- Paquetes Python requeridos (se pueden instalar usando `twilio==7.14.0
pandas==1.3.4
requests==2.22.0
tqdm==4.62.3`):
  - requests: Para realizar solicitudes HTTP a la API de WeatherAPI.
  - twilio: Para enviar mensajes de texto a través de la plataforma Twilio.

## Configuración

Antes de ejecutar la aplicación, asegúrate de configurar adecuadamente los siguientes parámetros:

1. Obtén una clave API de WeatherAPI registrándote en [https://www.weatherapi.com/](https://www.weatherapi.com/). Reemplaza `TU_API_KEY` en el código con tu clave API.

2. Regístrate en [Twilio](https://www.twilio.com/) y configura una cuenta. Obten tu SID de cuenta y token de autenticación de Twilio.

3. Configura la información de autenticación de Twilio en el código, reemplazando `TWILIO_ACCOUNT_SID`, `TWILIO_AUTH_TOKEN`, `TWILIO_PHONE_NUMBER` y `DESTINATION_PHONE_NUMBER` con los valores adecuados.

## Uso

Una vez que hayas configurado los parámetros, puedes ejecutar la aplicación manualmente con el siguiente comando:

```bash
python3 twilio_script.py

