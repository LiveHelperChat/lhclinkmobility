# link mobility integration
https://linkmobility.com WhatsApp support integration

# Installation

Clone repository to extesnions folder should look like

> extension > lhclinkmobility

There is no need to add this extension to settings file.

Run cronjob

> /usr/bin/php cron.php -s site_admin -e lhclinkmobility -c cron/import
 
It will install all the configuration. After this step go to 

> System configuration > Live help configuration > Incoming webhooks
 
* Find `LinkMobilityAPI` and edit. Click `Show integration information` and in `Attributes` section fill your username.
* Set department which one to use.

Each time you import you will have to enter attributes.

Also make sure you copy `URL to put in third party Rest API service` and put in your provider. Each time you reimport `Identifier` changes. You can change it to old one after import.

# Bot configuration

Imported default bot has few sampels what type of messages are support. To test it out edit department and choose as default bot newly imported bot. `LinkMobilityAPI`

Once you setup bot for department you can try to send messages and write 

`list`, `help`