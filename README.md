# link mobility integration
https://linkmobility.com WhatsApp support integration

# Installation

Clone repository to extesnions folder should look like

> extension > lhclinkmobility

Run cronjob

> /usr/bin/php cron.php -s site_admin -e lhclinkmobility -c cron/import
 
It will install all the configuration. After this step go to 

> System configuration > Live help configuration > Incoming webhooks
 
* Find `LinkMobilityAPI` and edit. Click `Show integration information` and in `Attributes` section fill your username.
* Set department which one to use.

Each time you import you will have to enter attributes.