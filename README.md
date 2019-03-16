# clt2019-vacuum
Slides and documents for talk at CLT2019 about connecting rooted Xiaomi MI vacuum cleaner with Alexa/Amazon Echo.


### Interfacing with Valetudo Backend ###

 * Starting vacuum: `curl --request PUT --url http://192.168.1.17/api/start_cleaning`
 * Stopping vacuum: `curl --request PUT --url http://192.168.1.17/api/stop_cleaning`
 * Sending vacuum back home: `curl --request PUT --url http://192.168.1.17/api/drive_home`


#### Fauxmo ####

 * patching fauxmo (PUT handling code): `patch -p1 < fauxmo-vacuum.diff`
 * configuring fauxmo: adding appropriate FAUXMOS
 * copying to rockrobo: `scp fauxmo.py root@robot:/usr/local/bin`
 * copying upstart configuration to rockrobo: `scp fauxmo.conf root@robot:/etc/init/`
 * installing python on rockrobo
	* `apt-get update`
	* `apt-get install python python-requests`
 * `service start fauxmo`

### Misc ###

For further questions or comments do not hestiate to contact me under <marcus.obst@outlook.de>.
