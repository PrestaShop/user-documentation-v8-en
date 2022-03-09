# Geolocation

Geolocation is "_the identification of the real-world geographic location of an object, such as a radar, a mobile phone or an Internet-connected computer_" (read more on [Wikipedia](http://en.wikipedia.org/wiki/Geolocation)). In our case, geolocation is used to discover the location of a visitor, using his or her computer's IP and other tools. One of the uses of geolocation is to block visitors from certain cities/countries.

As indicated the first time you open the "Geolocation" page, in order to use geolocation, you need to download a special file first: [http://geolite.maxmind.com/download/geoip/database/GeoLiteCity.dat.gz](http://geolite.maxmind.com/download/geoip/database/GeoLiteCity.dat.gz). This file is the GeoLite City database from MaxMind, an accurate database of cities and locations. Download it by clicking on the link, and then decompress it into the `/tools/geoip/` directory of your PrestaShop installation. Once the file in place, enable the "Geolocation by IP address" option, and you are set.

![](<../../../../.gitbook/assets/64225610 (4) (4).png>)

## Options <a href="#geolocation-options" id="geolocation-options"></a>

You can choose which countries can access your shop (by default, all of them), and set PrestaShop's behaviors for restricted and unrestricted countries (or "other" countries). You choose between these three options:

* Visitors cannot see your catalog.
* Visitors can see your catalog but cannot make an order. In effect, your store is in "Catalog mode".
* All features are available (only for unrestricted countries).\
  \
  ![](<../../../../.gitbook/assets/64225611 (4) (2) (3).png>)

You can select or deselect all countries at once by checking the box at the top of the list (next to "Name"). When selecting countries that can access your online shop, make sure to not block any country by mistake, as you would lose all potential sales to its inhabitants!

## Whitelist of IP address <a href="#geolocation-whitelistofipaddress" id="geolocation-whitelistofipaddress"></a>

This section enables you to accept specific IPs address despite a blockade. It can be useful in case of spammers, bots or attacks. It is already filled with a list of known good IPs. Add as many as needed, one per line, and click "Save".

![](<../../../../.gitbook/assets/64225612 (4).png>)
