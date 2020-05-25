# Club St Hil'Air bot

Ce bot, en Python d'après l'[excellent tuto](https://dev.to/zeyu2001/i-built-a-python-whatsapp-bot-to-keep-me-sane-during-quarantine-nph) de Zhang Zeyu utilise l'API Twilio whatsapp pour fournir quelques services utiles sur le group WhatsApp du Club St Hil'Air:

* Etat des balises FFVL sur Isère / Savoie / Haute Savoie
* Coordonnées / carte d'un point de rendez-vous, d'un décollage, d'un atterissage
* Les photos (pilote & voile) du trombinoscope

## A faire

* [ ] Coordonnées / carte d'un point de rendez-vous, d'un décollage, d'un atterissage
* [ ] Etat des balises FFVL sur Isère / Savoie / Haute Savoie
* [ ] Les photos (pilote & voile) du trombinoscope

## Développer

* Installer l'env Python: `python3 -m venv venv && source venv/bin/activate && pip3 install -r requirements.txt`
* Démarrer l'app: `python manage.py runserver`
* Démarrer ngrok: `ngrok http 8000`
* Mettre à jour `ALLOWED_HOSTS` dans settings.py avec le hostname de ngrok
* Twilio: https://www.twilio.com/console/sms/whatsapp/sandbox
* Twilio: mettre à jour la configuration Twilio sandbox de `WHEN A MESSAGE COMES IN` avec l'URL ngrok + `/bot/`
* Editer `bot_app/views.py`