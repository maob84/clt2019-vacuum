# clt2019-vacuum
Slides and documents for talk at CLT2019 about connecting Xiaomi MI vacuum with Alexa.


### Interfacing with Valetudo Backend ###

 * Starting vacuum: `curl --request PUT --url http://192.168.1.17/api/start_cleaning`
 * Stopping vacuum: `curl --request PUT --url http://192.168.1.17/api/stop_cleaning`
 * Sending vacuum back home: `curl --request PUT --url http://192.168.1.17/api/drive_home`
