BaseMaps for CKAN
============================================================================


* `Installation`_
* `Configuration`_

Installation
------------

**This plugin dependencies ckanext-spatial Plugin.**

The current version of ckanext-basemaps has been developed and tested again
**CKAN 2.2.x**. We assume a running CKAN 2.2.x instance.
 
The installation has the following steps, assuming you have a running
copy of CKAN:

#. Install the extension from its source repository::

    (pyenv) $ pip install -e git+https://github.com/niryuu/ckanext-basemaps


Configuration
-------------

These are the configuration options used by the extension 

#. Map Names::

    ckanext.basemaps.laylers.names = 地理院地図（標準）, 地理院地図（白地図）,電子国土基本図（オルソ画像）

#. Map URLs::

    ckanext.basemaps.laylers.urls = http://{s}.gsi.go.jp/xyz/std/{z}/{x}/{y}.png, http://{s}.gsi.go.jp/xyz/blank/{z}/{x}/{y}.png, http://{s}.gsi.go.jp/xyz/ort/{z}/{x}/{y}.jpg

#. Map Attributions(Optional)::

    ckanext.basemaps.laylers.attributions = 国土地理院,国土地理院,国土地理院

#. Map Subdomains(if you use subdomain)::

    ckanext.basemaps.laylers.subdomains = [["cyberjapandata-t1","cyberjapandata-t2","cyberjapandata-t3"],["cyberjapandata-t1","cyberjapandata-t2","cyberjapand    ata-t3"],["cyberjapandata-t1","cyberjapandata-t2","cyberjapandata-t3"],["cyberjapandata-t1","cyberjapandata-t2","cyberjapandata-t3"]]

NOTE: subdomains should be valid JSON
