Remote - Subscriber Notifications & Posting
======

Datastreams are the life blood of Project L.
Pretty much all the data from one moment in time transferred to many other people, places and times.

These Datastreams travel from a subscriber's remote to the L/Cloud to other subscriber remotes and TVs.

Each datastream must have a streamtype.


####JSON representation of a Remote:

```json
{
    "remote": {
        "remoteid": "",
        "androidid": "",
        "udid": "",
        "remotetype": "",
        "carrier": "",
        "device": [
            {
                "ble": "",
                "wifi": "",
                "cellular": "",
                "isFast": "",
                "isConnected"
            }
        ],
        "remotegeo": {
            "long": "",
            "lat": ""
        }
    }
}
```

TODO
------------
* Add description of object and its functionality


Repository Goals
------------
* create an example Remote in code
* Learn and experiment through thought


Contribution
------------

Use [Github issues](https://github.com/projectL/Remote/issues) for requests.


Inspirations
------------
the real remote control, spaces of confinement, public payphones, public places
