# api documentation for  [shipit (v1.0.2)](https://github.com/sailrish/shipit#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-shipit.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-shipit) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-shipit.svg)](https://travis-ci.org/npmdoc/node-npmdoc-shipit)
#### This module allows you to connect to many shipping carriers like UPS and FedEx and download tracking data for your packages in a common schema

[![NPM](https://nodei.co/npm/shipit.png?downloads=true)](https://www.npmjs.com/package/shipit)

[![apidoc](https://npmdoc.github.io/node-npmdoc-shipit/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-shipit_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-shipit/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-shipit/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-shipit/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Rishi Arora"
    },
    "bugs": {
        "url": "https://github.com/sailrish/shipit/issues"
    },
    "dependencies": {
        "async": "~0.2.10",
        "change-case": "~1.0.5",
        "cheerio": "~0.13.1",
        "grunt": "~0.4.2",
        "grunt-contrib-coffee": "~0.10.0",
        "moment-timezone": "~0.4.0",
        "request": "~2.33.0",
        "underscore": "~1.5.2",
        "xml2js": "~0.4.1"
    },
    "description": "This module allows you to connect to many shipping carriers like UPS and FedEx and download tracking data for your packages in a common schema",
    "devDependencies": {
        "bondjs": "~1.0.0",
        "chai": "~1.9.0",
        "grunt-mocha-test": "~0.6.3",
        "mocha": "~1.17.1"
    },
    "directories": {
        "test": "test"
    },
    "dist": {
        "shasum": "59395e79a0f95667cdc8b9c2e1dd5dd9df2eb4f6",
        "tarball": "https://registry.npmjs.org/shipit/-/shipit-1.0.2.tgz"
    },
    "gitHead": "98fae33441e8059229d7c824d29665b57322b13d",
    "homepage": "https://github.com/sailrish/shipit#readme",
    "keywords": [
        "FedEx",
        "UPS",
        "Postal",
        "Service",
        "Mail",
        "Package",
        "Shipping"
    ],
    "license": "MIT",
    "main": "lib/main.js",
    "maintainers": [
        {
            "name": "sailrish",
            "email": "rishi.r.arora@gmail.com"
        }
    ],
    "name": "shipit",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/sailrish/shipit.git"
    },
    "scripts": {
        "test": "grunt"
    },
    "version": "1.0.2"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module shipit](#apidoc.module.shipit)
1.  [function <span class="apidocSignatureSpan">shipit.</span>A1Client (options)](#apidoc.element.shipit.A1Client)
1.  [function <span class="apidocSignatureSpan">shipit.</span>AmazonClient (options)](#apidoc.element.shipit.AmazonClient)
1.  [function <span class="apidocSignatureSpan">shipit.</span>CanadaPostClient (_arg, options)](#apidoc.element.shipit.CanadaPostClient)
1.  [function <span class="apidocSignatureSpan">shipit.</span>DhlClient (_arg, options)](#apidoc.element.shipit.DhlClient)
1.  [function <span class="apidocSignatureSpan">shipit.</span>DhlGmClient (options)](#apidoc.element.shipit.DhlGmClient)
1.  [function <span class="apidocSignatureSpan">shipit.</span>FedexClient (_arg, options)](#apidoc.element.shipit.FedexClient)
1.  [function <span class="apidocSignatureSpan">shipit.</span>LasershipClient (options)](#apidoc.element.shipit.LasershipClient)
1.  [function <span class="apidocSignatureSpan">shipit.</span>OnTracClient (options)](#apidoc.element.shipit.OnTracClient)
1.  [function <span class="apidocSignatureSpan">shipit.</span>PrestigeClient (options)](#apidoc.element.shipit.PrestigeClient)
1.  [function <span class="apidocSignatureSpan">shipit.</span>UpsClient (_arg, options)](#apidoc.element.shipit.UpsClient)
1.  [function <span class="apidocSignatureSpan">shipit.</span>UpsMiClient (options)](#apidoc.element.shipit.UpsMiClient)
1.  [function <span class="apidocSignatureSpan">shipit.</span>UspsClient (_arg, options)](#apidoc.element.shipit.UspsClient)
1.  [function <span class="apidocSignatureSpan">shipit.</span>guessCarrier (trk)](#apidoc.element.shipit.guessCarrier)
1.  object <span class="apidocSignatureSpan">shipit.</span>A1Client.__super__
1.  object <span class="apidocSignatureSpan">shipit.</span>A1Client.prototype
1.  object <span class="apidocSignatureSpan">shipit.</span>AmazonClient.prototype
1.  object <span class="apidocSignatureSpan">shipit.</span>CanadaPostClient.prototype
1.  object <span class="apidocSignatureSpan">shipit.</span>DhlClient.prototype
1.  object <span class="apidocSignatureSpan">shipit.</span>DhlGmClient.prototype
1.  object <span class="apidocSignatureSpan">shipit.</span>FedexClient.prototype
1.  object <span class="apidocSignatureSpan">shipit.</span>LasershipClient.prototype
1.  object <span class="apidocSignatureSpan">shipit.</span>OnTracClient.prototype
1.  object <span class="apidocSignatureSpan">shipit.</span>PrestigeClient.prototype
1.  object <span class="apidocSignatureSpan">shipit.</span>UpsClient.prototype
1.  object <span class="apidocSignatureSpan">shipit.</span>UpsMiClient.prototype
1.  object <span class="apidocSignatureSpan">shipit.</span>UspsClient.prototype
1.  object <span class="apidocSignatureSpan">shipit.</span>a1
1.  object <span class="apidocSignatureSpan">shipit.</span>amazon
1.  object <span class="apidocSignatureSpan">shipit.</span>canada_post
1.  object <span class="apidocSignatureSpan">shipit.</span>dhl
1.  object <span class="apidocSignatureSpan">shipit.</span>dhlgm
1.  object <span class="apidocSignatureSpan">shipit.</span>fedex
1.  object <span class="apidocSignatureSpan">shipit.</span>lasership
1.  object <span class="apidocSignatureSpan">shipit.</span>ontrac
1.  object <span class="apidocSignatureSpan">shipit.</span>prestige
1.  object <span class="apidocSignatureSpan">shipit.</span>shipper
1.  object <span class="apidocSignatureSpan">shipit.</span>ups
1.  object <span class="apidocSignatureSpan">shipit.</span>upsmi
1.  object <span class="apidocSignatureSpan">shipit.</span>usps

#### [module shipit.A1Client](#apidoc.module.shipit.A1Client)
1.  [function <span class="apidocSignatureSpan">shipit.</span>A1Client (options)](#apidoc.element.shipit.A1Client.A1Client)
1.  object <span class="apidocSignatureSpan">shipit.A1Client.</span>STATUS_TYPES
1.  object <span class="apidocSignatureSpan">shipit.A1Client.</span>__super__

#### [module shipit.A1Client.__super__](#apidoc.module.shipit.A1Client.__super__)
1.  [function <span class="apidocSignatureSpan">shipit.A1Client.__super__.</span>presentLocation (_arg)](#apidoc.element.shipit.A1Client.__super__.presentLocation)
1.  [function <span class="apidocSignatureSpan">shipit.A1Client.__super__.</span>presentLocationString (location)](#apidoc.element.shipit.A1Client.__super__.presentLocationString)
1.  [function <span class="apidocSignatureSpan">shipit.A1Client.__super__.</span>presentPostalCode (rawCode)](#apidoc.element.shipit.A1Client.__super__.presentPostalCode)
1.  [function <span class="apidocSignatureSpan">shipit.A1Client.__super__.</span>presentResponse (response, requestData, cb)](#apidoc.element.shipit.A1Client.__super__.presentResponse)
1.  [function <span class="apidocSignatureSpan">shipit.A1Client.__super__.</span>requestData (requestData, cb)](#apidoc.element.shipit.A1Client.__super__.requestData)

#### [module shipit.A1Client.prototype](#apidoc.module.shipit.A1Client.prototype)
1.  [function <span class="apidocSignatureSpan">shipit.A1Client.prototype.</span>constructor (options)](#apidoc.element.shipit.A1Client.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">shipit.A1Client.prototype.</span>getActivitiesAndStatus (shipment)](#apidoc.element.shipit.A1Client.prototype.getActivitiesAndStatus)
1.  [function <span class="apidocSignatureSpan">shipit.A1Client.prototype.</span>getDestination (shipment)](#apidoc.element.shipit.A1Client.prototype.getDestination)
1.  [function <span class="apidocSignatureSpan">shipit.A1Client.prototype.</span>getEta (shipment)](#apidoc.element.shipit.A1Client.prototype.getEta)
1.  [function <span class="apidocSignatureSpan">shipit.A1Client.prototype.</span>getService (shipment)](#apidoc.element.shipit.A1Client.prototype.getService)
1.  [function <span class="apidocSignatureSpan">shipit.A1Client.prototype.</span>getStatus (shipment)](#apidoc.element.shipit.A1Client.prototype.getStatus)
1.  [function <span class="apidocSignatureSpan">shipit.A1Client.prototype.</span>getWeight (shipment)](#apidoc.element.shipit.A1Client.prototype.getWeight)
1.  [function <span class="apidocSignatureSpan">shipit.A1Client.prototype.</span>presentAddress (address)](#apidoc.element.shipit.A1Client.prototype.presentAddress)
1.  [function <span class="apidocSignatureSpan">shipit.A1Client.prototype.</span>requestOptions (_arg)](#apidoc.element.shipit.A1Client.prototype.requestOptions)
1.  [function <span class="apidocSignatureSpan">shipit.A1Client.prototype.</span>validateResponse (response, cb)](#apidoc.element.shipit.A1Client.prototype.validateResponse)

#### [module shipit.AmazonClient](#apidoc.module.shipit.AmazonClient)
1.  [function <span class="apidocSignatureSpan">shipit.</span>AmazonClient (options)](#apidoc.element.shipit.AmazonClient.AmazonClient)
1.  object <span class="apidocSignatureSpan">shipit.AmazonClient.</span>STATUS_TYPES
1.  object <span class="apidocSignatureSpan">shipit.AmazonClient.</span>__super__

#### [module shipit.AmazonClient.prototype](#apidoc.module.shipit.AmazonClient.prototype)
1.  [function <span class="apidocSignatureSpan">shipit.AmazonClient.prototype.</span>constructor (options)](#apidoc.element.shipit.AmazonClient.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">shipit.AmazonClient.prototype.</span>getActivitiesAndStatus (data)](#apidoc.element.shipit.AmazonClient.prototype.getActivitiesAndStatus)
1.  [function <span class="apidocSignatureSpan">shipit.AmazonClient.prototype.</span>getDestination (data)](#apidoc.element.shipit.AmazonClient.prototype.getDestination)
1.  [function <span class="apidocSignatureSpan">shipit.AmazonClient.prototype.</span>getEta (data)](#apidoc.element.shipit.AmazonClient.prototype.getEta)
1.  [function <span class="apidocSignatureSpan">shipit.AmazonClient.prototype.</span>getService ()](#apidoc.element.shipit.AmazonClient.prototype.getService)
1.  [function <span class="apidocSignatureSpan">shipit.AmazonClient.prototype.</span>getWeight ()](#apidoc.element.shipit.AmazonClient.prototype.getWeight)
1.  [function <span class="apidocSignatureSpan">shipit.AmazonClient.prototype.</span>presentStatus (details)](#apidoc.element.shipit.AmazonClient.prototype.presentStatus)
1.  [function <span class="apidocSignatureSpan">shipit.AmazonClient.prototype.</span>requestOptions (_arg)](#apidoc.element.shipit.AmazonClient.prototype.requestOptions)
1.  [function <span class="apidocSignatureSpan">shipit.AmazonClient.prototype.</span>validateResponse (response, cb)](#apidoc.element.shipit.AmazonClient.prototype.validateResponse)

#### [module shipit.CanadaPostClient](#apidoc.module.shipit.CanadaPostClient)
1.  [function <span class="apidocSignatureSpan">shipit.</span>CanadaPostClient (_arg, options)](#apidoc.element.shipit.CanadaPostClient.CanadaPostClient)
1.  object <span class="apidocSignatureSpan">shipit.CanadaPostClient.</span>STATUS_TYPES
1.  object <span class="apidocSignatureSpan">shipit.CanadaPostClient.</span>__super__

#### [module shipit.CanadaPostClient.prototype](#apidoc.module.shipit.CanadaPostClient.prototype)
1.  [function <span class="apidocSignatureSpan">shipit.CanadaPostClient.prototype.</span>constructor (_arg, options)](#apidoc.element.shipit.CanadaPostClient.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">shipit.CanadaPostClient.prototype.</span>findStatusFromMap (statusText)](#apidoc.element.shipit.CanadaPostClient.prototype.findStatusFromMap)
1.  [function <span class="apidocSignatureSpan">shipit.CanadaPostClient.prototype.</span>getActivitiesAndStatus (shipment)](#apidoc.element.shipit.CanadaPostClient.prototype.getActivitiesAndStatus)
1.  [function <span class="apidocSignatureSpan">shipit.CanadaPostClient.prototype.</span>getDestination (shipment)](#apidoc.element.shipit.CanadaPostClient.prototype.getDestination)
1.  [function <span class="apidocSignatureSpan">shipit.CanadaPostClient.prototype.</span>getEta (shipment)](#apidoc.element.shipit.CanadaPostClient.prototype.getEta)
1.  [function <span class="apidocSignatureSpan">shipit.CanadaPostClient.prototype.</span>getService (shipment)](#apidoc.element.shipit.CanadaPostClient.prototype.getService)
1.  [function <span class="apidocSignatureSpan">shipit.CanadaPostClient.prototype.</span>getStatus (lastEvent)](#apidoc.element.shipit.CanadaPostClient.prototype.getStatus)
1.  [function <span class="apidocSignatureSpan">shipit.CanadaPostClient.prototype.</span>getWeight (shipment)](#apidoc.element.shipit.CanadaPostClient.prototype.getWeight)
1.  [function <span class="apidocSignatureSpan">shipit.CanadaPostClient.prototype.</span>requestOptions (_arg)](#apidoc.element.shipit.CanadaPostClient.prototype.requestOptions)
1.  [function <span class="apidocSignatureSpan">shipit.CanadaPostClient.prototype.</span>validateResponse (response, cb)](#apidoc.element.shipit.CanadaPostClient.prototype.validateResponse)

#### [module shipit.DhlClient](#apidoc.module.shipit.DhlClient)
1.  [function <span class="apidocSignatureSpan">shipit.</span>DhlClient (_arg, options)](#apidoc.element.shipit.DhlClient.DhlClient)
1.  object <span class="apidocSignatureSpan">shipit.DhlClient.</span>STATUS_TYPES
1.  object <span class="apidocSignatureSpan">shipit.DhlClient.</span>__super__

#### [module shipit.DhlClient.prototype](#apidoc.module.shipit.DhlClient.prototype)
1.  [function <span class="apidocSignatureSpan">shipit.DhlClient.prototype.</span>constructor (_arg, options)](#apidoc.element.shipit.DhlClient.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">shipit.DhlClient.prototype.</span>generateRequest (trk)](#apidoc.element.shipit.DhlClient.prototype.generateRequest)
1.  [function <span class="apidocSignatureSpan">shipit.DhlClient.prototype.</span>getActivitiesAndStatus (shipment)](#apidoc.element.shipit.DhlClient.prototype.getActivitiesAndStatus)
1.  [function <span class="apidocSignatureSpan">shipit.DhlClient.prototype.</span>getDestination (shipment)](#apidoc.element.shipit.DhlClient.prototype.getDestination)
1.  [function <span class="apidocSignatureSpan">shipit.DhlClient.prototype.</span>getEta (shipment)](#apidoc.element.shipit.DhlClient.prototype.getEta)
1.  [function <span class="apidocSignatureSpan">shipit.DhlClient.prototype.</span>getService (shipment)](#apidoc.element.shipit.DhlClient.prototype.getService)
1.  [function <span class="apidocSignatureSpan">shipit.DhlClient.prototype.</span>getWeight (shipment)](#apidoc.element.shipit.DhlClient.prototype.getWeight)
1.  [function <span class="apidocSignatureSpan">shipit.DhlClient.prototype.</span>presentAddress (rawAddress)](#apidoc.element.shipit.DhlClient.prototype.presentAddress)
1.  [function <span class="apidocSignatureSpan">shipit.DhlClient.prototype.</span>presentDetails (rawAddress, rawDetails)](#apidoc.element.shipit.DhlClient.prototype.presentDetails)
1.  [function <span class="apidocSignatureSpan">shipit.DhlClient.prototype.</span>presentStatus (status)](#apidoc.element.shipit.DhlClient.prototype.presentStatus)
1.  [function <span class="apidocSignatureSpan">shipit.DhlClient.prototype.</span>presentTimestamp (dateString, timeString)](#apidoc.element.shipit.DhlClient.prototype.presentTimestamp)
1.  [function <span class="apidocSignatureSpan">shipit.DhlClient.prototype.</span>requestOptions (_arg)](#apidoc.element.shipit.DhlClient.prototype.requestOptions)
1.  [function <span class="apidocSignatureSpan">shipit.DhlClient.prototype.</span>validateResponse (response, cb)](#apidoc.element.shipit.DhlClient.prototype.validateResponse)

#### [module shipit.DhlGmClient](#apidoc.module.shipit.DhlGmClient)
1.  [function <span class="apidocSignatureSpan">shipit.</span>DhlGmClient (options)](#apidoc.element.shipit.DhlGmClient.DhlGmClient)
1.  object <span class="apidocSignatureSpan">shipit.DhlGmClient.</span>STATUS_TYPES
1.  object <span class="apidocSignatureSpan">shipit.DhlGmClient.</span>__super__

#### [module shipit.DhlGmClient.prototype](#apidoc.module.shipit.DhlGmClient.prototype)
1.  [function <span class="apidocSignatureSpan">shipit.DhlGmClient.prototype.</span>constructor (options)](#apidoc.element.shipit.DhlGmClient.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">shipit.DhlGmClient.prototype.</span>extractHeaderField (data, name)](#apidoc.element.shipit.DhlGmClient.prototype.extractHeaderField)
1.  [function <span class="apidocSignatureSpan">shipit.DhlGmClient.prototype.</span>extractSummaryField (data, name)](#apidoc.element.shipit.DhlGmClient.prototype.extractSummaryField)
1.  [function <span class="apidocSignatureSpan">shipit.DhlGmClient.prototype.</span>getActivitiesAndStatus (data)](#apidoc.element.shipit.DhlGmClient.prototype.getActivitiesAndStatus)
1.  [function <span class="apidocSignatureSpan">shipit.DhlGmClient.prototype.</span>getDestination (data)](#apidoc.element.shipit.DhlGmClient.prototype.getDestination)
1.  [function <span class="apidocSignatureSpan">shipit.DhlGmClient.prototype.</span>getEta (data)](#apidoc.element.shipit.DhlGmClient.prototype.getEta)
1.  [function <span class="apidocSignatureSpan">shipit.DhlGmClient.prototype.</span>getService (data)](#apidoc.element.shipit.DhlGmClient.prototype.getService)
1.  [function <span class="apidocSignatureSpan">shipit.DhlGmClient.prototype.</span>getWeight (data)](#apidoc.element.shipit.DhlGmClient.prototype.getWeight)
1.  [function <span class="apidocSignatureSpan">shipit.DhlGmClient.prototype.</span>presentStatus (details)](#apidoc.element.shipit.DhlGmClient.prototype.presentStatus)
1.  [function <span class="apidocSignatureSpan">shipit.DhlGmClient.prototype.</span>requestOptions (_arg)](#apidoc.element.shipit.DhlGmClient.prototype.requestOptions)
1.  [function <span class="apidocSignatureSpan">shipit.DhlGmClient.prototype.</span>validateResponse (response, cb)](#apidoc.element.shipit.DhlGmClient.prototype.validateResponse)

#### [module shipit.FedexClient](#apidoc.module.shipit.FedexClient)
1.  [function <span class="apidocSignatureSpan">shipit.</span>FedexClient (_arg, options)](#apidoc.element.shipit.FedexClient.FedexClient)
1.  object <span class="apidocSignatureSpan">shipit.FedexClient.</span>STATUS_TYPES
1.  object <span class="apidocSignatureSpan">shipit.FedexClient.</span>__super__

#### [module shipit.FedexClient.prototype](#apidoc.module.shipit.FedexClient.prototype)
1.  [function <span class="apidocSignatureSpan">shipit.FedexClient.prototype.</span>constructor (_arg, options)](#apidoc.element.shipit.FedexClient.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">shipit.FedexClient.prototype.</span>generateRequest (trk, reference)](#apidoc.element.shipit.FedexClient.prototype.generateRequest)
1.  [function <span class="apidocSignatureSpan">shipit.FedexClient.prototype.</span>getActivitiesAndStatus (shipment)](#apidoc.element.shipit.FedexClient.prototype.getActivitiesAndStatus)
1.  [function <span class="apidocSignatureSpan">shipit.FedexClient.prototype.</span>getDestination (shipment)](#apidoc.element.shipit.FedexClient.prototype.getDestination)
1.  [function <span class="apidocSignatureSpan">shipit.FedexClient.prototype.</span>getEta (shipment)](#apidoc.element.shipit.FedexClient.prototype.getEta)
1.  [function <span class="apidocSignatureSpan">shipit.FedexClient.prototype.</span>getService (shipment)](#apidoc.element.shipit.FedexClient.prototype.getService)
1.  [function <span class="apidocSignatureSpan">shipit.FedexClient.prototype.</span>getStatus (shipment)](#apidoc.element.shipit.FedexClient.prototype.getStatus)
1.  [function <span class="apidocSignatureSpan">shipit.FedexClient.prototype.</span>getWeight (shipment)](#apidoc.element.shipit.FedexClient.prototype.getWeight)
1.  [function <span class="apidocSignatureSpan">shipit.FedexClient.prototype.</span>presentAddress (address)](#apidoc.element.shipit.FedexClient.prototype.presentAddress)
1.  [function <span class="apidocSignatureSpan">shipit.FedexClient.prototype.</span>requestOptions (_arg)](#apidoc.element.shipit.FedexClient.prototype.requestOptions)
1.  [function <span class="apidocSignatureSpan">shipit.FedexClient.prototype.</span>validateResponse (response, cb)](#apidoc.element.shipit.FedexClient.prototype.validateResponse)

#### [module shipit.LasershipClient](#apidoc.module.shipit.LasershipClient)
1.  [function <span class="apidocSignatureSpan">shipit.</span>LasershipClient (options)](#apidoc.element.shipit.LasershipClient.LasershipClient)
1.  object <span class="apidocSignatureSpan">shipit.LasershipClient.</span>STATUS_TYPES
1.  object <span class="apidocSignatureSpan">shipit.LasershipClient.</span>__super__

#### [module shipit.LasershipClient.prototype](#apidoc.module.shipit.LasershipClient.prototype)
1.  [function <span class="apidocSignatureSpan">shipit.LasershipClient.prototype.</span>constructor (options)](#apidoc.element.shipit.LasershipClient.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">shipit.LasershipClient.prototype.</span>getActivitiesAndStatus (shipment)](#apidoc.element.shipit.LasershipClient.prototype.getActivitiesAndStatus)
1.  [function <span class="apidocSignatureSpan">shipit.LasershipClient.prototype.</span>getDestination (shipment)](#apidoc.element.shipit.LasershipClient.prototype.getDestination)
1.  [function <span class="apidocSignatureSpan">shipit.LasershipClient.prototype.</span>getEta (shipment)](#apidoc.element.shipit.LasershipClient.prototype.getEta)
1.  [function <span class="apidocSignatureSpan">shipit.LasershipClient.prototype.</span>getService (shipment)](#apidoc.element.shipit.LasershipClient.prototype.getService)
1.  [function <span class="apidocSignatureSpan">shipit.LasershipClient.prototype.</span>getWeight (shipment)](#apidoc.element.shipit.LasershipClient.prototype.getWeight)
1.  [function <span class="apidocSignatureSpan">shipit.LasershipClient.prototype.</span>presentAddress (address)](#apidoc.element.shipit.LasershipClient.prototype.presentAddress)
1.  [function <span class="apidocSignatureSpan">shipit.LasershipClient.prototype.</span>presentStatus (eventType)](#apidoc.element.shipit.LasershipClient.prototype.presentStatus)
1.  [function <span class="apidocSignatureSpan">shipit.LasershipClient.prototype.</span>requestOptions (_arg)](#apidoc.element.shipit.LasershipClient.prototype.requestOptions)
1.  [function <span class="apidocSignatureSpan">shipit.LasershipClient.prototype.</span>validateResponse (response, cb)](#apidoc.element.shipit.LasershipClient.prototype.validateResponse)

#### [module shipit.OnTracClient](#apidoc.module.shipit.OnTracClient)
1.  [function <span class="apidocSignatureSpan">shipit.</span>OnTracClient (options)](#apidoc.element.shipit.OnTracClient.OnTracClient)
1.  object <span class="apidocSignatureSpan">shipit.OnTracClient.</span>STATUS_TYPES
1.  object <span class="apidocSignatureSpan">shipit.OnTracClient.</span>__super__

#### [module shipit.OnTracClient.prototype](#apidoc.module.shipit.OnTracClient.prototype)
1.  [function <span class="apidocSignatureSpan">shipit.OnTracClient.prototype.</span>constructor (options)](#apidoc.element.shipit.OnTracClient.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">shipit.OnTracClient.prototype.</span>extractSummaryField (shipment, name)](#apidoc.element.shipit.OnTracClient.prototype.extractSummaryField)
1.  [function <span class="apidocSignatureSpan">shipit.OnTracClient.prototype.</span>getActivitiesAndStatus (shipment)](#apidoc.element.shipit.OnTracClient.prototype.getActivitiesAndStatus)
1.  [function <span class="apidocSignatureSpan">shipit.OnTracClient.prototype.</span>getDestination (shipment)](#apidoc.element.shipit.OnTracClient.prototype.getDestination)
1.  [function <span class="apidocSignatureSpan">shipit.OnTracClient.prototype.</span>getEta (shipment)](#apidoc.element.shipit.OnTracClient.prototype.getEta)
1.  [function <span class="apidocSignatureSpan">shipit.OnTracClient.prototype.</span>getService (shipment)](#apidoc.element.shipit.OnTracClient.prototype.getService)
1.  [function <span class="apidocSignatureSpan">shipit.OnTracClient.prototype.</span>getWeight (shipment)](#apidoc.element.shipit.OnTracClient.prototype.getWeight)
1.  [function <span class="apidocSignatureSpan">shipit.OnTracClient.prototype.</span>presentAddress (location)](#apidoc.element.shipit.OnTracClient.prototype.presentAddress)
1.  [function <span class="apidocSignatureSpan">shipit.OnTracClient.prototype.</span>presentStatus (status)](#apidoc.element.shipit.OnTracClient.prototype.presentStatus)
1.  [function <span class="apidocSignatureSpan">shipit.OnTracClient.prototype.</span>presentTimestamp (ts)](#apidoc.element.shipit.OnTracClient.prototype.presentTimestamp)
1.  [function <span class="apidocSignatureSpan">shipit.OnTracClient.prototype.</span>requestOptions (_arg)](#apidoc.element.shipit.OnTracClient.prototype.requestOptions)
1.  [function <span class="apidocSignatureSpan">shipit.OnTracClient.prototype.</span>validateResponse (response, cb)](#apidoc.element.shipit.OnTracClient.prototype.validateResponse)

#### [module shipit.PrestigeClient](#apidoc.module.shipit.PrestigeClient)
1.  [function <span class="apidocSignatureSpan">shipit.</span>PrestigeClient (options)](#apidoc.element.shipit.PrestigeClient.PrestigeClient)
1.  object <span class="apidocSignatureSpan">shipit.PrestigeClient.</span>STATUS_TYPES
1.  object <span class="apidocSignatureSpan">shipit.PrestigeClient.</span>__super__

#### [module shipit.PrestigeClient.prototype](#apidoc.module.shipit.PrestigeClient.prototype)
1.  [function <span class="apidocSignatureSpan">shipit.PrestigeClient.prototype.</span>constructor (options)](#apidoc.element.shipit.PrestigeClient.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">shipit.PrestigeClient.prototype.</span>getActivitiesAndStatus (shipment)](#apidoc.element.shipit.PrestigeClient.prototype.getActivitiesAndStatus)
1.  [function <span class="apidocSignatureSpan">shipit.PrestigeClient.prototype.</span>getDestination (shipment)](#apidoc.element.shipit.PrestigeClient.prototype.getDestination)
1.  [function <span class="apidocSignatureSpan">shipit.PrestigeClient.prototype.</span>getEta (shipment)](#apidoc.element.shipit.PrestigeClient.prototype.getEta)
1.  [function <span class="apidocSignatureSpan">shipit.PrestigeClient.prototype.</span>getService (shipment)](#apidoc.element.shipit.PrestigeClient.prototype.getService)
1.  [function <span class="apidocSignatureSpan">shipit.PrestigeClient.prototype.</span>getWeight (shipment)](#apidoc.element.shipit.PrestigeClient.prototype.getWeight)
1.  [function <span class="apidocSignatureSpan">shipit.PrestigeClient.prototype.</span>presentAddress (prefix, event)](#apidoc.element.shipit.PrestigeClient.prototype.presentAddress)
1.  [function <span class="apidocSignatureSpan">shipit.PrestigeClient.prototype.</span>presentStatus (eventType)](#apidoc.element.shipit.PrestigeClient.prototype.presentStatus)
1.  [function <span class="apidocSignatureSpan">shipit.PrestigeClient.prototype.</span>requestOptions (_arg)](#apidoc.element.shipit.PrestigeClient.prototype.requestOptions)
1.  [function <span class="apidocSignatureSpan">shipit.PrestigeClient.prototype.</span>validateResponse (response, cb)](#apidoc.element.shipit.PrestigeClient.prototype.validateResponse)

#### [module shipit.UpsClient](#apidoc.module.shipit.UpsClient)
1.  [function <span class="apidocSignatureSpan">shipit.</span>UpsClient (_arg, options)](#apidoc.element.shipit.UpsClient.UpsClient)
1.  object <span class="apidocSignatureSpan">shipit.UpsClient.</span>STATUS_TYPES
1.  object <span class="apidocSignatureSpan">shipit.UpsClient.</span>__super__

#### [module shipit.UpsClient.prototype](#apidoc.module.shipit.UpsClient.prototype)
1.  [function <span class="apidocSignatureSpan">shipit.UpsClient.prototype.</span>constructor (_arg, options)](#apidoc.element.shipit.UpsClient.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">shipit.UpsClient.prototype.</span>generateRequest (trk, reference)](#apidoc.element.shipit.UpsClient.prototype.generateRequest)
1.  [function <span class="apidocSignatureSpan">shipit.UpsClient.prototype.</span>getActivitiesAndStatus (shipment)](#apidoc.element.shipit.UpsClient.prototype.getActivitiesAndStatus)
1.  [function <span class="apidocSignatureSpan">shipit.UpsClient.prototype.</span>getDestination (shipment)](#apidoc.element.shipit.UpsClient.prototype.getDestination)
1.  [function <span class="apidocSignatureSpan">shipit.UpsClient.prototype.</span>getEta (shipment)](#apidoc.element.shipit.UpsClient.prototype.getEta)
1.  [function <span class="apidocSignatureSpan">shipit.UpsClient.prototype.</span>getService (shipment)](#apidoc.element.shipit.UpsClient.prototype.getService)
1.  [function <span class="apidocSignatureSpan">shipit.UpsClient.prototype.</span>getWeight (shipment)](#apidoc.element.shipit.UpsClient.prototype.getWeight)
1.  [function <span class="apidocSignatureSpan">shipit.UpsClient.prototype.</span>presentAddress (rawAddress)](#apidoc.element.shipit.UpsClient.prototype.presentAddress)
1.  [function <span class="apidocSignatureSpan">shipit.UpsClient.prototype.</span>presentStatus (status)](#apidoc.element.shipit.UpsClient.prototype.presentStatus)
1.  [function <span class="apidocSignatureSpan">shipit.UpsClient.prototype.</span>presentTimestamp (dateString, timeString)](#apidoc.element.shipit.UpsClient.prototype.presentTimestamp)
1.  [function <span class="apidocSignatureSpan">shipit.UpsClient.prototype.</span>requestOptions (_arg)](#apidoc.element.shipit.UpsClient.prototype.requestOptions)
1.  [function <span class="apidocSignatureSpan">shipit.UpsClient.prototype.</span>validateResponse (response, cb)](#apidoc.element.shipit.UpsClient.prototype.validateResponse)

#### [module shipit.UpsMiClient](#apidoc.module.shipit.UpsMiClient)
1.  [function <span class="apidocSignatureSpan">shipit.</span>UpsMiClient (options)](#apidoc.element.shipit.UpsMiClient.UpsMiClient)
1.  object <span class="apidocSignatureSpan">shipit.UpsMiClient.</span>STATUS_TYPES
1.  object <span class="apidocSignatureSpan">shipit.UpsMiClient.</span>__super__

#### [module shipit.UpsMiClient.prototype](#apidoc.module.shipit.UpsMiClient.prototype)
1.  [function <span class="apidocSignatureSpan">shipit.UpsMiClient.prototype.</span>constructor (options)](#apidoc.element.shipit.UpsMiClient.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">shipit.UpsMiClient.prototype.</span>extractActivities ($, table)](#apidoc.element.shipit.UpsMiClient.prototype.extractActivities)
1.  [function <span class="apidocSignatureSpan">shipit.UpsMiClient.prototype.</span>extractSummaryField (data, name)](#apidoc.element.shipit.UpsMiClient.prototype.extractSummaryField)
1.  [function <span class="apidocSignatureSpan">shipit.UpsMiClient.prototype.</span>extractTimestamp (tsString)](#apidoc.element.shipit.UpsMiClient.prototype.extractTimestamp)
1.  [function <span class="apidocSignatureSpan">shipit.UpsMiClient.prototype.</span>getActivitiesAndStatus (data)](#apidoc.element.shipit.UpsMiClient.prototype.getActivitiesAndStatus)
1.  [function <span class="apidocSignatureSpan">shipit.UpsMiClient.prototype.</span>getDestination (data)](#apidoc.element.shipit.UpsMiClient.prototype.getDestination)
1.  [function <span class="apidocSignatureSpan">shipit.UpsMiClient.prototype.</span>getEta (data)](#apidoc.element.shipit.UpsMiClient.prototype.getEta)
1.  [function <span class="apidocSignatureSpan">shipit.UpsMiClient.prototype.</span>getService ()](#apidoc.element.shipit.UpsMiClient.prototype.getService)
1.  [function <span class="apidocSignatureSpan">shipit.UpsMiClient.prototype.</span>getWeight (data)](#apidoc.element.shipit.UpsMiClient.prototype.getWeight)
1.  [function <span class="apidocSignatureSpan">shipit.UpsMiClient.prototype.</span>presentStatus (details)](#apidoc.element.shipit.UpsMiClient.prototype.presentStatus)
1.  [function <span class="apidocSignatureSpan">shipit.UpsMiClient.prototype.</span>requestOptions (_arg)](#apidoc.element.shipit.UpsMiClient.prototype.requestOptions)
1.  [function <span class="apidocSignatureSpan">shipit.UpsMiClient.prototype.</span>validateResponse (response, cb)](#apidoc.element.shipit.UpsMiClient.prototype.validateResponse)

#### [module shipit.UspsClient](#apidoc.module.shipit.UspsClient)
1.  [function <span class="apidocSignatureSpan">shipit.</span>UspsClient (_arg, options)](#apidoc.element.shipit.UspsClient.UspsClient)
1.  object <span class="apidocSignatureSpan">shipit.UspsClient.</span>STATUS_TYPES
1.  object <span class="apidocSignatureSpan">shipit.UspsClient.</span>__super__

#### [module shipit.UspsClient.prototype](#apidoc.module.shipit.UspsClient.prototype)
1.  [function <span class="apidocSignatureSpan">shipit.UspsClient.prototype.</span>constructor (_arg, options)](#apidoc.element.shipit.UspsClient.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">shipit.UspsClient.prototype.</span>findStatusFromMap (statusText)](#apidoc.element.shipit.UspsClient.prototype.findStatusFromMap)
1.  [function <span class="apidocSignatureSpan">shipit.UspsClient.prototype.</span>generateRequest (trk, clientIp)](#apidoc.element.shipit.UspsClient.prototype.generateRequest)
1.  [function <span class="apidocSignatureSpan">shipit.UspsClient.prototype.</span>getActivitiesAndStatus (shipment)](#apidoc.element.shipit.UspsClient.prototype.getActivitiesAndStatus)
1.  [function <span class="apidocSignatureSpan">shipit.UspsClient.prototype.</span>getDestination (shipment)](#apidoc.element.shipit.UspsClient.prototype.getDestination)
1.  [function <span class="apidocSignatureSpan">shipit.UspsClient.prototype.</span>getEta (shipment)](#apidoc.element.shipit.UspsClient.prototype.getEta)
1.  [function <span class="apidocSignatureSpan">shipit.UspsClient.prototype.</span>getService (shipment)](#apidoc.element.shipit.UspsClient.prototype.getService)
1.  [function <span class="apidocSignatureSpan">shipit.UspsClient.prototype.</span>getStatus (shipment)](#apidoc.element.shipit.UspsClient.prototype.getStatus)
1.  [function <span class="apidocSignatureSpan">shipit.UspsClient.prototype.</span>getWeight (shipment)](#apidoc.element.shipit.UspsClient.prototype.getWeight)
1.  [function <span class="apidocSignatureSpan">shipit.UspsClient.prototype.</span>presentActivity (rawActivity)](#apidoc.element.shipit.UspsClient.prototype.presentActivity)
1.  [function <span class="apidocSignatureSpan">shipit.UspsClient.prototype.</span>presentStatus (status)](#apidoc.element.shipit.UspsClient.prototype.presentStatus)
1.  [function <span class="apidocSignatureSpan">shipit.UspsClient.prototype.</span>presentTimestamp (dateString, timeString)](#apidoc.element.shipit.UspsClient.prototype.presentTimestamp)
1.  [function <span class="apidocSignatureSpan">shipit.UspsClient.prototype.</span>requestOptions (_arg)](#apidoc.element.shipit.UspsClient.prototype.requestOptions)
1.  [function <span class="apidocSignatureSpan">shipit.UspsClient.prototype.</span>validateResponse (response, cb)](#apidoc.element.shipit.UspsClient.prototype.validateResponse)

#### [module shipit.a1](#apidoc.module.shipit.a1)
1.  [function <span class="apidocSignatureSpan">shipit.a1.</span>A1Client (options)](#apidoc.element.shipit.a1.A1Client)

#### [module shipit.amazon](#apidoc.module.shipit.amazon)
1.  [function <span class="apidocSignatureSpan">shipit.amazon.</span>AmazonClient (options)](#apidoc.element.shipit.amazon.AmazonClient)

#### [module shipit.canada_post](#apidoc.module.shipit.canada_post)
1.  [function <span class="apidocSignatureSpan">shipit.canada_post.</span>CanadaPostClient (_arg, options)](#apidoc.element.shipit.canada_post.CanadaPostClient)

#### [module shipit.dhl](#apidoc.module.shipit.dhl)
1.  [function <span class="apidocSignatureSpan">shipit.dhl.</span>DhlClient (_arg, options)](#apidoc.element.shipit.dhl.DhlClient)

#### [module shipit.dhlgm](#apidoc.module.shipit.dhlgm)
1.  [function <span class="apidocSignatureSpan">shipit.dhlgm.</span>DhlGmClient (options)](#apidoc.element.shipit.dhlgm.DhlGmClient)

#### [module shipit.fedex](#apidoc.module.shipit.fedex)
1.  [function <span class="apidocSignatureSpan">shipit.fedex.</span>FedexClient (_arg, options)](#apidoc.element.shipit.fedex.FedexClient)

#### [module shipit.lasership](#apidoc.module.shipit.lasership)
1.  [function <span class="apidocSignatureSpan">shipit.lasership.</span>LasershipClient (options)](#apidoc.element.shipit.lasership.LasershipClient)

#### [module shipit.ontrac](#apidoc.module.shipit.ontrac)
1.  [function <span class="apidocSignatureSpan">shipit.ontrac.</span>OnTracClient (options)](#apidoc.element.shipit.ontrac.OnTracClient)

#### [module shipit.prestige](#apidoc.module.shipit.prestige)
1.  [function <span class="apidocSignatureSpan">shipit.prestige.</span>PrestigeClient (options)](#apidoc.element.shipit.prestige.PrestigeClient)

#### [module shipit.shipper](#apidoc.module.shipit.shipper)
1.  [function <span class="apidocSignatureSpan">shipit.shipper.</span>ShipperClient ()](#apidoc.element.shipit.shipper.ShipperClient)

#### [module shipit.ups](#apidoc.module.shipit.ups)
1.  [function <span class="apidocSignatureSpan">shipit.ups.</span>UpsClient (_arg, options)](#apidoc.element.shipit.ups.UpsClient)

#### [module shipit.upsmi](#apidoc.module.shipit.upsmi)
1.  [function <span class="apidocSignatureSpan">shipit.upsmi.</span>UpsMiClient (options)](#apidoc.element.shipit.upsmi.UpsMiClient)

#### [module shipit.usps](#apidoc.module.shipit.usps)
1.  [function <span class="apidocSignatureSpan">shipit.usps.</span>UspsClient (_arg, options)](#apidoc.element.shipit.usps.UspsClient)



# <a name="apidoc.module.shipit"></a>[module shipit](#apidoc.module.shipit)

#### <a name="apidoc.element.shipit.A1Client"></a>[function <span class="apidocSignatureSpan">shipit.</span>A1Client (options)](#apidoc.element.shipit.A1Client)
- description and source-code
```javascript
function A1Client(options) {
  this.options = options;
  A1Client.__super__.constructor.apply(this, arguments);
  this.parser = new Parser();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.shipit.AmazonClient"></a>[function <span class="apidocSignatureSpan">shipit.</span>AmazonClient (options)](#apidoc.element.shipit.AmazonClient)
- description and source-code
```javascript
function AmazonClient(options) {
  this.options = options;
  STATUS_MAP[ShipperClient.STATUS_TYPES.DELAYED] = ['delivery attempted'];
  STATUS_MAP[ShipperClient.STATUS_TYPES.DELIVERED] = ['delivered'];
  STATUS_MAP[ShipperClient.STATUS_TYPES.OUT_FOR_DELIVERY] = ['out for delivery'];
  STATUS_MAP[ShipperClient.STATUS_TYPES.SHIPPING] = ['in transit to carrier', 'shipping soon'];
  STATUS_MAP[ShipperClient.STATUS_TYPES.EN_ROUTE] = ['on the way', 'package arrived', 'package received', 'shipment departed', '
shipment arrived'];
  DAYS_OF_THE_WEEK['SUNDAY'] = 0;
  DAYS_OF_THE_WEEK['MONDAY'] = 1;
  DAYS_OF_THE_WEEK['TUESDAY'] = 2;
  DAYS_OF_THE_WEEK['WEDNESDAY'] = 3;
  DAYS_OF_THE_WEEK['THURSDAY'] = 4;
  DAYS_OF_THE_WEEK['FRIDAY'] = 5;
  DAYS_OF_THE_WEEK['SATURDAY'] = 6;
  AmazonClient.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.shipit.CanadaPostClient"></a>[function <span class="apidocSignatureSpan">shipit.</span>CanadaPostClient (_arg, options)](#apidoc.element.shipit.CanadaPostClient)
- description and source-code
```javascript
function CanadaPostClient(_arg, options) {
  this.username = _arg.username, this.password = _arg.password;
  this.options = options;
  CanadaPostClient.__super__.constructor.apply(this, arguments);
  this.parser = new Parser();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.shipit.DhlClient"></a>[function <span class="apidocSignatureSpan">shipit.</span>DhlClient (_arg, options)](#apidoc.element.shipit.DhlClient)
- description and source-code
```javascript
function DhlClient(_arg, options) {
  this.userId = _arg.userId, this.password = _arg.password;
  this.options = options;
  DhlClient.__super__.constructor.apply(this, arguments);
  this.parser = new Parser();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.shipit.DhlGmClient"></a>[function <span class="apidocSignatureSpan">shipit.</span>DhlGmClient (options)](#apidoc.element.shipit.DhlGmClient)
- description and source-code
```javascript
function DhlGmClient(options) {
  this.options = options;
  STATUS_MAP[ShipperClient.STATUS_TYPES.DELIVERED] = ['delivered'];
  STATUS_MAP[ShipperClient.STATUS_TYPES.EN_ROUTE] = ['transferred', 'cleared', 'received', 'processed', 'sorted', 'sorting complete
', 'arrival', 'tendered'];
  STATUS_MAP[ShipperClient.STATUS_TYPES.OUT_FOR_DELIVERY] = ['out for delivery'];
  STATUS_MAP[ShipperClient.STATUS_TYPES.SHIPPING] = ['electronic notification received'];
  DhlGmClient.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.shipit.FedexClient"></a>[function <span class="apidocSignatureSpan">shipit.</span>FedexClient (_arg, options)](#apidoc.element.shipit.FedexClient)
- description and source-code
```javascript
function FedexClient(_arg, options) {
  this.key = _arg.key, this.password = _arg.password, this.account = _arg.account, this.meter = _arg.meter;
  this.options = options;
  FedexClient.__super__.constructor.apply(this, arguments);
  this.parser = new Parser();
  this.builder = new Builder({
    renderOpts: {
      pretty: false
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.shipit.LasershipClient"></a>[function <span class="apidocSignatureSpan">shipit.</span>LasershipClient (options)](#apidoc.element.shipit.LasershipClient)
- description and source-code
```javascript
function LasershipClient(options) {
  this.options = options;
  LasershipClient.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.shipit.OnTracClient"></a>[function <span class="apidocSignatureSpan">shipit.</span>OnTracClient (options)](#apidoc.element.shipit.OnTracClient)
- description and source-code
```javascript
function OnTracClient(options) {
  this.options = options;
  OnTracClient.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.shipit.PrestigeClient"></a>[function <span class="apidocSignatureSpan">shipit.</span>PrestigeClient (options)](#apidoc.element.shipit.PrestigeClient)
- description and source-code
```javascript
function PrestigeClient(options) {
  this.options = options;
  PrestigeClient.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.shipit.UpsClient"></a>[function <span class="apidocSignatureSpan">shipit.</span>UpsClient (_arg, options)](#apidoc.element.shipit.UpsClient)
- description and source-code
```javascript
function UpsClient(_arg, options) {
  this.licenseNumber = _arg.licenseNumber, this.userId = _arg.userId, this.password = _arg.password;
  this.options = options;
  UpsClient.__super__.constructor.apply(this, arguments);
  this.parser = new Parser();
  this.builder = new Builder({
    renderOpts: {
      pretty: false
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.shipit.UpsMiClient"></a>[function <span class="apidocSignatureSpan">shipit.</span>UpsMiClient (options)](#apidoc.element.shipit.UpsMiClient)
- description and source-code
```javascript
function UpsMiClient(options) {
  this.options = options;
  STATUS_MAP[ShipperClient.STATUS_TYPES.DELIVERED] = ['delivered'];
  STATUS_MAP[ShipperClient.STATUS_TYPES.EN_ROUTE] = ['transferred', 'received', 'processed', 'sorted', 'post office entry'];
  STATUS_MAP[ShipperClient.STATUS_TYPES.OUT_FOR_DELIVERY] = ['out for post office delivery'];
  STATUS_MAP[ShipperClient.STATUS_TYPES.SHIPPING] = ['shipment information received'];
  UpsMiClient.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.shipit.UspsClient"></a>[function <span class="apidocSignatureSpan">shipit.</span>UspsClient (_arg, options)](#apidoc.element.shipit.UspsClient)
- description and source-code
```javascript
function UspsClient(_arg, options) {
  this.userId = _arg.userId;
  this.options = options;
  UspsClient.__super__.constructor.apply(this, arguments);
  this.parser = new Parser();
  this.builder = new Builder({
    renderOpts: {
      pretty: false
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.shipit.guessCarrier"></a>[function <span class="apidocSignatureSpan">shipit.</span>guessCarrier (trk)](#apidoc.element.shipit.guessCarrier)
- description and source-code
```javascript
guessCarrier = function (trk) {
  var carriers;
  carriers = [];
  trk = _preprocess(trk);
  CARRIERS.every(function(c) {
    var good, stop, _ref;
    if (trk.match(c.regex)) {
      if (c.confirm != null) {
        _ref = c.confirm(trk), good = _ref[0], stop = _ref[1];
        if (good) {
          carriers.push(c.name);
        }
        return !stop;
      }
      carriers.push(c.name);
      return true;
    }
    return true;
  });
  return uniq(carriers);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.shipit.A1Client"></a>[module shipit.A1Client](#apidoc.module.shipit.A1Client)

#### <a name="apidoc.element.shipit.A1Client.A1Client"></a>[function <span class="apidocSignatureSpan">shipit.</span>A1Client (options)](#apidoc.element.shipit.A1Client.A1Client)
- description and source-code
```javascript
function A1Client(options) {
  this.options = options;
  A1Client.__super__.constructor.apply(this, arguments);
  this.parser = new Parser();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.shipit.A1Client.__super__"></a>[module shipit.A1Client.__super__](#apidoc.module.shipit.A1Client.__super__)

#### <a name="apidoc.element.shipit.A1Client.__super__.presentLocation"></a>[function <span class="apidocSignatureSpan">shipit.A1Client.__super__.</span>presentLocation (_arg)](#apidoc.element.shipit.A1Client.__super__.presentLocation)
- description and source-code
```javascript
presentLocation = function (_arg) {
  var address, city, countryCode, postalCode, stateCode;
  city = _arg.city, stateCode = _arg.stateCode, countryCode = _arg.countryCode, postalCode = _arg.postalCode;
  if (city != null ? city.length : void 0) {
    city = titleCase(city);
  }
  if (stateCode != null ? stateCode.length : void 0) {
    stateCode = stateCode.trim();
    if (stateCode.length > 3) {
      stateCode = titleCase(stateCode);
    }
    if (city != null ? city.length : void 0) {
      city = city.trim();
      address = "" + city + ", " + stateCode;
    } else {
      address = stateCode;
    }
  } else {
    address = city;
  }
  postalCode = this.presentPostalCode(postalCode);
  if (countryCode != null ? countryCode.length : void 0) {
    countryCode = countryCode.trim();
    if (countryCode.length > 3) {
      countryCode = titleCase(countryCode);
    }
    if (address != null ? address.length : void 0) {
      address = countryCode !== 'US' ? "" + address + ", " + countryCode : address;
    } else {
      address = countryCode;
    }
  }
  if (postalCode != null ? postalCode.length : void 0) {
    address = address != null ? "" + address + " " + postalCode : postalCode;
  }
  return address;
}
```
- example usage
```shell
...
  if (address == null) {
    return;
  }
  city = (_ref = address['City']) != null ? _ref[0] : void 0;
  stateCode = (_ref1 = address['StateProvince']) != null ? _ref1[0] : void 0;
  countryCode = (_ref2 = address['CountryCode']) != null ? _ref2[0] : void 0;
  postalCode = (_ref3 = address['PostalCode']) != null ? _ref3[0] : void 0;
  return this.presentLocation({
    city: city,
    stateCode: stateCode,
    countryCode: countryCode,
    postalCode: postalCode
  });
};
...
```

#### <a name="apidoc.element.shipit.A1Client.__super__.presentLocationString"></a>[function <span class="apidocSignatureSpan">shipit.A1Client.__super__.</span>presentLocationString (location)](#apidoc.element.shipit.A1Client.__super__.presentLocationString)
- description and source-code
```javascript
presentLocationString = function (location) {
  var field, newFields, _i, _len, _ref;
  newFields = [];
  _ref = (location != null ? location.split(',') : void 0) || [];
  for (_i = 0, _len = _ref.length; _i < _len; _i++) {
    field = _ref[_i];
    field = field.trim();
    if (field.length > 2) {
      field = titleCase(field);
    }
    newFields.push(field);
  }
  return newFields.join(', ');
}
```
- example usage
```shell
...
  var $, dest, rightNow;
  if (data == null) {
    return;
  }
  $ = data.$, rightNow = data.rightNow;
  dest = $(".delivery-address").text();
  if (dest != null ? dest.length : void 0) {
    return this.presentLocationString(dest);
  }
};

AmazonClient.prototype.getEta = function(data) {
  var $, container, dateComponent, dateComponentStr, deliveryStatus, etaDayVal, etaString, matches, nowDayVal, numDays, rightNow
, timeComponent, _ref1, _ref2;
  if (data == null) {
    return;
...
```

#### <a name="apidoc.element.shipit.A1Client.__super__.presentPostalCode"></a>[function <span class="apidocSignatureSpan">shipit.A1Client.__super__.</span>presentPostalCode (rawCode)](#apidoc.element.shipit.A1Client.__super__.presentPostalCode)
- description and source-code
```javascript
presentPostalCode = function (rawCode) {
  rawCode = rawCode != null ? rawCode.trim() : void 0;
  if (/^\d{9}$/.test(rawCode)) {
    return "" + rawCode.slice(0, 5) + "-" + rawCode.slice(5);
  } else {
    return rawCode;
  }
}
```
- example usage
```shell
...
    address = "" + city + ", " + stateCode;
  } else {
    address = stateCode;
  }
} else {
  address = city;
}
postalCode = this.presentPostalCode(postalCode);
if (countryCode != null ? countryCode.length : void 0) {
  countryCode = countryCode.trim();
  if (countryCode.length > 3) {
    countryCode = titleCase(countryCode);
  }
  if (address != null ? address.length : void 0) {
    address = countryCode !== 'US' ? "" + address + ", " + countryCode : address;
...
```

#### <a name="apidoc.element.shipit.A1Client.__super__.presentResponse"></a>[function <span class="apidocSignatureSpan">shipit.A1Client.__super__.</span>presentResponse (response, requestData, cb)](#apidoc.element.shipit.A1Client.__super__.presentResponse)
- description and source-code
```javascript
presentResponse = function (response, requestData, cb) {
  return this.validateResponse(response, (function(_this) {
    return function(err, shipment) {
      var activities, adjustedEta, eta, presentedResponse, status, _ref, _ref1;
      if ((err != null) || (shipment == null)) {
        return cb(err);
      }
      _ref = _this.getActivitiesAndStatus(shipment), activities = _ref.activities, status = _ref.status;
      eta = _this.getEta(shipment);
      if (eta != null) {
        adjustedEta = moment(eta).utc().format().replace(/T00:00:00/, 'T23:59:59');
      }
      if (adjustedEta != null) {
        adjustedEta = moment(adjustedEta).toDate();
      }
      presentedResponse = {
        eta: adjustedEta,
        service: _this.getService(shipment),
        weight: _this.getWeight(shipment),
        destination: _this.getDestination(shipment),
        activities: activities,
        status: status
      };
      if ((requestData != null ? requestData.raw : void 0) != null) {
        if (requestData.raw) {
          presentedResponse.raw = response;
        }
      } else {
        if ((_ref1 = _this.options) != null ? _ref1.raw : void 0) {
          presentedResponse.raw = response;
        }
      }
      presentedResponse.request = requestData;
      return cb(null, presentedResponse);
    };
  })(this));
}
```
- example usage
```shell
...
      return function(err, response, body) {
        if ((body == null) || (err != null)) {
          return cb(err);
        }
        if (response.statusCode !== 200) {
          return cb("response status " + response.statusCode);
        }
        return _this.presentResponse(body, requestData, cb);
      };
    })(this));
  };

  return ShipperClient;

})();
...
```

#### <a name="apidoc.element.shipit.A1Client.__super__.requestData"></a>[function <span class="apidocSignatureSpan">shipit.A1Client.__super__.</span>requestData (requestData, cb)](#apidoc.element.shipit.A1Client.__super__.requestData)
- description and source-code
```javascript
requestData = function (requestData, cb) {
  var opts, _ref;
  opts = this.requestOptions(requestData);
  opts.timeout = (requestData != null ? requestData.timeout : void 0) || ((_ref = this.options) != null ? _ref.timeout : void 0);
  return request(opts, (function(_this) {
    return function(err, response, body) {
      if ((body == null) || (err != null)) {
        return cb(err);
      }
      if (response.statusCode !== 200) {
        return cb("response status " + response.statusCode);
      }
      return _this.presentResponse(body, requestData, cb);
    };
  })(this));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.shipit.A1Client.prototype"></a>[module shipit.A1Client.prototype](#apidoc.module.shipit.A1Client.prototype)

#### <a name="apidoc.element.shipit.A1Client.prototype.constructor"></a>[function <span class="apidocSignatureSpan">shipit.A1Client.prototype.</span>constructor (options)](#apidoc.element.shipit.A1Client.prototype.constructor)
- description and source-code
```javascript
function A1Client(options) {
  this.options = options;
  A1Client.__super__.constructor.apply(this, arguments);
  this.parser = new Parser();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.shipit.A1Client.prototype.getActivitiesAndStatus"></a>[function <span class="apidocSignatureSpan">shipit.A1Client.prototype.</span>getActivitiesAndStatus (shipment)](#apidoc.element.shipit.A1Client.prototype.getActivitiesAndStatus)
- description and source-code
```javascript
getActivitiesAndStatus = function (shipment) {
  var activities, activity, datetime, details, event_time, location, rawActivities, rawActivity, raw_timestamp, status, timestamp
, _i, _len, _ref, _ref1, _ref2, _ref3, _ref4;
  activities = [];
  status = null;
  rawActivities = (_ref = shipment['TrackingEventHistory']) != null ? (_ref1 = _ref[0]) != null ? _ref1['TrackingEventDetail'] :
void 0 : void 0;
  _ref2 = rawActivities || [];
  for (_i = 0, _len = _ref2.length; _i < _len; _i++) {
    rawActivity = _ref2[_i];
    location = this.presentAddress(rawActivity != null ? (_ref3 = rawActivity['EventLocation']) != null ? _ref3[0] : void 0 : void
 0);
    raw_timestamp = rawActivity != null ? rawActivity['EventDateTime'][0] : void 0;
    if (raw_timestamp != null) {
      event_time = moment(raw_timestamp);
      timestamp = event_time.toDate();
      datetime = raw_timestamp.slice(0, 19);
    }
    details = rawActivity != null ? (_ref4 = rawActivity['EventCodeDesc']) != null ? _ref4[0] : void 0 : void 0;
    if ((details != null) && (timestamp != null)) {
      activity = {
        timestamp: timestamp,
        datetime: datetime,
        location: location,
        details: details
      };
      activities.push(activity);
    }
  }
  return {
    activities: activities,
    status: this.getStatus(shipment)
  };
}
```
- example usage
```shell
...
    ShipperClient.prototype.presentResponse = function(response, requestData, cb) {
return this.validateResponse(response, (function(_this) {
  return function(err, shipment) {
    var activities, adjustedEta, eta, presentedResponse, status, _ref, _ref1;
    if ((err != null) || (shipment == null)) {
      return cb(err);
    }
    _ref = _this.getActivitiesAndStatus(shipment), activities = _ref.activities, status = _ref.status;
    eta = _this.getEta(shipment);
    if (eta != null) {
      adjustedEta = moment(eta).utc().format().replace(/T00:00:00/, 'T23:59:59');
    }
    if (adjustedEta != null) {
      adjustedEta = moment(adjustedEta).toDate();
    }
...
```

#### <a name="apidoc.element.shipit.A1Client.prototype.getDestination"></a>[function <span class="apidocSignatureSpan">shipit.A1Client.prototype.</span>getDestination (shipment)](#apidoc.element.shipit.A1Client.prototype.getDestination)
- description and source-code
```javascript
getDestination = function (shipment) {
  var _ref;
  return this.presentAddress(shipment != null ? (_ref = shipment['PackageDestinationLocation']) != null ? _ref[0] : void 0 : void
 0);
}
```
- example usage
```shell
...
if (adjustedEta != null) {
  adjustedEta = moment(adjustedEta).toDate();
}
presentedResponse = {
  eta: adjustedEta,
  service: _this.getService(shipment),
  weight: _this.getWeight(shipment),
  destination: _this.getDestination(shipment),
  activities: activities,
  status: status
};
if ((requestData != null ? requestData.raw : void 0) != null) {
  if (requestData.raw) {
    presentedResponse.raw = response;
  }
...
```

#### <a name="apidoc.element.shipit.A1Client.prototype.getEta"></a>[function <span class="apidocSignatureSpan">shipit.A1Client.prototype.</span>getEta (shipment)](#apidoc.element.shipit.A1Client.prototype.getEta)
- description and source-code
```javascript
getEta = function (shipment) {
  var activities, firstActivity, _ref, _ref1, _ref2, _ref3;
  activities = ((_ref = shipment['TrackingEventHistory']) != null ? (_ref1 = _ref[0]) != null ? _ref1['TrackingEventDetail'] : void
 0 : void 0) || [];
  firstActivity = activities[activities.length - 1];
  if ((firstActivity != null ? (_ref2 = firstActivity['EstimatedDeliveryDate']) != null ? _ref2[0] : void 0 : void 0) == null) {
    return;
  }
  return moment("" + (firstActivity != null ? (_ref3 = firstActivity['EstimatedDeliveryDate']) != null ? _ref3[0] : void 0 : void
 0) + "T00:00:00Z").toDate();
}
```
- example usage
```shell
...
      return this.validateResponse(response, (function(_this) {
return function(err, shipment) {
  var activities, adjustedEta, eta, presentedResponse, status, _ref, _ref1;
  if ((err != null) || (shipment == null)) {
    return cb(err);
  }
  _ref = _this.getActivitiesAndStatus(shipment), activities = _ref.activities, status = _ref.status;
  eta = _this.getEta(shipment);
  if (eta != null) {
    adjustedEta = moment(eta).utc().format().replace(/T00:00:00/, 'T23:59:59');
  }
  if (adjustedEta != null) {
    adjustedEta = moment(adjustedEta).toDate();
  }
  presentedResponse = {
...
```

#### <a name="apidoc.element.shipit.A1Client.prototype.getService"></a>[function <span class="apidocSignatureSpan">shipit.A1Client.prototype.</span>getService (shipment)](#apidoc.element.shipit.A1Client.prototype.getService)
- description and source-code
```javascript
getService = function (shipment) {
  return null;
}
```
- example usage
```shell
...
  adjustedEta = moment(eta).utc().format().replace(/T00:00:00/, 'T23:59:59');
}
if (adjustedEta != null) {
  adjustedEta = moment(adjustedEta).toDate();
}
presentedResponse = {
  eta: adjustedEta,
  service: _this.getService(shipment),
  weight: _this.getWeight(shipment),
  destination: _this.getDestination(shipment),
  activities: activities,
  status: status
};
if ((requestData != null ? requestData.raw : void 0) != null) {
  if (requestData.raw) {
...
```

#### <a name="apidoc.element.shipit.A1Client.prototype.getStatus"></a>[function <span class="apidocSignatureSpan">shipit.A1Client.prototype.</span>getStatus (shipment)](#apidoc.element.shipit.A1Client.prototype.getStatus)
- description and source-code
```javascript
getStatus = function (shipment) {
  var code, lastActivity, statusCode, _ref, _ref1, _ref2, _ref3, _ref4;
  lastActivity = (_ref = shipment['TrackingEventHistory']) != null ? (_ref1 = _ref[0]) != null ? (_ref2 = _ref1['TrackingEventDetail
']) != null ? _ref2[0] : void 0 : void 0 : void 0;
  statusCode = lastActivity != null ? (_ref3 = lastActivity['EventCode']) != null ? _ref3[0] : void 0 : void 0;
  if (statusCode == null) {
    return;
  }
  code = parseInt((_ref4 = statusCode.match(/EVENT_(.*)$/)) != null ? _ref4[1] : void 0);
  if (isNaN(code)) {
    return;
  }
  if (STATUS_MAP[code] != null) {
    return STATUS_MAP[code];
  } else {
    if (code < 300) {
      return ShipperClient.STATUS_TYPES.EN_ROUTE;
    } else {
      return ShipperClient.STATUS_TYPES.UNKNOWN;
    }
  }
}
```
- example usage
```shell
...
        details: details
      };
      activities.push(activity);
    }
  }
  return {
    activities: activities,
    status: this.getStatus(shipment)
  };
};

A1Client.prototype.getEta = function(shipment) {
  var activities, firstActivity, _ref, _ref1, _ref2, _ref3;
  activities = ((_ref = shipment['TrackingEventHistory']) != null ? (_ref1 = _ref[0]) != null ? _ref1['TrackingEventDetail'] : void
 0 : void 0) || [];
  firstActivity = activities[activities.length - 1];
...
```

#### <a name="apidoc.element.shipit.A1Client.prototype.getWeight"></a>[function <span class="apidocSignatureSpan">shipit.A1Client.prototype.</span>getWeight (shipment)](#apidoc.element.shipit.A1Client.prototype.getWeight)
- description and source-code
```javascript
getWeight = function (shipment) {
  return null;
}
```
- example usage
```shell
...
}
if (adjustedEta != null) {
  adjustedEta = moment(adjustedEta).toDate();
}
presentedResponse = {
  eta: adjustedEta,
  service: _this.getService(shipment),
  weight: _this.getWeight(shipment),
  destination: _this.getDestination(shipment),
  activities: activities,
  status: status
};
if ((requestData != null ? requestData.raw : void 0) != null) {
  if (requestData.raw) {
    presentedResponse.raw = response;
...
```

#### <a name="apidoc.element.shipit.A1Client.prototype.presentAddress"></a>[function <span class="apidocSignatureSpan">shipit.A1Client.prototype.</span>presentAddress (address)](#apidoc.element.shipit.A1Client.prototype.presentAddress)
- description and source-code
```javascript
presentAddress = function (address) {
  var city, countryCode, postalCode, stateCode, _ref, _ref1, _ref2, _ref3;
  if (address == null) {
    return;
  }
  city = (_ref = address['City']) != null ? _ref[0] : void 0;
  stateCode = (_ref1 = address['StateProvince']) != null ? _ref1[0] : void 0;
  countryCode = (_ref2 = address['CountryCode']) != null ? _ref2[0] : void 0;
  postalCode = (_ref3 = address['PostalCode']) != null ? _ref3[0] : void 0;
  return this.presentLocation({
    city: city,
    stateCode: stateCode,
    countryCode: countryCode,
    postalCode: postalCode
  });
}
```
- example usage
```shell
...
var activities, activity, datetime, details, event_time, location, rawActivities, rawActivity, raw_timestamp, status, timestamp,
_i, _len, _ref, _ref1, _ref2, _ref3, _ref4;
activities = [];
status = null;
rawActivities = (_ref = shipment['TrackingEventHistory']) != null ? (_ref1 = _ref[0]) != null ? _ref1['TrackingEventDetail'] : void
 0 : void 0;
_ref2 = rawActivities || [];
for (_i = 0, _len = _ref2.length; _i < _len; _i++) {
  rawActivity = _ref2[_i];
  location = this.presentAddress(rawActivity != null ? (_ref3 = rawActivity['EventLocation']) != null ? _ref3[0] : void 0 : void
 0);
  raw_timestamp = rawActivity != null ? rawActivity['EventDateTime'][0] : void 0;
  if (raw_timestamp != null) {
    event_time = moment(raw_timestamp);
    timestamp = event_time.toDate();
    datetime = raw_timestamp.slice(0, 19);
  }
  details = rawActivity != null ? (_ref4 = rawActivity['EventCodeDesc']) != null ? _ref4[0] : void 0 : void 0;
...
```

#### <a name="apidoc.element.shipit.A1Client.prototype.requestOptions"></a>[function <span class="apidocSignatureSpan">shipit.A1Client.prototype.</span>requestOptions (_arg)](#apidoc.element.shipit.A1Client.prototype.requestOptions)
- description and source-code
```javascript
requestOptions = function (_arg) {
  var trackingNumber;
  trackingNumber = _arg.trackingNumber;
  return {
    method: 'GET',
    uri: "http://www.aoneonline.com/pages/customers/trackingrequest.php?tracking_number=" + trackingNumber
  };
}
```
- example usage
```shell
...
      return cb(null, presentedResponse);
    };
  })(this));
};

ShipperClient.prototype.requestData = function(requestData, cb) {
  var opts, _ref;
  opts = this.requestOptions(requestData);
  opts.timeout = (requestData != null ? requestData.timeout : void 0) || ((_ref = this.options) != null ? _ref.timeout : void 0);
  return request(opts, (function(_this) {
    return function(err, response, body) {
      if ((body == null) || (err != null)) {
        return cb(err);
      }
      if (response.statusCode !== 200) {
...
```

#### <a name="apidoc.element.shipit.A1Client.prototype.validateResponse"></a>[function <span class="apidocSignatureSpan">shipit.A1Client.prototype.</span>validateResponse (response, cb)](#apidoc.element.shipit.A1Client.prototype.validateResponse)
- description and source-code
```javascript
validateResponse = function (response, cb) {
  var handleResponse;
  handleResponse = function(xmlErr, trackResult) {
    var error, errorInfo, trackingInfo, _ref, _ref1, _ref2, _ref3, _ref4, _ref5, _ref6;
    if ((xmlErr != null) || (trackResult == null)) {
      return cb(xmlErr);
    }
    trackingInfo = (_ref = trackResult['AmazonTrackingResponse']) != null ? (_ref1 = _ref['PackageTrackingInfo']) != null ? _ref1
[0] : void 0 : void 0;
    if ((trackingInfo != null ? trackingInfo['TrackingNumber'] : void 0) == null) {
      errorInfo = (_ref2 = trackResult['AmazonTrackingResponse']) != null ? (_ref3 = _ref2['TrackingErrorInfo']) != null ? _ref3
[0] : void 0 : void 0;
      error = errorInfo != null ? (_ref4 = errorInfo['TrackingErrorDetail']) != null ? (_ref5 = _ref4[0]) != null ? (_ref6 = _ref5
['ErrorDetailCodeDesc']) != null ? _ref6[0] : void 0 : void 0 : void 0 : void 0;
      if (error != null) {
        return cb(error);
      }
      cb('unknown error');
    }
    return cb(null, trackingInfo);
  };
  this.parser.reset();
  return this.parser.parseString(response, handleResponse);
}
```
- example usage
```shell
...
  if (postalCode != null ? postalCode.length : void 0) {
    address = address != null ? "" + address + " " + postalCode : postalCode;
  }
  return address;
};

ShipperClient.prototype.presentResponse = function(response, requestData, cb) {
  return this.validateResponse(response, (function(_this) {
    return function(err, shipment) {
      var activities, adjustedEta, eta, presentedResponse, status, _ref, _ref1;
      if ((err != null) || (shipment == null)) {
        return cb(err);
      }
      _ref = _this.getActivitiesAndStatus(shipment), activities = _ref.activities, status = _ref.status;
      eta = _this.getEta(shipment);
...
```



# <a name="apidoc.module.shipit.AmazonClient"></a>[module shipit.AmazonClient](#apidoc.module.shipit.AmazonClient)

#### <a name="apidoc.element.shipit.AmazonClient.AmazonClient"></a>[function <span class="apidocSignatureSpan">shipit.</span>AmazonClient (options)](#apidoc.element.shipit.AmazonClient.AmazonClient)
- description and source-code
```javascript
function AmazonClient(options) {
  this.options = options;
  STATUS_MAP[ShipperClient.STATUS_TYPES.DELAYED] = ['delivery attempted'];
  STATUS_MAP[ShipperClient.STATUS_TYPES.DELIVERED] = ['delivered'];
  STATUS_MAP[ShipperClient.STATUS_TYPES.OUT_FOR_DELIVERY] = ['out for delivery'];
  STATUS_MAP[ShipperClient.STATUS_TYPES.SHIPPING] = ['in transit to carrier', 'shipping soon'];
  STATUS_MAP[ShipperClient.STATUS_TYPES.EN_ROUTE] = ['on the way', 'package arrived', 'package received', 'shipment departed', '
shipment arrived'];
  DAYS_OF_THE_WEEK['SUNDAY'] = 0;
  DAYS_OF_THE_WEEK['MONDAY'] = 1;
  DAYS_OF_THE_WEEK['TUESDAY'] = 2;
  DAYS_OF_THE_WEEK['WEDNESDAY'] = 3;
  DAYS_OF_THE_WEEK['THURSDAY'] = 4;
  DAYS_OF_THE_WEEK['FRIDAY'] = 5;
  DAYS_OF_THE_WEEK['SATURDAY'] = 6;
  AmazonClient.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.shipit.AmazonClient.prototype"></a>[module shipit.AmazonClient.prototype](#apidoc.module.shipit.AmazonClient.prototype)

#### <a name="apidoc.element.shipit.AmazonClient.prototype.constructor"></a>[function <span class="apidocSignatureSpan">shipit.AmazonClient.prototype.</span>constructor (options)](#apidoc.element.shipit.AmazonClient.prototype.constructor)
- description and source-code
```javascript
function AmazonClient(options) {
  this.options = options;
  STATUS_MAP[ShipperClient.STATUS_TYPES.DELAYED] = ['delivery attempted'];
  STATUS_MAP[ShipperClient.STATUS_TYPES.DELIVERED] = ['delivered'];
  STATUS_MAP[ShipperClient.STATUS_TYPES.OUT_FOR_DELIVERY] = ['out for delivery'];
  STATUS_MAP[ShipperClient.STATUS_TYPES.SHIPPING] = ['in transit to carrier', 'shipping soon'];
  STATUS_MAP[ShipperClient.STATUS_TYPES.EN_ROUTE] = ['on the way', 'package arrived', 'package received', 'shipment departed', '
shipment arrived'];
  DAYS_OF_THE_WEEK['SUNDAY'] = 0;
  DAYS_OF_THE_WEEK['MONDAY'] = 1;
  DAYS_OF_THE_WEEK['TUESDAY'] = 2;
  DAYS_OF_THE_WEEK['WEDNESDAY'] = 3;
  DAYS_OF_THE_WEEK['THURSDAY'] = 4;
  DAYS_OF_THE_WEEK['FRIDAY'] = 5;
  DAYS_OF_THE_WEEK['SATURDAY'] = 6;
  AmazonClient.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.shipit.AmazonClient.prototype.getActivitiesAndStatus"></a>[function <span class="apidocSignatureSpan">shipit.AmazonClient.prototype.</span>getActivitiesAndStatus (data)](#apidoc.element.shipit.AmazonClient.prototype.getActivitiesAndStatus)
- description and source-code
```javascript
getActivitiesAndStatus = function (data) {
  var $, activities, columns, components, date, dateStr, details, location, rightNow, row, rows, status, timeOfDay, timestamp, ts
, _i, _len;
  activities = [];
  status = null;
  if (data == null) {
    return {
      activities: activities,
      status: status
    };
  }
  $ = data.$, rightNow = data.rightNow;
  status = this.presentStatus($(".latest-event-status").text());
  rows = $("div[data-a-expander-name=event-history-list] .a-box");
  for (_i = 0, _len = rows.length; _i < _len; _i++) {
    row = rows[_i];
    columns = $($(row).find(".a-row")[0]).children('.a-column');
    if (columns.length === 2) {
      timeOfDay = $(columns[0]).text().trim();
      if (timeOfDay === '--') {
        timeOfDay = '12:00 AM';
      }
      components = $(columns[1]).children('span');
      details = (components != null ? components[0] : void 0) != null ? $(components[0]).text().trim() : '';
      location = (components != null ? components[1] : void 0) != null ? $(components[1]).text().trim() : '';
      location = this.presentLocationString(location);
      ts = "" + dateStr + " " + timeOfDay + " +00:00";
      timestamp = moment(ts, 'YYYY-MM-DD H:mm A Z').toDate();
      if ((timestamp != null) && (details != null ? details.length : void 0)) {
        activities.push({
          timestamp: timestamp,
          location: location,
          details: details
        });
        if (status == null) {
          status = this.presentStatus(details);
        }
      }
    } else {
      dateStr = $(row).text().trim().replace('Latest update: ', '');
      if (/yesterday/i.test(dateStr)) {
        date = moment(rightNow).subtract(1, 'day');
      } else if (/today/i.test(dateStr)) {
        date = moment(rightNow);
      } else if (/day/.test(dateStr)) {
        date = moment("" + dateStr + ", " + (moment(rightNow).format('YYYY')));
      } else {
        date = moment(dateStr);
      }
      dateStr = date.format('YYYY-MM-DD');
    }
  }
  return {
    activities: activities,
    status: status
  };
}
```
- example usage
```shell
...
    ShipperClient.prototype.presentResponse = function(response, requestData, cb) {
return this.validateResponse(response, (function(_this) {
  return function(err, shipment) {
    var activities, adjustedEta, eta, presentedResponse, status, _ref, _ref1;
    if ((err != null) || (shipment == null)) {
      return cb(err);
    }
    _ref = _this.getActivitiesAndStatus(shipment), activities = _ref.activities, status = _ref.status;
    eta = _this.getEta(shipment);
    if (eta != null) {
      adjustedEta = moment(eta).utc().format().replace(/T00:00:00/, 'T23:59:59');
    }
    if (adjustedEta != null) {
      adjustedEta = moment(adjustedEta).toDate();
    }
...
```

#### <a name="apidoc.element.shipit.AmazonClient.prototype.getDestination"></a>[function <span class="apidocSignatureSpan">shipit.AmazonClient.prototype.</span>getDestination (data)](#apidoc.element.shipit.AmazonClient.prototype.getDestination)
- description and source-code
```javascript
getDestination = function (data) {
  var $, dest, rightNow;
  if (data == null) {
    return;
  }
  $ = data.$, rightNow = data.rightNow;
  dest = $(".delivery-address").text();
  if (dest != null ? dest.length : void 0) {
    return this.presentLocationString(dest);
  }
}
```
- example usage
```shell
...
if (adjustedEta != null) {
  adjustedEta = moment(adjustedEta).toDate();
}
presentedResponse = {
  eta: adjustedEta,
  service: _this.getService(shipment),
  weight: _this.getWeight(shipment),
  destination: _this.getDestination(shipment),
  activities: activities,
  status: status
};
if ((requestData != null ? requestData.raw : void 0) != null) {
  if (requestData.raw) {
    presentedResponse.raw = response;
  }
...
```

#### <a name="apidoc.element.shipit.AmazonClient.prototype.getEta"></a>[function <span class="apidocSignatureSpan">shipit.AmazonClient.prototype.</span>getEta (data)](#apidoc.element.shipit.AmazonClient.prototype.getEta)
- description and source-code
```javascript
getEta = function (data) {
  var $, container, dateComponent, dateComponentStr, deliveryStatus, etaDayVal, etaString, matches, nowDayVal, numDays, rightNow
, timeComponent, _ref1, _ref2;
  if (data == null) {
    return;
  }
  $ = data.$, rightNow = data.rightNow;
  container = $(".shipment-status-content").children('span');
  if (!container.length) {
    return;
  }
  deliveryStatus = $(container[0]).text().trim();
  if (/delivered/i.test(deliveryStatus)) {
    return;
  }
  if (!/arriving/i.test(deliveryStatus)) {
    return;
  }
  if (/.* by .*/i.test(deliveryStatus)) {
    matches = deliveryStatus.match(/(.*) by (.*)/, 'i');
    deliveryStatus = matches[1];
    timeComponent = matches[2];
  }
  matches = deliveryStatus.match(/Arriving (.*)/, 'i');
  dateComponentStr = matches != null ? matches[1] : void 0;
  if (/-/.test(dateComponentStr)) {
    dateComponentStr = (_ref1 = dateComponentStr.split('-')) != null ? (_ref2 = _ref1[1]) != null ? _ref2.trim() : void 0 : void
 0;
  }
  dateComponent = moment(rightNow);
  if (/today/i.test(dateComponentStr)) {
    numDays = 0;
  } else if (/tomorrow/i.test(dateComponentStr)) {
    numDays = 1;
  } else if (/day/i.test(dateComponentStr)) {
    nowDayVal = DAYS_OF_THE_WEEK[upperCase(moment(rightNow).format('dddd'))];
    etaDayVal = DAYS_OF_THE_WEEK[upperCase(dateComponentStr)];
    if (etaDayVal > nowDayVal) {
      numDays = etaDayVal - nowDayVal;
    } else {
      numDays = 7 + (etaDayVal - nowDayVal);
    }
  } else {
    if (!/20\d{2}/.test(dateComponentStr)) {
      dateComponentStr += ', 2015';
    }
    numDays = (moment(dateComponentStr) - moment(rightNow)) / (1000 * 3600 * 24) + 1;
  }
  dateComponent = moment(rightNow).add(numDays, 'days');
  if (timeComponent == null) {
    timeComponent = "11pm";
  }
  timeComponent = upperCase(timeComponent);
  etaString = "" + (dateComponent.format('YYYY-MM-DD')) + " " + timeComponent + " +00:00";
  return moment(etaString, 'YYYY-MM-DD HA Z').toDate();
}
```
- example usage
```shell
...
      return this.validateResponse(response, (function(_this) {
return function(err, shipment) {
  var activities, adjustedEta, eta, presentedResponse, status, _ref, _ref1;
  if ((err != null) || (shipment == null)) {
    return cb(err);
  }
  _ref = _this.getActivitiesAndStatus(shipment), activities = _ref.activities, status = _ref.status;
  eta = _this.getEta(shipment);
  if (eta != null) {
    adjustedEta = moment(eta).utc().format().replace(/T00:00:00/, 'T23:59:59');
  }
  if (adjustedEta != null) {
    adjustedEta = moment(adjustedEta).toDate();
  }
  presentedResponse = {
...
```

#### <a name="apidoc.element.shipit.AmazonClient.prototype.getService"></a>[function <span class="apidocSignatureSpan">shipit.AmazonClient.prototype.</span>getService ()](#apidoc.element.shipit.AmazonClient.prototype.getService)
- description and source-code
```javascript
getService = function () {}
```
- example usage
```shell
...
  adjustedEta = moment(eta).utc().format().replace(/T00:00:00/, 'T23:59:59');
}
if (adjustedEta != null) {
  adjustedEta = moment(adjustedEta).toDate();
}
presentedResponse = {
  eta: adjustedEta,
  service: _this.getService(shipment),
  weight: _this.getWeight(shipment),
  destination: _this.getDestination(shipment),
  activities: activities,
  status: status
};
if ((requestData != null ? requestData.raw : void 0) != null) {
  if (requestData.raw) {
...
```

#### <a name="apidoc.element.shipit.AmazonClient.prototype.getWeight"></a>[function <span class="apidocSignatureSpan">shipit.AmazonClient.prototype.</span>getWeight ()](#apidoc.element.shipit.AmazonClient.prototype.getWeight)
- description and source-code
```javascript
getWeight = function () {}
```
- example usage
```shell
...
}
if (adjustedEta != null) {
  adjustedEta = moment(adjustedEta).toDate();
}
presentedResponse = {
  eta: adjustedEta,
  service: _this.getService(shipment),
  weight: _this.getWeight(shipment),
  destination: _this.getDestination(shipment),
  activities: activities,
  status: status
};
if ((requestData != null ? requestData.raw : void 0) != null) {
  if (requestData.raw) {
    presentedResponse.raw = response;
...
```

#### <a name="apidoc.element.shipit.AmazonClient.prototype.presentStatus"></a>[function <span class="apidocSignatureSpan">shipit.AmazonClient.prototype.</span>presentStatus (details)](#apidoc.element.shipit.AmazonClient.prototype.presentStatus)
- description and source-code
```javascript
presentStatus = function (details) {
  var matchStrings, regex, status, statusCode, text, _i, _len;
  status = null;
  for (statusCode in STATUS_MAP) {
    matchStrings = STATUS_MAP[statusCode];
    for (_i = 0, _len = matchStrings.length; _i < _len; _i++) {
      text = matchStrings[_i];
      regex = new RegExp(text, 'i');
      if (regex.test(lowerCase(details))) {
        status = statusCode;
        break;
      }
    }
    if (status != null) {
      break;
    }
  }
  if (status != null) {
    return parseInt(status, 10);
  }
}
```
- example usage
```shell
...
if (data == null) {
  return {
    activities: activities,
    status: status
  };
}
$ = data.$, rightNow = data.rightNow;
status = this.presentStatus($(".latest-event-status").text());
rows = $("div[data-a-expander-name=event-history-list] .a-box");
for (_i = 0, _len = rows.length; _i < _len; _i++) {
  row = rows[_i];
  columns = $($(row).find(".a-row")[0]).children('.a-column');
  if (columns.length === 2) {
    timeOfDay = $(columns[0]).text().trim();
    if (timeOfDay === '--') {
...
```

#### <a name="apidoc.element.shipit.AmazonClient.prototype.requestOptions"></a>[function <span class="apidocSignatureSpan">shipit.AmazonClient.prototype.</span>requestOptions (_arg)](#apidoc.element.shipit.AmazonClient.prototype.requestOptions)
- description and source-code
```javascript
requestOptions = function (_arg) {
  var orderID, orderingShipmentId;
  orderID = _arg.orderID, orderingShipmentId = _arg.orderingShipmentId;
  return {
    method: 'GET',
    uri: "https://www.amazon.com/gp/css/shiptrack/view.html" + "/ref=pe_385040_121528360_TE_SIMP_typ?ie=UTF8" + ("&orderID=" + orderID
) + ("&orderingShipmentId=" + orderingShipmentId) + "&packageId=1"
  };
}
```
- example usage
```shell
...
      return cb(null, presentedResponse);
    };
  })(this));
};

ShipperClient.prototype.requestData = function(requestData, cb) {
  var opts, _ref;
  opts = this.requestOptions(requestData);
  opts.timeout = (requestData != null ? requestData.timeout : void 0) || ((_ref = this.options) != null ? _ref.timeout : void 0);
  return request(opts, (function(_this) {
    return function(err, response, body) {
      if ((body == null) || (err != null)) {
        return cb(err);
      }
      if (response.statusCode !== 200) {
...
```

#### <a name="apidoc.element.shipit.AmazonClient.prototype.validateResponse"></a>[function <span class="apidocSignatureSpan">shipit.AmazonClient.prototype.</span>validateResponse (response, cb)](#apidoc.element.shipit.AmazonClient.prototype.validateResponse)
- description and source-code
```javascript
validateResponse = function (response, cb) {
  var $, rightNow, _ref1;
  $ = load(response, {
    normalizeWhitespace: true
  });
  rightNow = (_ref1 = /<!-- navp-.* \((.*)\) --?>/.exec(response)) != null ? _ref1[1] : void 0;
  return cb(null, {
    $: $,
    rightNow: rightNow
  });
}
```
- example usage
```shell
...
  if (postalCode != null ? postalCode.length : void 0) {
    address = address != null ? "" + address + " " + postalCode : postalCode;
  }
  return address;
};

ShipperClient.prototype.presentResponse = function(response, requestData, cb) {
  return this.validateResponse(response, (function(_this) {
    return function(err, shipment) {
      var activities, adjustedEta, eta, presentedResponse, status, _ref, _ref1;
      if ((err != null) || (shipment == null)) {
        return cb(err);
      }
      _ref = _this.getActivitiesAndStatus(shipment), activities = _ref.activities, status = _ref.status;
      eta = _this.getEta(shipment);
...
```



# <a name="apidoc.module.shipit.CanadaPostClient"></a>[module shipit.CanadaPostClient](#apidoc.module.shipit.CanadaPostClient)

#### <a name="apidoc.element.shipit.CanadaPostClient.CanadaPostClient"></a>[function <span class="apidocSignatureSpan">shipit.</span>CanadaPostClient (_arg, options)](#apidoc.element.shipit.CanadaPostClient.CanadaPostClient)
- description and source-code
```javascript
function CanadaPostClient(_arg, options) {
  this.username = _arg.username, this.password = _arg.password;
  this.options = options;
  CanadaPostClient.__super__.constructor.apply(this, arguments);
  this.parser = new Parser();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.shipit.CanadaPostClient.prototype"></a>[module shipit.CanadaPostClient.prototype](#apidoc.module.shipit.CanadaPostClient.prototype)

#### <a name="apidoc.element.shipit.CanadaPostClient.prototype.constructor"></a>[function <span class="apidocSignatureSpan">shipit.CanadaPostClient.prototype.</span>constructor (_arg, options)](#apidoc.element.shipit.CanadaPostClient.prototype.constructor)
- description and source-code
```javascript
function CanadaPostClient(_arg, options) {
  this.username = _arg.username, this.password = _arg.password;
  this.options = options;
  CanadaPostClient.__super__.constructor.apply(this, arguments);
  this.parser = new Parser();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.shipit.CanadaPostClient.prototype.findStatusFromMap"></a>[function <span class="apidocSignatureSpan">shipit.CanadaPostClient.prototype.</span>findStatusFromMap (statusText)](#apidoc.element.shipit.CanadaPostClient.prototype.findStatusFromMap)
- description and source-code
```javascript
findStatusFromMap = function (statusText) {
  var regex, status, statusCode, text;
  status = ShipperClient.STATUS_TYPES.UNKNOWN;
  if (!(statusText != null ? statusText.length : void 0)) {
    return status;
  }
  for (text in STATUS_MAP) {
    statusCode = STATUS_MAP[text];
    regex = new RegExp(text, 'i');
    if (regex.test(statusText)) {
      status = statusCode;
      break;
    }
  }
  return status;
}
```
- example usage
```shell
...
      break;
    }
  }
  return status;
};

CanadaPostClient.prototype.getStatus = function(lastEvent) {
  return this.findStatusFromMap(lastEvent != null ? lastEvent.details : void 0);
};

CanadaPostClient.prototype.getActivitiesAndStatus = function(shipment) {
  var activities, activity, city, details, event, events, location, stateCode, status, timestamp, _i, _len, _ref, _ref1, _ref2,
_ref3, _ref4, _ref5, _ref6, _ref7;
  activities = [];
  status = null;
  events = (_ref = shipment['significant-events']) != null ? (_ref1 = _ref[0]) != null ? _ref1['occurrence'] : void 0 : void 0;
...
```

#### <a name="apidoc.element.shipit.CanadaPostClient.prototype.getActivitiesAndStatus"></a>[function <span class="apidocSignatureSpan">shipit.CanadaPostClient.prototype.</span>getActivitiesAndStatus (shipment)](#apidoc.element.shipit.CanadaPostClient.prototype.getActivitiesAndStatus)
- description and source-code
```javascript
getActivitiesAndStatus = function (shipment) {
  var activities, activity, city, details, event, events, location, stateCode, status, timestamp, _i, _len, _ref, _ref1, _ref2,
_ref3, _ref4, _ref5, _ref6, _ref7;
  activities = [];
  status = null;
  events = (_ref = shipment['significant-events']) != null ? (_ref1 = _ref[0]) != null ? _ref1['occurrence'] : void 0 : void 0;
  _ref2 = events || [];
  for (_i = 0, _len = _ref2.length; _i < _len; _i++) {
    event = _ref2[_i];
    city = (_ref3 = event['event-site']) != null ? _ref3[0] : void 0;
    stateCode = (_ref4 = event['event-province']) != null ? _ref4[0] : void 0;
    location = this.presentLocation({
      city: city,
      stateCode: stateCode
    });
    timestamp = "" + ((_ref5 = event['event-date']) != null ? _ref5[0] : void 0) + "T" + ((_ref6 = event['event-time']) != null ?
_ref6[0] : void 0) + "Z";
    timestamp = moment(timestamp).toDate();
    details = (_ref7 = event['event-description']) != null ? _ref7[0] : void 0;
    if ((details != null) && (timestamp != null)) {
      activity = {
        timestamp: timestamp,
        location: location,
        details: details
      };
      activities.push(activity);
    }
  }
  return {
    activities: activities,
    status: this.getStatus(activities != null ? activities[0] : void 0)
  };
}
```
- example usage
```shell
...
    ShipperClient.prototype.presentResponse = function(response, requestData, cb) {
return this.validateResponse(response, (function(_this) {
  return function(err, shipment) {
    var activities, adjustedEta, eta, presentedResponse, status, _ref, _ref1;
    if ((err != null) || (shipment == null)) {
      return cb(err);
    }
    _ref = _this.getActivitiesAndStatus(shipment), activities = _ref.activities, status = _ref.status;
    eta = _this.getEta(shipment);
    if (eta != null) {
      adjustedEta = moment(eta).utc().format().replace(/T00:00:00/, 'T23:59:59');
    }
    if (adjustedEta != null) {
      adjustedEta = moment(adjustedEta).toDate();
    }
...
```

#### <a name="apidoc.element.shipit.CanadaPostClient.prototype.getDestination"></a>[function <span class="apidocSignatureSpan">shipit.CanadaPostClient.prototype.</span>getDestination (shipment)](#apidoc.element.shipit.CanadaPostClient.prototype.getDestination)
- description and source-code
```javascript
getDestination = function (shipment) {
  var _ref;
  return (_ref = shipment['destination-postal-id']) != null ? _ref[0] : void 0;
}
```
- example usage
```shell
...
if (adjustedEta != null) {
  adjustedEta = moment(adjustedEta).toDate();
}
presentedResponse = {
  eta: adjustedEta,
  service: _this.getService(shipment),
  weight: _this.getWeight(shipment),
  destination: _this.getDestination(shipment),
  activities: activities,
  status: status
};
if ((requestData != null ? requestData.raw : void 0) != null) {
  if (requestData.raw) {
    presentedResponse.raw = response;
  }
...
```

#### <a name="apidoc.element.shipit.CanadaPostClient.prototype.getEta"></a>[function <span class="apidocSignatureSpan">shipit.CanadaPostClient.prototype.</span>getEta (shipment)](#apidoc.element.shipit.CanadaPostClient.prototype.getEta)
- description and source-code
```javascript
getEta = function (shipment) {
  var ts, _ref, _ref1;
  ts = ((_ref = shipment['changed-expected-date']) != null ? _ref[0] : void 0) || ((_ref1 = shipment['expected-delivery-date']) !=
null ? _ref1[0] : void 0);
  if (!(ts != null ? ts.length : void 0)) {
    return;
  }
  if (ts != null ? ts.length : void 0) {
    return moment("" + ts + "T00:00:00Z").toDate();
  }
}
```
- example usage
```shell
...
      return this.validateResponse(response, (function(_this) {
return function(err, shipment) {
  var activities, adjustedEta, eta, presentedResponse, status, _ref, _ref1;
  if ((err != null) || (shipment == null)) {
    return cb(err);
  }
  _ref = _this.getActivitiesAndStatus(shipment), activities = _ref.activities, status = _ref.status;
  eta = _this.getEta(shipment);
  if (eta != null) {
    adjustedEta = moment(eta).utc().format().replace(/T00:00:00/, 'T23:59:59');
  }
  if (adjustedEta != null) {
    adjustedEta = moment(adjustedEta).toDate();
  }
  presentedResponse = {
...
```

#### <a name="apidoc.element.shipit.CanadaPostClient.prototype.getService"></a>[function <span class="apidocSignatureSpan">shipit.CanadaPostClient.prototype.</span>getService (shipment)](#apidoc.element.shipit.CanadaPostClient.prototype.getService)
- description and source-code
```javascript
getService = function (shipment) {
  var _ref;
  return (_ref = shipment['service-name']) != null ? _ref[0] : void 0;
}
```
- example usage
```shell
...
  adjustedEta = moment(eta).utc().format().replace(/T00:00:00/, 'T23:59:59');
}
if (adjustedEta != null) {
  adjustedEta = moment(adjustedEta).toDate();
}
presentedResponse = {
  eta: adjustedEta,
  service: _this.getService(shipment),
  weight: _this.getWeight(shipment),
  destination: _this.getDestination(shipment),
  activities: activities,
  status: status
};
if ((requestData != null ? requestData.raw : void 0) != null) {
  if (requestData.raw) {
...
```

#### <a name="apidoc.element.shipit.CanadaPostClient.prototype.getStatus"></a>[function <span class="apidocSignatureSpan">shipit.CanadaPostClient.prototype.</span>getStatus (lastEvent)](#apidoc.element.shipit.CanadaPostClient.prototype.getStatus)
- description and source-code
```javascript
getStatus = function (lastEvent) {
  return this.findStatusFromMap(lastEvent != null ? lastEvent.details : void 0);
}
```
- example usage
```shell
...
        details: details
      };
      activities.push(activity);
    }
  }
  return {
    activities: activities,
    status: this.getStatus(shipment)
  };
};

A1Client.prototype.getEta = function(shipment) {
  var activities, firstActivity, _ref, _ref1, _ref2, _ref3;
  activities = ((_ref = shipment['TrackingEventHistory']) != null ? (_ref1 = _ref[0]) != null ? _ref1['TrackingEventDetail'] : void
 0 : void 0) || [];
  firstActivity = activities[activities.length - 1];
...
```

#### <a name="apidoc.element.shipit.CanadaPostClient.prototype.getWeight"></a>[function <span class="apidocSignatureSpan">shipit.CanadaPostClient.prototype.</span>getWeight (shipment)](#apidoc.element.shipit.CanadaPostClient.prototype.getWeight)
- description and source-code
```javascript
getWeight = function (shipment) {}
```
- example usage
```shell
...
}
if (adjustedEta != null) {
  adjustedEta = moment(adjustedEta).toDate();
}
presentedResponse = {
  eta: adjustedEta,
  service: _this.getService(shipment),
  weight: _this.getWeight(shipment),
  destination: _this.getDestination(shipment),
  activities: activities,
  status: status
};
if ((requestData != null ? requestData.raw : void 0) != null) {
  if (requestData.raw) {
    presentedResponse.raw = response;
...
```

#### <a name="apidoc.element.shipit.CanadaPostClient.prototype.requestOptions"></a>[function <span class="apidocSignatureSpan">shipit.CanadaPostClient.prototype.</span>requestOptions (_arg)](#apidoc.element.shipit.CanadaPostClient.prototype.requestOptions)
- description and source-code
```javascript
requestOptions = function (_arg) {
  var trackingNumber;
  trackingNumber = _arg.trackingNumber;
  return {
    method: 'GET',
    uri: "https://soa-gw.canadapost.ca/vis/track/pin/" + trackingNumber + "/detail.xml",
    auth: {
      user: this.username,
      pass: this.password
    }
  };
}
```
- example usage
```shell
...
      return cb(null, presentedResponse);
    };
  })(this));
};

ShipperClient.prototype.requestData = function(requestData, cb) {
  var opts, _ref;
  opts = this.requestOptions(requestData);
  opts.timeout = (requestData != null ? requestData.timeout : void 0) || ((_ref = this.options) != null ? _ref.timeout : void 0);
  return request(opts, (function(_this) {
    return function(err, response, body) {
      if ((body == null) || (err != null)) {
        return cb(err);
      }
      if (response.statusCode !== 200) {
...
```

#### <a name="apidoc.element.shipit.CanadaPostClient.prototype.validateResponse"></a>[function <span class="apidocSignatureSpan">shipit.CanadaPostClient.prototype.</span>validateResponse (response, cb)](#apidoc.element.shipit.CanadaPostClient.prototype.validateResponse)
- description and source-code
```javascript
validateResponse = function (response, cb) {
  var handleResponse;
  handleResponse = function(xmlErr, trackResult) {
    var details;
    if ((xmlErr != null) || (trackResult == null)) {
      return cb(xmlErr);
    }
    details = trackResult['tracking-detail'];
    if (details == null) {
      return cb('response not recognized');
    }
    return cb(null, details);
  };
  this.parser.reset();
  return this.parser.parseString(response, handleResponse);
}
```
- example usage
```shell
...
  if (postalCode != null ? postalCode.length : void 0) {
    address = address != null ? "" + address + " " + postalCode : postalCode;
  }
  return address;
};

ShipperClient.prototype.presentResponse = function(response, requestData, cb) {
  return this.validateResponse(response, (function(_this) {
    return function(err, shipment) {
      var activities, adjustedEta, eta, presentedResponse, status, _ref, _ref1;
      if ((err != null) || (shipment == null)) {
        return cb(err);
      }
      _ref = _this.getActivitiesAndStatus(shipment), activities = _ref.activities, status = _ref.status;
      eta = _this.getEta(shipment);
...
```



# <a name="apidoc.module.shipit.DhlClient"></a>[module shipit.DhlClient](#apidoc.module.shipit.DhlClient)

#### <a name="apidoc.element.shipit.DhlClient.DhlClient"></a>[function <span class="apidocSignatureSpan">shipit.</span>DhlClient (_arg, options)](#apidoc.element.shipit.DhlClient.DhlClient)
- description and source-code
```javascript
function DhlClient(_arg, options) {
  this.userId = _arg.userId, this.password = _arg.password;
  this.options = options;
  DhlClient.__super__.constructor.apply(this, arguments);
  this.parser = new Parser();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.shipit.DhlClient.prototype"></a>[module shipit.DhlClient.prototype](#apidoc.module.shipit.DhlClient.prototype)

#### <a name="apidoc.element.shipit.DhlClient.prototype.constructor"></a>[function <span class="apidocSignatureSpan">shipit.DhlClient.prototype.</span>constructor (_arg, options)](#apidoc.element.shipit.DhlClient.prototype.constructor)
- description and source-code
```javascript
function DhlClient(_arg, options) {
  this.userId = _arg.userId, this.password = _arg.password;
  this.options = options;
  DhlClient.__super__.constructor.apply(this, arguments);
  this.parser = new Parser();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.shipit.DhlClient.prototype.generateRequest"></a>[function <span class="apidocSignatureSpan">shipit.DhlClient.prototype.</span>generateRequest (trk)](#apidoc.element.shipit.DhlClient.prototype.generateRequest)
- description and source-code
```javascript
generateRequest = function (trk) {
  return "<?xml version=\"1.0\" encoding=\"UTF-8\" standalone=\"yes\"?>\n<req:KnownTrackingRequest xmlns:req=\"http://www.dhl.com\">\n  <Request>\n    <ServiceHeader>\n      <SiteID>" + this.userId + "</SiteID>\n      <Password>" + this.password + "</Password>\n    </ServiceHeader>\n  </Request>\n  <LanguageCode>en</LanguageCode>\n  <AWBNumber>" + trk + "</AWBNumber>\n  <LevelOfDetails>ALL_CHECK_POINTS</LevelOfDetails>\n</req:KnownTrackingRequest>";
}
```
- example usage
```shell
...

  DhlClient.prototype.requestOptions = function(_arg) {
    var trackingNumber;
    trackingNumber = _arg.trackingNumber;
    return {
      method: 'POST',
      uri: 'http://xmlpi-ea.dhl.com/XMLShippingServlet',
      body: this.generateRequest(trackingNumber)
    };
  };

  return DhlClient;

})(ShipperClient);
...
```

#### <a name="apidoc.element.shipit.DhlClient.prototype.getActivitiesAndStatus"></a>[function <span class="apidocSignatureSpan">shipit.DhlClient.prototype.</span>getActivitiesAndStatus (shipment)](#apidoc.element.shipit.DhlClient.prototype.getActivitiesAndStatus)
- description and source-code
```javascript
getActivitiesAndStatus = function (shipment) {
  var activities, activity, details, location, rawActivities, rawActivity, rawLocation, status, timestamp, _i, _len, _ref1, _ref10
, _ref11, _ref12, _ref2, _ref3, _ref4, _ref5, _ref6, _ref7, _ref8, _ref9;
  activities = [];
  status = null;
  rawActivities = shipment['ShipmentEvent'];
  if (rawActivities == null) {
    rawActivities = [];
  }
  rawActivities.reverse();
  _ref1 = rawActivities || [];
  for (_i = 0, _len = _ref1.length; _i < _len; _i++) {
    rawActivity = _ref1[_i];
    rawLocation = (_ref2 = rawActivity['ServiceArea']) != null ? (_ref3 = _ref2[0]) != null ? (_ref4 = _ref3['Description']) !=
null ? _ref4[0] : void 0 : void 0 : void 0;
    location = this.presentAddress(rawLocation);
    timestamp = this.presentTimestamp((_ref5 = rawActivity['Date']) != null ? _ref5[0] : void 0, (_ref6 = rawActivity['Time']) !=
null ? _ref6[0] : void 0);
    details = this.presentDetails(rawLocation, (_ref7 = rawActivity['ServiceEvent']) != null ? (_ref8 = _ref7[0]) != null ? (_ref9
 = _ref8['Description']) != null ? _ref9[0] : void 0 : void 0 : void 0);
    if ((details != null) && (timestamp != null)) {
      details = details.slice(-1) === '.' ? details.slice(0, -1) : details;
      activity = {
        timestamp: timestamp,
        location: location,
        details: details
      };
      activities.push(activity);
    }
    if (!status) {
      status = this.presentStatus((_ref10 = rawActivity['ServiceEvent']) != null ? (_ref11 = _ref10[0]) != null ? (_ref12 = _ref11
['EventCode']) != null ? _ref12[0] : void 0 : void 0 : void 0);
    }
  }
  return {
    activities: activities,
    status: status
  };
}
```
- example usage
```shell
...
    ShipperClient.prototype.presentResponse = function(response, requestData, cb) {
return this.validateResponse(response, (function(_this) {
  return function(err, shipment) {
    var activities, adjustedEta, eta, presentedResponse, status, _ref, _ref1;
    if ((err != null) || (shipment == null)) {
      return cb(err);
    }
    _ref = _this.getActivitiesAndStatus(shipment), activities = _ref.activities, status = _ref.status;
    eta = _this.getEta(shipment);
    if (eta != null) {
      adjustedEta = moment(eta).utc().format().replace(/T00:00:00/, 'T23:59:59');
    }
    if (adjustedEta != null) {
      adjustedEta = moment(adjustedEta).toDate();
    }
...
```

#### <a name="apidoc.element.shipit.DhlClient.prototype.getDestination"></a>[function <span class="apidocSignatureSpan">shipit.DhlClient.prototype.</span>getDestination (shipment)](#apidoc.element.shipit.DhlClient.prototype.getDestination)
- description and source-code
```javascript
getDestination = function (shipment) {
  var destination, _ref1, _ref2, _ref3;
  destination = (_ref1 = shipment['DestinationServiceArea']) != null ? (_ref2 = _ref1[0]) != null ? (_ref3 = _ref2['Description']) !=
null ? _ref3[0] : void 0 : void 0 : void 0;
  if (destination == null) {
    return;
  }
  return this.presentAddress(destination);
}
```
- example usage
```shell
...
if (adjustedEta != null) {
  adjustedEta = moment(adjustedEta).toDate();
}
presentedResponse = {
  eta: adjustedEta,
  service: _this.getService(shipment),
  weight: _this.getWeight(shipment),
  destination: _this.getDestination(shipment),
  activities: activities,
  status: status
};
if ((requestData != null ? requestData.raw : void 0) != null) {
  if (requestData.raw) {
    presentedResponse.raw = response;
  }
...
```

#### <a name="apidoc.element.shipit.DhlClient.prototype.getEta"></a>[function <span class="apidocSignatureSpan">shipit.DhlClient.prototype.</span>getEta (shipment)](#apidoc.element.shipit.DhlClient.prototype.getEta)
- description and source-code
```javascript
getEta = function (shipment) {}
```
- example usage
```shell
...
      return this.validateResponse(response, (function(_this) {
return function(err, shipment) {
  var activities, adjustedEta, eta, presentedResponse, status, _ref, _ref1;
  if ((err != null) || (shipment == null)) {
    return cb(err);
  }
  _ref = _this.getActivitiesAndStatus(shipment), activities = _ref.activities, status = _ref.status;
  eta = _this.getEta(shipment);
  if (eta != null) {
    adjustedEta = moment(eta).utc().format().replace(/T00:00:00/, 'T23:59:59');
  }
  if (adjustedEta != null) {
    adjustedEta = moment(adjustedEta).toDate();
  }
  presentedResponse = {
...
```

#### <a name="apidoc.element.shipit.DhlClient.prototype.getService"></a>[function <span class="apidocSignatureSpan">shipit.DhlClient.prototype.</span>getService (shipment)](#apidoc.element.shipit.DhlClient.prototype.getService)
- description and source-code
```javascript
getService = function (shipment) {}
```
- example usage
```shell
...
  adjustedEta = moment(eta).utc().format().replace(/T00:00:00/, 'T23:59:59');
}
if (adjustedEta != null) {
  adjustedEta = moment(adjustedEta).toDate();
}
presentedResponse = {
  eta: adjustedEta,
  service: _this.getService(shipment),
  weight: _this.getWeight(shipment),
  destination: _this.getDestination(shipment),
  activities: activities,
  status: status
};
if ((requestData != null ? requestData.raw : void 0) != null) {
  if (requestData.raw) {
...
```

#### <a name="apidoc.element.shipit.DhlClient.prototype.getWeight"></a>[function <span class="apidocSignatureSpan">shipit.DhlClient.prototype.</span>getWeight (shipment)](#apidoc.element.shipit.DhlClient.prototype.getWeight)
- description and source-code
```javascript
getWeight = function (shipment) {
  var weight, _ref1;
  weight = (_ref1 = shipment['Weight']) != null ? _ref1[0] : void 0;
  if (weight != null) {
    return "" + weight + " LB";
  }
}
```
- example usage
```shell
...
}
if (adjustedEta != null) {
  adjustedEta = moment(adjustedEta).toDate();
}
presentedResponse = {
  eta: adjustedEta,
  service: _this.getService(shipment),
  weight: _this.getWeight(shipment),
  destination: _this.getDestination(shipment),
  activities: activities,
  status: status
};
if ((requestData != null ? requestData.raw : void 0) != null) {
  if (requestData.raw) {
    presentedResponse.raw = response;
...
```

#### <a name="apidoc.element.shipit.DhlClient.prototype.presentAddress"></a>[function <span class="apidocSignatureSpan">shipit.DhlClient.prototype.</span>presentAddress (rawAddress)](#apidoc.element.shipit.DhlClient.prototype.presentAddress)
- description and source-code
```javascript
presentAddress = function (rawAddress) {
  var city, countryCode, firstComma, firstDash, stateCode;
  if (rawAddress == null) {
    return;
  }
  firstComma = rawAddress.indexOf(',');
  firstDash = rawAddress.indexOf('-', firstComma);
  if (firstComma > -1 && firstDash > -1) {
    city = rawAddress.substring(0, firstComma).trim();
    stateCode = rawAddress.substring(firstComma + 1, firstDash).trim();
    countryCode = rawAddress.substring(firstDash + 1).trim();
  } else if (firstComma < 0 && firstDash > -1) {
    city = rawAddress.substring(0, firstDash).trim();
    stateCode = null;
    countryCode = rawAddress.substring(firstDash + 1).trim();
  } else {
    return rawAddress;
  }
  city = city.replace(' HUB', '');
  city = city.replace(' GATEWAY', '');
  return this.presentLocation({
    city: city,
    stateCode: stateCode,
    countryCode: countryCode
  });
}
```
- example usage
```shell
...
var activities, activity, datetime, details, event_time, location, rawActivities, rawActivity, raw_timestamp, status, timestamp,
_i, _len, _ref, _ref1, _ref2, _ref3, _ref4;
activities = [];
status = null;
rawActivities = (_ref = shipment['TrackingEventHistory']) != null ? (_ref1 = _ref[0]) != null ? _ref1['TrackingEventDetail'] : void
 0 : void 0;
_ref2 = rawActivities || [];
for (_i = 0, _len = _ref2.length; _i < _len; _i++) {
  rawActivity = _ref2[_i];
  location = this.presentAddress(rawActivity != null ? (_ref3 = rawActivity['EventLocation']) != null ? _ref3[0] : void 0 : void
 0);
  raw_timestamp = rawActivity != null ? rawActivity['EventDateTime'][0] : void 0;
  if (raw_timestamp != null) {
    event_time = moment(raw_timestamp);
    timestamp = event_time.toDate();
    datetime = raw_timestamp.slice(0, 19);
  }
  details = rawActivity != null ? (_ref4 = rawActivity['EventCodeDesc']) != null ? _ref4[0] : void 0 : void 0;
...
```

#### <a name="apidoc.element.shipit.DhlClient.prototype.presentDetails"></a>[function <span class="apidocSignatureSpan">shipit.DhlClient.prototype.</span>presentDetails (rawAddress, rawDetails)](#apidoc.element.shipit.DhlClient.prototype.presentDetails)
- description and source-code
```javascript
presentDetails = function (rawAddress, rawDetails) {
  if (rawDetails == null) {
    return;
  }
  if (rawAddress == null) {
    return rawDetails;
  }
  return rawDetails.replace(/\s\s+/, ' ').trim().replace(new RegExp("(?: at| in)? " + (rawAddress.trim()) + "$"), '');
}
```
- example usage
```shell
...
rawActivities.reverse();
_ref1 = rawActivities || [];
for (_i = 0, _len = _ref1.length; _i < _len; _i++) {
  rawActivity = _ref1[_i];
  rawLocation = (_ref2 = rawActivity['ServiceArea']) != null ? (_ref3 = _ref2[0]) != null ? (_ref4 = _ref3['Description']) != null
 ? _ref4[0] : void 0 : void 0 : void 0;
  location = this.presentAddress(rawLocation);
  timestamp = this.presentTimestamp((_ref5 = rawActivity['Date']) != null ? _ref5[0] : void 0, (_ref6 = rawActivity['Time']) !=
null ? _ref6[0] : void 0);
  details = this.presentDetails(rawLocation, (_ref7 = rawActivity['ServiceEvent']) != null ? (_ref8 = _ref7[0]) != null ? (_ref9
 = _ref8['Description']) != null ? _ref9[0] : void 0 : void 0 : void 0);
  if ((details != null) && (timestamp != null)) {
    details = details.slice(-1) === '.' ? details.slice(0, -1) : details;
    activity = {
      timestamp: timestamp,
      location: location,
      details: details
    };
...
```

#### <a name="apidoc.element.shipit.DhlClient.prototype.presentStatus"></a>[function <span class="apidocSignatureSpan">shipit.DhlClient.prototype.</span>presentStatus (status)](#apidoc.element.shipit.DhlClient.prototype.presentStatus)
- description and source-code
```javascript
presentStatus = function (status) {
  return STATUS_MAP[status] || ShipperClient.STATUS_TYPES.UNKNOWN;
}
```
- example usage
```shell
...
if (data == null) {
  return {
    activities: activities,
    status: status
  };
}
$ = data.$, rightNow = data.rightNow;
status = this.presentStatus($(".latest-event-status").text());
rows = $("div[data-a-expander-name=event-history-list] .a-box");
for (_i = 0, _len = rows.length; _i < _len; _i++) {
  row = rows[_i];
  columns = $($(row).find(".a-row")[0]).children('.a-column');
  if (columns.length === 2) {
    timeOfDay = $(columns[0]).text().trim();
    if (timeOfDay === '--') {
...
```

#### <a name="apidoc.element.shipit.DhlClient.prototype.presentTimestamp"></a>[function <span class="apidocSignatureSpan">shipit.DhlClient.prototype.</span>presentTimestamp (dateString, timeString)](#apidoc.element.shipit.DhlClient.prototype.presentTimestamp)
- description and source-code
```javascript
presentTimestamp = function (dateString, timeString) {
  var inputString;
  if (dateString == null) {
    return;
  }
  if (timeString == null) {
    timeString = '00:00';
  }
  inputString = "" + dateString + " " + timeString + " +0000";
  return moment(inputString).toDate();
}
```
- example usage
```shell
...
}
rawActivities.reverse();
_ref1 = rawActivities || [];
for (_i = 0, _len = _ref1.length; _i < _len; _i++) {
  rawActivity = _ref1[_i];
  rawLocation = (_ref2 = rawActivity['ServiceArea']) != null ? (_ref3 = _ref2[0]) != null ? (_ref4 = _ref3['Description']) != null
 ? _ref4[0] : void 0 : void 0 : void 0;
  location = this.presentAddress(rawLocation);
  timestamp = this.presentTimestamp((_ref5 = rawActivity['Date']) != null ? _ref5[0] : void 0, (_ref6 = rawActivity['Time']) !=
null ? _ref6[0] : void 0);
  details = this.presentDetails(rawLocation, (_ref7 = rawActivity['ServiceEvent']) != null ? (_ref8 = _ref7[0]) != null ? (_ref9
 = _ref8['Description']) != null ? _ref9[0] : void 0 : void 0 : void 0);
  if ((details != null) && (timestamp != null)) {
    details = details.slice(-1) === '.' ? details.slice(0, -1) : details;
    activity = {
      timestamp: timestamp,
      location: location,
      details: details
...
```

#### <a name="apidoc.element.shipit.DhlClient.prototype.requestOptions"></a>[function <span class="apidocSignatureSpan">shipit.DhlClient.prototype.</span>requestOptions (_arg)](#apidoc.element.shipit.DhlClient.prototype.requestOptions)
- description and source-code
```javascript
requestOptions = function (_arg) {
  var trackingNumber;
  trackingNumber = _arg.trackingNumber;
  return {
    method: 'POST',
    uri: 'http://xmlpi-ea.dhl.com/XMLShippingServlet',
    body: this.generateRequest(trackingNumber)
  };
}
```
- example usage
```shell
...
      return cb(null, presentedResponse);
    };
  })(this));
};

ShipperClient.prototype.requestData = function(requestData, cb) {
  var opts, _ref;
  opts = this.requestOptions(requestData);
  opts.timeout = (requestData != null ? requestData.timeout : void 0) || ((_ref = this.options) != null ? _ref.timeout : void 0);
  return request(opts, (function(_this) {
    return function(err, response, body) {
      if ((body == null) || (err != null)) {
        return cb(err);
      }
      if (response.statusCode !== 200) {
...
```

#### <a name="apidoc.element.shipit.DhlClient.prototype.validateResponse"></a>[function <span class="apidocSignatureSpan">shipit.DhlClient.prototype.</span>validateResponse (response, cb)](#apidoc.element.shipit.DhlClient.prototype.validateResponse)
- description and source-code
```javascript
validateResponse = function (response, cb) {
  var handleResponse;
  handleResponse = function(xmlErr, trackResult) {
    var awbInfo, shipment, statusCode, trackStatus, trackingResponse, _ref1, _ref2, _ref3;
    if ((xmlErr != null) || (trackResult == null)) {
      return cb(xmlErr);
    }
    trackingResponse = trackResult['req:TrackingResponse'];
    if (trackingResponse == null) {
      return cb({
        error: 'no tracking response'
      });
    }
    awbInfo = (_ref1 = trackingResponse['AWBInfo']) != null ? _ref1[0] : void 0;
    if (awbInfo == null) {
      return cb({
        error: 'no AWBInfo in response'
      });
    }
    shipment = (_ref2 = awbInfo['ShipmentInfo']) != null ? _ref2[0] : void 0;
    if (shipment == null) {
      return cb({
        error: 'could not find shipment'
      });
    }
    trackStatus = (_ref3 = awbInfo['Status']) != null ? _ref3[0] : void 0;
    statusCode = trackStatus != null ? trackStatus['ActionStatus'] : void 0;
    if (statusCode.toString() !== 'success') {
      return cb({
        error: "unexpected track status code=" + statusCode
      });
    }
    return cb(null, shipment);
  };
  this.parser.reset();
  return this.parser.parseString(response, handleResponse);
}
```
- example usage
```shell
...
  if (postalCode != null ? postalCode.length : void 0) {
    address = address != null ? "" + address + " " + postalCode : postalCode;
  }
  return address;
};

ShipperClient.prototype.presentResponse = function(response, requestData, cb) {
  return this.validateResponse(response, (function(_this) {
    return function(err, shipment) {
      var activities, adjustedEta, eta, presentedResponse, status, _ref, _ref1;
      if ((err != null) || (shipment == null)) {
        return cb(err);
      }
      _ref = _this.getActivitiesAndStatus(shipment), activities = _ref.activities, status = _ref.status;
      eta = _this.getEta(shipment);
...
```



# <a name="apidoc.module.shipit.DhlGmClient"></a>[module shipit.DhlGmClient](#apidoc.module.shipit.DhlGmClient)

#### <a name="apidoc.element.shipit.DhlGmClient.DhlGmClient"></a>[function <span class="apidocSignatureSpan">shipit.</span>DhlGmClient (options)](#apidoc.element.shipit.DhlGmClient.DhlGmClient)
- description and source-code
```javascript
function DhlGmClient(options) {
  this.options = options;
  STATUS_MAP[ShipperClient.STATUS_TYPES.DELIVERED] = ['delivered'];
  STATUS_MAP[ShipperClient.STATUS_TYPES.EN_ROUTE] = ['transferred', 'cleared', 'received', 'processed', 'sorted', 'sorting complete
', 'arrival', 'tendered'];
  STATUS_MAP[ShipperClient.STATUS_TYPES.OUT_FOR_DELIVERY] = ['out for delivery'];
  STATUS_MAP[ShipperClient.STATUS_TYPES.SHIPPING] = ['electronic notification received'];
  DhlGmClient.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.shipit.DhlGmClient.prototype"></a>[module shipit.DhlGmClient.prototype](#apidoc.module.shipit.DhlGmClient.prototype)

#### <a name="apidoc.element.shipit.DhlGmClient.prototype.constructor"></a>[function <span class="apidocSignatureSpan">shipit.DhlGmClient.prototype.</span>constructor (options)](#apidoc.element.shipit.DhlGmClient.prototype.constructor)
- description and source-code
```javascript
function DhlGmClient(options) {
  this.options = options;
  STATUS_MAP[ShipperClient.STATUS_TYPES.DELIVERED] = ['delivered'];
  STATUS_MAP[ShipperClient.STATUS_TYPES.EN_ROUTE] = ['transferred', 'cleared', 'received', 'processed', 'sorted', 'sorting complete
', 'arrival', 'tendered'];
  STATUS_MAP[ShipperClient.STATUS_TYPES.OUT_FOR_DELIVERY] = ['out for delivery'];
  STATUS_MAP[ShipperClient.STATUS_TYPES.SHIPPING] = ['electronic notification received'];
  DhlGmClient.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.shipit.DhlGmClient.prototype.extractHeaderField"></a>[function <span class="apidocSignatureSpan">shipit.DhlGmClient.prototype.</span>extractHeaderField (data, name)](#apidoc.element.shipit.DhlGmClient.prototype.extractHeaderField)
- description and source-code
```javascript
extractHeaderField = function (data, name) {
  var $, regex, value;
  if (data == null) {
    return;
  }
  $ = data;
  value = void 0;
  regex = new RegExp(name);
  $(".card > .row").children().each(function(findex, field) {
    $(field).children().each(function(cindex, col) {
      return $(col).find('dt').each(function(dindex, element) {
        var _ref1, _ref2;
        if (regex.test($(element).text())) {
          return value = (_ref1 = $(element).next()) != null ? (_ref2 = _ref1.text()) != null ? _ref2.trim() : void 0 : void 0;
        }
      });
    });
    if (value != null) {
      return false;
    }
  });
  return value;
}
```
- example usage
```shell
...
  return {
    activities: activities,
    status: status
  };
};

DhlGmClient.prototype.getDestination = function(data) {
  return this.extractHeaderField(data, 'To:');
};

DhlGmClient.prototype.requestOptions = function(_arg) {
  var trackingNumber;
  trackingNumber = _arg.trackingNumber;
  return {
    method: 'GET',
...
```

#### <a name="apidoc.element.shipit.DhlGmClient.prototype.extractSummaryField"></a>[function <span class="apidocSignatureSpan">shipit.DhlGmClient.prototype.</span>extractSummaryField (data, name)](#apidoc.element.shipit.DhlGmClient.prototype.extractSummaryField)
- description and source-code
```javascript
extractSummaryField = function (data, name) {
  var $, regex, value;
  if (data == null) {
    return;
  }
  $ = data;
  value = void 0;
  regex = new RegExp(name);
  $(".card-info > dl").children().each(function(findex, field) {
    var _ref1, _ref2;
    if (regex.test($(field).text())) {
      value = (_ref1 = $(field).next()) != null ? (_ref2 = _ref1.text()) != null ? _ref2.trim() : void 0 : void 0;
    }
    if (value != null) {
      return false;
    }
  });
  return value;
}
```
- example usage
```shell
...
  if (!(eta != null ? eta.length : void 0)) {
    return;
  }
  return moment("" + eta + " 23:59:59 +00:00").toDate();
};

DhlGmClient.prototype.getService = function(data) {
  return this.extractSummaryField(data, 'Service');
};

DhlGmClient.prototype.getWeight = function(data) {
  return this.extractSummaryField(data, 'Weight');
};

DhlGmClient.prototype.presentStatus = function(details) {
...
```

#### <a name="apidoc.element.shipit.DhlGmClient.prototype.getActivitiesAndStatus"></a>[function <span class="apidocSignatureSpan">shipit.DhlGmClient.prototype.</span>getActivitiesAndStatus (data)](#apidoc.element.shipit.DhlGmClient.prototype.getActivitiesAndStatus)
- description and source-code
```javascript
getActivitiesAndStatus = function (data) {
  var $, activities, currentDate, currentTime, details, location, row, rowData, status, timestamp, _i, _len, _ref1, _ref2, _ref3
;
  status = null;
  activities = [];
  if (data == null) {
    return {
      activities: activities,
      status: status
    };
  }
  $ = data;
  currentDate = null;
  _ref1 = $(".timeline").children() || [];
  for (_i = 0, _len = _ref1.length; _i < _len; _i++) {
    rowData = _ref1[_i];
    row = $(rowData);
    if (row.hasClass('timeline-date')) {
      currentDate = row.text();
    }
    if (row.hasClass('timeline-event')) {
      currentTime = row.find(".timeline-time").text();
      if (currentTime != null ? currentTime.length : void 0) {
        if (currentTime != null ? currentTime.length : void 0) {
          currentTime = (_ref2 = currentTime.trim().split(' ')) != null ? _ref2[0] : void 0;
        }
        currentTime = currentTime.replace('AM', ' AM').replace('PM', ' PM');
        currentTime += " +00:00";
        timestamp = moment("" + currentDate + " " + currentTime).toDate();
      }
      location = row.find(".timeline-location-responsive").text();
      location = location != null ? location.trim() : void 0;
      if (location != null ? location.length : void 0) {
        location = upperCaseFirst(location);
      }
      details = (_ref3 = row.find(".timeline-description").text()) != null ? _ref3.trim() : void 0;
      if ((details != null) && (timestamp != null)) {
        if (status == null) {
          status = this.presentStatus(details);
        }
        activities.push({
          details: details,
          location: location,
          timestamp: timestamp
        });
      }
    }
  }
  return {
    activities: activities,
    status: status
  };
}
```
- example usage
```shell
...
    ShipperClient.prototype.presentResponse = function(response, requestData, cb) {
return this.validateResponse(response, (function(_this) {
  return function(err, shipment) {
    var activities, adjustedEta, eta, presentedResponse, status, _ref, _ref1;
    if ((err != null) || (shipment == null)) {
      return cb(err);
    }
    _ref = _this.getActivitiesAndStatus(shipment), activities = _ref.activities, status = _ref.status;
    eta = _this.getEta(shipment);
    if (eta != null) {
      adjustedEta = moment(eta).utc().format().replace(/T00:00:00/, 'T23:59:59');
    }
    if (adjustedEta != null) {
      adjustedEta = moment(adjustedEta).toDate();
    }
...
```

#### <a name="apidoc.element.shipit.DhlGmClient.prototype.getDestination"></a>[function <span class="apidocSignatureSpan">shipit.DhlGmClient.prototype.</span>getDestination (data)](#apidoc.element.shipit.DhlGmClient.prototype.getDestination)
- description and source-code
```javascript
getDestination = function (data) {
  return this.extractHeaderField(data, 'To:');
}
```
- example usage
```shell
...
if (adjustedEta != null) {
  adjustedEta = moment(adjustedEta).toDate();
}
presentedResponse = {
  eta: adjustedEta,
  service: _this.getService(shipment),
  weight: _this.getWeight(shipment),
  destination: _this.getDestination(shipment),
  activities: activities,
  status: status
};
if ((requestData != null ? requestData.raw : void 0) != null) {
  if (requestData.raw) {
    presentedResponse.raw = response;
  }
...
```

#### <a name="apidoc.element.shipit.DhlGmClient.prototype.getEta"></a>[function <span class="apidocSignatureSpan">shipit.DhlGmClient.prototype.</span>getEta (data)](#apidoc.element.shipit.DhlGmClient.prototype.getEta)
- description and source-code
```javascript
getEta = function (data) {
  var $, eta;
  if (data == null) {
    return;
  }
  $ = data;
  eta = $(".status-info > .row .est-delivery > p").text();
  if (!(eta != null ? eta.length : void 0)) {
    return;
  }
  return moment("" + eta + " 23:59:59 +00:00").toDate();
}
```
- example usage
```shell
...
      return this.validateResponse(response, (function(_this) {
return function(err, shipment) {
  var activities, adjustedEta, eta, presentedResponse, status, _ref, _ref1;
  if ((err != null) || (shipment == null)) {
    return cb(err);
  }
  _ref = _this.getActivitiesAndStatus(shipment), activities = _ref.activities, status = _ref.status;
  eta = _this.getEta(shipment);
  if (eta != null) {
    adjustedEta = moment(eta).utc().format().replace(/T00:00:00/, 'T23:59:59');
  }
  if (adjustedEta != null) {
    adjustedEta = moment(adjustedEta).toDate();
  }
  presentedResponse = {
...
```

#### <a name="apidoc.element.shipit.DhlGmClient.prototype.getService"></a>[function <span class="apidocSignatureSpan">shipit.DhlGmClient.prototype.</span>getService (data)](#apidoc.element.shipit.DhlGmClient.prototype.getService)
- description and source-code
```javascript
getService = function (data) {
  return this.extractSummaryField(data, 'Service');
}
```
- example usage
```shell
...
  adjustedEta = moment(eta).utc().format().replace(/T00:00:00/, 'T23:59:59');
}
if (adjustedEta != null) {
  adjustedEta = moment(adjustedEta).toDate();
}
presentedResponse = {
  eta: adjustedEta,
  service: _this.getService(shipment),
  weight: _this.getWeight(shipment),
  destination: _this.getDestination(shipment),
  activities: activities,
  status: status
};
if ((requestData != null ? requestData.raw : void 0) != null) {
  if (requestData.raw) {
...
```

#### <a name="apidoc.element.shipit.DhlGmClient.prototype.getWeight"></a>[function <span class="apidocSignatureSpan">shipit.DhlGmClient.prototype.</span>getWeight (data)](#apidoc.element.shipit.DhlGmClient.prototype.getWeight)
- description and source-code
```javascript
getWeight = function (data) {
  return this.extractSummaryField(data, 'Weight');
}
```
- example usage
```shell
...
}
if (adjustedEta != null) {
  adjustedEta = moment(adjustedEta).toDate();
}
presentedResponse = {
  eta: adjustedEta,
  service: _this.getService(shipment),
  weight: _this.getWeight(shipment),
  destination: _this.getDestination(shipment),
  activities: activities,
  status: status
};
if ((requestData != null ? requestData.raw : void 0) != null) {
  if (requestData.raw) {
    presentedResponse.raw = response;
...
```

#### <a name="apidoc.element.shipit.DhlGmClient.prototype.presentStatus"></a>[function <span class="apidocSignatureSpan">shipit.DhlGmClient.prototype.</span>presentStatus (details)](#apidoc.element.shipit.DhlGmClient.prototype.presentStatus)
- description and source-code
```javascript
presentStatus = function (details) {
  var matchStrings, regex, status, statusCode, text, _i, _len;
  status = null;
  for (statusCode in STATUS_MAP) {
    matchStrings = STATUS_MAP[statusCode];
    for (_i = 0, _len = matchStrings.length; _i < _len; _i++) {
      text = matchStrings[_i];
      regex = new RegExp(text, 'i');
      if (regex.test(lowerCase(details))) {
        status = statusCode;
        break;
      }
    }
    if (status != null) {
      break;
    }
  }
  if (status != null) {
    return parseInt(status, 10);
  }
}
```
- example usage
```shell
...
if (data == null) {
  return {
    activities: activities,
    status: status
  };
}
$ = data.$, rightNow = data.rightNow;
status = this.presentStatus($(".latest-event-status").text());
rows = $("div[data-a-expander-name=event-history-list] .a-box");
for (_i = 0, _len = rows.length; _i < _len; _i++) {
  row = rows[_i];
  columns = $($(row).find(".a-row")[0]).children('.a-column');
  if (columns.length === 2) {
    timeOfDay = $(columns[0]).text().trim();
    if (timeOfDay === '--') {
...
```

#### <a name="apidoc.element.shipit.DhlGmClient.prototype.requestOptions"></a>[function <span class="apidocSignatureSpan">shipit.DhlGmClient.prototype.</span>requestOptions (_arg)](#apidoc.element.shipit.DhlGmClient.prototype.requestOptions)
- description and source-code
```javascript
requestOptions = function (_arg) {
  var trackingNumber;
  trackingNumber = _arg.trackingNumber;
  return {
    method: 'GET',
    uri: "http://webtrack.dhlglobalmail.com/?trackingnumber=" + trackingNumber
  };
}
```
- example usage
```shell
...
      return cb(null, presentedResponse);
    };
  })(this));
};

ShipperClient.prototype.requestData = function(requestData, cb) {
  var opts, _ref;
  opts = this.requestOptions(requestData);
  opts.timeout = (requestData != null ? requestData.timeout : void 0) || ((_ref = this.options) != null ? _ref.timeout : void 0);
  return request(opts, (function(_this) {
    return function(err, response, body) {
      if ((body == null) || (err != null)) {
        return cb(err);
      }
      if (response.statusCode !== 200) {
...
```

#### <a name="apidoc.element.shipit.DhlGmClient.prototype.validateResponse"></a>[function <span class="apidocSignatureSpan">shipit.DhlGmClient.prototype.</span>validateResponse (response, cb)](#apidoc.element.shipit.DhlGmClient.prototype.validateResponse)
- description and source-code
```javascript
validateResponse = function (response, cb) {
  var error;
  try {
    response = response.replace(/<br>/gi, ' ');
    return cb(null, load(response, {
      normalizeWhitespace: true
    }));
  } catch (_error) {
    error = _error;
    return cb(error);
  }
}
```
- example usage
```shell
...
  if (postalCode != null ? postalCode.length : void 0) {
    address = address != null ? "" + address + " " + postalCode : postalCode;
  }
  return address;
};

ShipperClient.prototype.presentResponse = function(response, requestData, cb) {
  return this.validateResponse(response, (function(_this) {
    return function(err, shipment) {
      var activities, adjustedEta, eta, presentedResponse, status, _ref, _ref1;
      if ((err != null) || (shipment == null)) {
        return cb(err);
      }
      _ref = _this.getActivitiesAndStatus(shipment), activities = _ref.activities, status = _ref.status;
      eta = _this.getEta(shipment);
...
```



# <a name="apidoc.module.shipit.FedexClient"></a>[module shipit.FedexClient](#apidoc.module.shipit.FedexClient)

#### <a name="apidoc.element.shipit.FedexClient.FedexClient"></a>[function <span class="apidocSignatureSpan">shipit.</span>FedexClient (_arg, options)](#apidoc.element.shipit.FedexClient.FedexClient)
- description and source-code
```javascript
function FedexClient(_arg, options) {
  this.key = _arg.key, this.password = _arg.password, this.account = _arg.account, this.meter = _arg.meter;
  this.options = options;
  FedexClient.__super__.constructor.apply(this, arguments);
  this.parser = new Parser();
  this.builder = new Builder({
    renderOpts: {
      pretty: false
    }
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.shipit.FedexClient.prototype"></a>[module shipit.FedexClient.prototype](#apidoc.module.shipit.FedexClient.prototype)

#### <a name="apidoc.element.shipit.FedexClient.prototype.constructor"></a>[function <span class="apidocSignatureSpan">shipit.FedexClient.prototype.</span>constructor (_arg, options)](#apidoc.element.shipit.FedexClient.prototype.constructor)
- description and source-code
```javascript
function FedexClient(_arg, options) {
  this.key = _arg.key, this.password = _arg.password, this.account = _arg.account, this.meter = _arg.meter;
  this.options = options;
  FedexClient.__super__.constructor.apply(this, arguments);
  this.parser = new Parser();
  this.builder = new Builder({
    renderOpts: {
      pretty: false
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.shipit.FedexClient.prototype.generateRequest"></a>[function <span class="apidocSignatureSpan">shipit.FedexClient.prototype.</span>generateRequest (trk, reference)](#apidoc.element.shipit.FedexClient.prototype.generateRequest)
- description and source-code
```javascript
generateRequest = function (trk, reference) {
  if (reference == null) {
    reference = 'n/a';
  }
  return this.builder.buildObject({
    'ns:TrackRequest': {
      '$': {
        'xmlns:ns': 'http://fedex.com/ws/track/v5',
        'xmlns:xsi': 'http://www.w3.org/2001/XMLSchema-instance',
        'xsi:schemaLocation': 'http://fedex.com/ws/track/v4 TrackService_v4.xsd'
      },
      'ns:WebAuthenticationDetail': {
        'ns:UserCredential': {
          'ns:Key': this.key,
          'ns:Password': this.password
        }
      },
      'ns:ClientDetail': {
        'ns:AccountNumber': this.account,
        'ns:MeterNumber': this.meter
      },
      'ns:TransactionDetail': {
        'ns:CustomerTransactionId': reference
      },
      'ns:Version': {
        'ns:ServiceId': 'trck',
        'ns:Major': 5,
        'ns:Intermediate': 0,
        'ns:Minor': 0
      },
      'ns:PackageIdentifier': {
        'ns:Value': trk,
        'ns:Type': 'TRACKING_NUMBER_OR_DOORTAG'
      },
      'ns:IncludeDetailedScans': true
    }
  });
}
```
- example usage
```shell
...

  DhlClient.prototype.requestOptions = function(_arg) {
    var trackingNumber;
    trackingNumber = _arg.trackingNumber;
    return {
      method: 'POST',
      uri: 'http://xmlpi-ea.dhl.com/XMLShippingServlet',
      body: this.generateRequest(trackingNumber)
    };
  };

  return DhlClient;

})(ShipperClient);
...
```

#### <a name="apidoc.element.shipit.FedexClient.prototype.getActivitiesAndStatus"></a>[function <span class="apidocSignatureSpan">shipit.FedexClient.prototype.</span>getActivitiesAndStatus (shipment)](#apidoc.element.shipit.FedexClient.prototype.getActivitiesAndStatus)
- description and source-code
```javascript
getActivitiesAndStatus = function (shipment) {
  var activities, activity, datetime, details, event_time, location, rawActivity, raw_timestamp, status, timestamp, _i, _len, _ref1
, _ref2, _ref3, _ref4;
  activities = [];
  status = null;
  _ref1 = shipment['Events'] || [];
  for (_i = 0, _len = _ref1.length; _i < _len; _i++) {
    rawActivity = _ref1[_i];
    location = this.presentAddress((_ref2 = rawActivity['Address']) != null ? _ref2[0] : void 0);
    raw_timestamp = (_ref3 = rawActivity['Timestamp']) != null ? _ref3[0] : void 0;
    if (raw_timestamp != null) {
      event_time = moment(raw_timestamp);
      timestamp = event_time.toDate();
      datetime = raw_timestamp.slice(0, 19);
    }
    details = (_ref4 = rawActivity['EventDescription']) != null ? _ref4[0] : void 0;
    if ((details != null) && (timestamp != null)) {
      activity = {
        timestamp: timestamp,
        datetime: datetime,
        location: location,
        details: details
      };
      activities.push(activity);
    }
  }
  return {
    activities: activities,
    status: this.getStatus(shipment)
  };
}
```
- example usage
```shell
...
    ShipperClient.prototype.presentResponse = function(response, requestData, cb) {
return this.validateResponse(response, (function(_this) {
  return function(err, shipment) {
    var activities, adjustedEta, eta, presentedResponse, status, _ref, _ref1;
    if ((err != null) || (shipment == null)) {
      return cb(err);
    }
    _ref = _this.getActivitiesAndStatus(shipment), activities = _ref.activities, status = _ref.status;
    eta = _this.getEta(shipment);
    if (eta != null) {
      adjustedEta = moment(eta).utc().format().replace(/T00:00:00/, 'T23:59:59');
    }
    if (adjustedEta != null) {
      adjustedEta = moment(adjustedEta).toDate();
    }
...
```

#### <a name="apidoc.element.shipit.FedexClient.prototype.getDestination"></a>[function <span class="apidocSignatureSpan">shipit.FedexClient.prototype.</span>getDestination (shipment)](#apidoc.element.shipit.FedexClient.prototype.getDestination)
- description and source-code
```javascript
getDestination = function (shipment) {
  var _ref1;
  return this.presentAddress((_ref1 = shipment['DestinationAddress']) != null ? _ref1[0] : void 0);
}
```
- example usage
```shell
...
if (adjustedEta != null) {
  adjustedEta = moment(adjustedEta).toDate();
}
presentedResponse = {
  eta: adjustedEta,
  service: _this.getService(shipment),
  weight: _this.getWeight(shipment),
  destination: _this.getDestination(shipment),
  activities: activities,
  status: status
};
if ((requestData != null ? requestData.raw : void 0) != null) {
  if (requestData.raw) {
    presentedResponse.raw = response;
  }
...
```

#### <a name="apidoc.element.shipit.FedexClient.prototype.getEta"></a>[function <span class="apidocSignatureSpan">shipit.FedexClient.prototype.</span>getEta (shipment)](#apidoc.element.shipit.FedexClient.prototype.getEta)
- description and source-code
```javascript
getEta = function (shipment) {
  var ts, _ref1;
  ts = shipment != null ? (_ref1 = shipment['EstimatedDeliveryTimestamp']) != null ? _ref1[0] : void 0 : void 0;
  if (ts == null) {
    return;
  }
  return moment("" + ts.slice(0, 19) + "Z").toDate();
}
```
- example usage
```shell
...
      return this.validateResponse(response, (function(_this) {
return function(err, shipment) {
  var activities, adjustedEta, eta, presentedResponse, status, _ref, _ref1;
  if ((err != null) || (shipment == null)) {
    return cb(err);
  }
  _ref = _this.getActivitiesAndStatus(shipment), activities = _ref.activities, status = _ref.status;
  eta = _this.getEta(shipment);
  if (eta != null) {
    adjustedEta = moment(eta).utc().format().replace(/T00:00:00/, 'T23:59:59');
  }
  if (adjustedEta != null) {
    adjustedEta = moment(adjustedEta).toDate();
  }
  presentedResponse = {
...
```

#### <a name="apidoc.element.shipit.FedexClient.prototype.getService"></a>[function <span class="apidocSignatureSpan">shipit.FedexClient.prototype.</span>getService (shipment)](#apidoc.element.shipit.FedexClient.prototype.getService)
- description and source-code
```javascript
getService = function (shipment) {
  var _ref1;
  return shipment != null ? (_ref1 = shipment['ServiceInfo']) != null ? _ref1[0] : void 0 : void 0;
}
```
- example usage
```shell
...
  adjustedEta = moment(eta).utc().format().replace(/T00:00:00/, 'T23:59:59');
}
if (adjustedEta != null) {
  adjustedEta = moment(adjustedEta).toDate();
}
presentedResponse = {
  eta: adjustedEta,
  service: _this.getService(shipment),
  weight: _this.getWeight(shipment),
  destination: _this.getDestination(shipment),
  activities: activities,
  status: status
};
if ((requestData != null ? requestData.raw : void 0) != null) {
  if (requestData.raw) {
...
```

#### <a name="apidoc.element.shipit.FedexClient.prototype.getStatus"></a>[function <span class="apidocSignatureSpan">shipit.FedexClient.prototype.</span>getStatus (shipment)](#apidoc.element.shipit.FedexClient.prototype.getStatus)
- description and source-code
```javascript
getStatus = function (shipment) {
  var statusCode, _ref1;
  statusCode = shipment != null ? (_ref1 = shipment['StatusCode']) != null ? _ref1[0] : void 0 : void 0;
  if (statusCode == null) {
    return;
  }
  if (STATUS_MAP[statusCode] != null) {
    return STATUS_MAP[statusCode];
  } else {
    return ShipperClient.STATUS_TYPES.UNKNOWN;
  }
}
```
- example usage
```shell
...
        details: details
      };
      activities.push(activity);
    }
  }
  return {
    activities: activities,
    status: this.getStatus(shipment)
  };
};

A1Client.prototype.getEta = function(shipment) {
  var activities, firstActivity, _ref, _ref1, _ref2, _ref3;
  activities = ((_ref = shipment['TrackingEventHistory']) != null ? (_ref1 = _ref[0]) != null ? _ref1['TrackingEventDetail'] : void
 0 : void 0) || [];
  firstActivity = activities[activities.length - 1];
...
```

#### <a name="apidoc.element.shipit.FedexClient.prototype.getWeight"></a>[function <span class="apidocSignatureSpan">shipit.FedexClient.prototype.</span>getWeight (shipment)](#apidoc.element.shipit.FedexClient.prototype.getWeight)
- description and source-code
```javascript
getWeight = function (shipment) {
  var units, value, weightData, _ref1, _ref2, _ref3;
  weightData = shipment != null ? (_ref1 = shipment['PackageWeight']) != null ? _ref1[0] : void 0 : void 0;
  if (weightData == null) {
    return;
  }
  units = (_ref2 = weightData['Units']) != null ? _ref2[0] : void 0;
  value = (_ref3 = weightData['Value']) != null ? _ref3[0] : void 0;
  if ((units != null) && (value != null)) {
    return "" + value + " " + units;
  }
}
```
- example usage
```shell
...
}
if (adjustedEta != null) {
  adjustedEta = moment(adjustedEta).toDate();
}
presentedResponse = {
  eta: adjustedEta,
  service: _this.getService(shipment),
  weight: _this.getWeight(shipment),
  destination: _this.getDestination(shipment),
  activities: activities,
  status: status
};
if ((requestData != null ? requestData.raw : void 0) != null) {
  if (requestData.raw) {
    presentedResponse.raw = response;
...
```

#### <a name="apidoc.element.shipit.FedexClient.prototype.presentAddress"></a>[function <span class="apidocSignatureSpan">shipit.FedexClient.prototype.</span>presentAddress (address)](#apidoc.element.shipit.FedexClient.prototype.presentAddress)
- description and source-code
```javascript
presentAddress = function (address) {
  var city, countryCode, postalCode, stateCode, _ref1, _ref2, _ref3, _ref4;
  if (address == null) {
    return;
  }
  city = (_ref1 = address['City']) != null ? _ref1[0] : void 0;
  if (city != null) {
    city = city.replace('FEDEX SMARTPOST ', '');
  }
  stateCode = (_ref2 = address['StateOrProvinceCode']) != null ? _ref2[0] : void 0;
  countryCode = (_ref3 = address['CountryCode']) != null ? _ref3[0] : void 0;
  postalCode = (_ref4 = address['PostalCode']) != null ? _ref4[0] : void 0;
  return this.presentLocation({
    city: city,
    stateCode: stateCode,
    countryCode: countryCode,
    postalCode: postalCode
  });
}
```
- example usage
```shell
...
var activities, activity, datetime, details, event_time, location, rawActivities, rawActivity, raw_timestamp, status, timestamp,
_i, _len, _ref, _ref1, _ref2, _ref3, _ref4;
activities = [];
status = null;
rawActivities = (_ref = shipment['TrackingEventHistory']) != null ? (_ref1 = _ref[0]) != null ? _ref1['TrackingEventDetail'] : void
 0 : void 0;
_ref2 = rawActivities || [];
for (_i = 0, _len = _ref2.length; _i < _len; _i++) {
  rawActivity = _ref2[_i];
  location = this.presentAddress(rawActivity != null ? (_ref3 = rawActivity['EventLocation']) != null ? _ref3[0] : void 0 : void
 0);
  raw_timestamp = rawActivity != null ? rawActivity['EventDateTime'][0] : void 0;
  if (raw_timestamp != null) {
    event_time = moment(raw_timestamp);
    timestamp = event_time.toDate();
    datetime = raw_timestamp.slice(0, 19);
  }
  details = rawActivity != null ? (_ref4 = rawActivity['EventCodeDesc']) != null ? _ref4[0] : void 0 : void 0;
...
```

#### <a name="apidoc.element.shipit.FedexClient.prototype.requestOptions"></a>[function <span class="apidocSignatureSpan">shipit.FedexClient.prototype.</span>requestOptions (_arg)](#apidoc.element.shipit.FedexClient.prototype.requestOptions)
- description and source-code
```javascript
requestOptions = function (_arg) {
  var reference, trackingNumber;
  trackingNumber = _arg.trackingNumber, reference = _arg.reference;
  return {
    method: 'POST',
    uri: 'https://ws.fedex.com/xml',
    body: this.generateRequest(trackingNumber, reference)
  };
}
```
- example usage
```shell
...
      return cb(null, presentedResponse);
    };
  })(this));
};

ShipperClient.prototype.requestData = function(requestData, cb) {
  var opts, _ref;
  opts = this.requestOptions(requestData);
  opts.timeout = (requestData != null ? requestData.timeout : void 0) || ((_ref = this.options) != null ? _ref.timeout : void 0);
  return request(opts, (function(_this) {
    return function(err, response, body) {
      if ((body == null) || (err != null)) {
        return cb(err);
      }
      if (response.statusCode !== 200) {
...
```

#### <a name="apidoc.element.shipit.FedexClient.prototype.validateResponse"></a>[function <span class="apidocSignatureSpan">shipit.FedexClient.prototype.</span>validateResponse (response, cb)](#apidoc.element.shipit.FedexClient.prototype.validateResponse)
- description and source-code
```javascript
validateResponse = function (response, cb) {
  var handleResponse;
  handleResponse = function(xmlErr, trackResult) {
    var notifications, success, _ref1, _ref2, _ref3;
    if ((xmlErr != null) || (trackResult == null)) {
      return cb(xmlErr);
    }
    notifications = (_ref1 = trackResult['TrackReply']) != null ? _ref1['Notifications'] : void 0;
    success = find(notifications, function(notice) {
      var _ref2;
      return (notice != null ? (_ref2 = notice['Code']) != null ? _ref2[0] : void 0 : void 0) === '0';
    });
    if (!success) {
      return cb(notifications || 'invalid reply');
    }
    return cb(null, (_ref2 = trackResult['TrackReply']) != null ? (_ref3 = _ref2['TrackDetails']) != null ? _ref3[0] : void 0 :
void 0);
  };
  this.parser.reset();
  return this.parser.parseString(response, handleResponse);
}
```
- example usage
```shell
...
  if (postalCode != null ? postalCode.length : void 0) {
    address = address != null ? "" + address + " " + postalCode : postalCode;
  }
  return address;
};

ShipperClient.prototype.presentResponse = function(response, requestData, cb) {
  return this.validateResponse(response, (function(_this) {
    return function(err, shipment) {
      var activities, adjustedEta, eta, presentedResponse, status, _ref, _ref1;
      if ((err != null) || (shipment == null)) {
        return cb(err);
      }
      _ref = _this.getActivitiesAndStatus(shipment), activities = _ref.activities, status = _ref.status;
      eta = _this.getEta(shipment);
...
```



# <a name="apidoc.module.shipit.LasershipClient"></a>[module shipit.LasershipClient](#apidoc.module.shipit.LasershipClient)

#### <a name="apidoc.element.shipit.LasershipClient.LasershipClient"></a>[function <span class="apidocSignatureSpan">shipit.</span>LasershipClient (options)](#apidoc.element.shipit.LasershipClient.LasershipClient)
- description and source-code
```javascript
function LasershipClient(options) {
  this.options = options;
  LasershipClient.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.shipit.LasershipClient.prototype"></a>[module shipit.LasershipClient.prototype](#apidoc.module.shipit.LasershipClient.prototype)

#### <a name="apidoc.element.shipit.LasershipClient.prototype.constructor"></a>[function <span class="apidocSignatureSpan">shipit.LasershipClient.prototype.</span>constructor (options)](#apidoc.element.shipit.LasershipClient.prototype.constructor)
- description and source-code
```javascript
function LasershipClient(options) {
  this.options = options;
  LasershipClient.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.shipit.LasershipClient.prototype.getActivitiesAndStatus"></a>[function <span class="apidocSignatureSpan">shipit.LasershipClient.prototype.</span>getActivitiesAndStatus (shipment)](#apidoc.element.shipit.LasershipClient.prototype.getActivitiesAndStatus)
- description and source-code
```javascript
getActivitiesAndStatus = function (shipment) {
  var activities, activity, dateTime, details, location, rawActivities, rawActivity, status, timestamp, _i, _len, _ref;
  activities = [];
  status = null;
  rawActivities = shipment != null ? shipment['Events'] : void 0;
  _ref = rawActivities || [];
  for (_i = 0, _len = _ref.length; _i < _len; _i++) {
    rawActivity = _ref[_i];
    location = this.presentAddress(rawActivity);
    dateTime = rawActivity != null ? rawActivity['DateTime'] : void 0;
    if (dateTime != null) {
      timestamp = moment("" + dateTime + "Z").toDate();
    }
    details = rawActivity != null ? rawActivity['EventShortText'] : void 0;
    if ((details != null) && (timestamp != null)) {
      activity = {
        timestamp: timestamp,
        location: location,
        details: details
      };
      activities.push(activity);
    }
    if (!status) {
      status = this.presentStatus(rawActivity != null ? rawActivity['EventType'] : void 0);
    }
  }
  return {
    activities: activities,
    status: status
  };
}
```
- example usage
```shell
...
    ShipperClient.prototype.presentResponse = function(response, requestData, cb) {
return this.validateResponse(response, (function(_this) {
  return function(err, shipment) {
    var activities, adjustedEta, eta, presentedResponse, status, _ref, _ref1;
    if ((err != null) || (shipment == null)) {
      return cb(err);
    }
    _ref = _this.getActivitiesAndStatus(shipment), activities = _ref.activities, status = _ref.status;
    eta = _this.getEta(shipment);
    if (eta != null) {
      adjustedEta = moment(eta).utc().format().replace(/T00:00:00/, 'T23:59:59');
    }
    if (adjustedEta != null) {
      adjustedEta = moment(adjustedEta).toDate();
    }
...
```

#### <a name="apidoc.element.shipit.LasershipClient.prototype.getDestination"></a>[function <span class="apidocSignatureSpan">shipit.LasershipClient.prototype.</span>getDestination (shipment)](#apidoc.element.shipit.LasershipClient.prototype.getDestination)
- description and source-code
```javascript
getDestination = function (shipment) {
  var destination;
  destination = shipment != null ? shipment['Destination'] : void 0;
  if (destination == null) {
    return;
  }
  return this.presentAddress(destination);
}
```
- example usage
```shell
...
if (adjustedEta != null) {
  adjustedEta = moment(adjustedEta).toDate();
}
presentedResponse = {
  eta: adjustedEta,
  service: _this.getService(shipment),
  weight: _this.getWeight(shipment),
  destination: _this.getDestination(shipment),
  activities: activities,
  status: status
};
if ((requestData != null ? requestData.raw : void 0) != null) {
  if (requestData.raw) {
    presentedResponse.raw = response;
  }
...
```

#### <a name="apidoc.element.shipit.LasershipClient.prototype.getEta"></a>[function <span class="apidocSignatureSpan">shipit.LasershipClient.prototype.</span>getEta (shipment)](#apidoc.element.shipit.LasershipClient.prototype.getEta)
- description and source-code
```javascript
getEta = function (shipment) {
  if ((shipment != null ? shipment['EstimatedDeliveryDate'] : void 0) == null) {
    return;
  }
  return moment("" + shipment['EstimatedDeliveryDate'] + "T00:00:00Z").toDate();
}
```
- example usage
```shell
...
      return this.validateResponse(response, (function(_this) {
return function(err, shipment) {
  var activities, adjustedEta, eta, presentedResponse, status, _ref, _ref1;
  if ((err != null) || (shipment == null)) {
    return cb(err);
  }
  _ref = _this.getActivitiesAndStatus(shipment), activities = _ref.activities, status = _ref.status;
  eta = _this.getEta(shipment);
  if (eta != null) {
    adjustedEta = moment(eta).utc().format().replace(/T00:00:00/, 'T23:59:59');
  }
  if (adjustedEta != null) {
    adjustedEta = moment(adjustedEta).toDate();
  }
  presentedResponse = {
...
```

#### <a name="apidoc.element.shipit.LasershipClient.prototype.getService"></a>[function <span class="apidocSignatureSpan">shipit.LasershipClient.prototype.</span>getService (shipment)](#apidoc.element.shipit.LasershipClient.prototype.getService)
- description and source-code
```javascript
getService = function (shipment) {}
```
- example usage
```shell
...
  adjustedEta = moment(eta).utc().format().replace(/T00:00:00/, 'T23:59:59');
}
if (adjustedEta != null) {
  adjustedEta = moment(adjustedEta).toDate();
}
presentedResponse = {
  eta: adjustedEta,
  service: _this.getService(shipment),
  weight: _this.getWeight(shipment),
  destination: _this.getDestination(shipment),
  activities: activities,
  status: status
};
if ((requestData != null ? requestData.raw : void 0) != null) {
  if (requestData.raw) {
...
```

#### <a name="apidoc.element.shipit.LasershipClient.prototype.getWeight"></a>[function <span class="apidocSignatureSpan">shipit.LasershipClient.prototype.</span>getWeight (shipment)](#apidoc.element.shipit.LasershipClient.prototype.getWeight)
- description and source-code
```javascript
getWeight = function (shipment) {
  var piece, units, weight, _ref;
  if (!(shipment != null ? (_ref = shipment['Pieces']) != null ? _ref.length : void 0 : void 0)) {
    return;
  }
  piece = shipment['Pieces'][0];
  weight = "" + piece['Weight'];
  units = piece['WeightUnit'];
  if (units != null) {
    weight = "" + weight + " " + units;
  }
  return weight;
}
```
- example usage
```shell
...
}
if (adjustedEta != null) {
  adjustedEta = moment(adjustedEta).toDate();
}
presentedResponse = {
  eta: adjustedEta,
  service: _this.getService(shipment),
  weight: _this.getWeight(shipment),
  destination: _this.getDestination(shipment),
  activities: activities,
  status: status
};
if ((requestData != null ? requestData.raw : void 0) != null) {
  if (requestData.raw) {
    presentedResponse.raw = response;
...
```

#### <a name="apidoc.element.shipit.LasershipClient.prototype.presentAddress"></a>[function <span class="apidocSignatureSpan">shipit.LasershipClient.prototype.</span>presentAddress (address)](#apidoc.element.shipit.LasershipClient.prototype.presentAddress)
- description and source-code
```javascript
presentAddress = function (address) {
  var city, countryCode, postalCode, stateCode;
  city = address['City'];
  stateCode = address['State'];
  postalCode = address['PostalCode'];
  countryCode = address['Country'];
  return this.presentLocation({
    city: city,
    stateCode: stateCode,
    countryCode: countryCode,
    postalCode: postalCode
  });
}
```
- example usage
```shell
...
var activities, activity, datetime, details, event_time, location, rawActivities, rawActivity, raw_timestamp, status, timestamp,
_i, _len, _ref, _ref1, _ref2, _ref3, _ref4;
activities = [];
status = null;
rawActivities = (_ref = shipment['TrackingEventHistory']) != null ? (_ref1 = _ref[0]) != null ? _ref1['TrackingEventDetail'] : void
 0 : void 0;
_ref2 = rawActivities || [];
for (_i = 0, _len = _ref2.length; _i < _len; _i++) {
  rawActivity = _ref2[_i];
  location = this.presentAddress(rawActivity != null ? (_ref3 = rawActivity['EventLocation']) != null ? _ref3[0] : void 0 : void
 0);
  raw_timestamp = rawActivity != null ? rawActivity['EventDateTime'][0] : void 0;
  if (raw_timestamp != null) {
    event_time = moment(raw_timestamp);
    timestamp = event_time.toDate();
    datetime = raw_timestamp.slice(0, 19);
  }
  details = rawActivity != null ? (_ref4 = rawActivity['EventCodeDesc']) != null ? _ref4[0] : void 0 : void 0;
...
```

#### <a name="apidoc.element.shipit.LasershipClient.prototype.presentStatus"></a>[function <span class="apidocSignatureSpan">shipit.LasershipClient.prototype.</span>presentStatus (eventType)](#apidoc.element.shipit.LasershipClient.prototype.presentStatus)
- description and source-code
```javascript
presentStatus = function (eventType) {
  if (eventType != null) {
    return STATUS_MAP[eventType];
  }
}
```
- example usage
```shell
...
if (data == null) {
  return {
    activities: activities,
    status: status
  };
}
$ = data.$, rightNow = data.rightNow;
status = this.presentStatus($(".latest-event-status").text());
rows = $("div[data-a-expander-name=event-history-list] .a-box");
for (_i = 0, _len = rows.length; _i < _len; _i++) {
  row = rows[_i];
  columns = $($(row).find(".a-row")[0]).children('.a-column');
  if (columns.length === 2) {
    timeOfDay = $(columns[0]).text().trim();
    if (timeOfDay === '--') {
...
```

#### <a name="apidoc.element.shipit.LasershipClient.prototype.requestOptions"></a>[function <span class="apidocSignatureSpan">shipit.LasershipClient.prototype.</span>requestOptions (_arg)](#apidoc.element.shipit.LasershipClient.prototype.requestOptions)
- description and source-code
```javascript
requestOptions = function (_arg) {
  var trackingNumber;
  trackingNumber = _arg.trackingNumber;
  return {
    method: 'GET',
    uri: "http://www.lasership.com/track/" + trackingNumber + "/json"
  };
}
```
- example usage
```shell
...
      return cb(null, presentedResponse);
    };
  })(this));
};

ShipperClient.prototype.requestData = function(requestData, cb) {
  var opts, _ref;
  opts = this.requestOptions(requestData);
  opts.timeout = (requestData != null ? requestData.timeout : void 0) || ((_ref = this.options) != null ? _ref.timeout : void 0);
  return request(opts, (function(_this) {
    return function(err, response, body) {
      if ((body == null) || (err != null)) {
        return cb(err);
      }
      if (response.statusCode !== 200) {
...
```

#### <a name="apidoc.element.shipit.LasershipClient.prototype.validateResponse"></a>[function <span class="apidocSignatureSpan">shipit.LasershipClient.prototype.</span>validateResponse (response, cb)](#apidoc.element.shipit.LasershipClient.prototype.validateResponse)
- description and source-code
```javascript
validateResponse = function (response, cb) {
  response = JSON.parse(response);
  if (response['Events'] == null) {
    return cb({
      error: 'missing events'
    });
  }
  return cb(null, response);
}
```
- example usage
```shell
...
  if (postalCode != null ? postalCode.length : void 0) {
    address = address != null ? "" + address + " " + postalCode : postalCode;
  }
  return address;
};

ShipperClient.prototype.presentResponse = function(response, requestData, cb) {
  return this.validateResponse(response, (function(_this) {
    return function(err, shipment) {
      var activities, adjustedEta, eta, presentedResponse, status, _ref, _ref1;
      if ((err != null) || (shipment == null)) {
        return cb(err);
      }
      _ref = _this.getActivitiesAndStatus(shipment), activities = _ref.activities, status = _ref.status;
      eta = _this.getEta(shipment);
...
```



# <a name="apidoc.module.shipit.OnTracClient"></a>[module shipit.OnTracClient](#apidoc.module.shipit.OnTracClient)

#### <a name="apidoc.element.shipit.OnTracClient.OnTracClient"></a>[function <span class="apidocSignatureSpan">shipit.</span>OnTracClient (options)](#apidoc.element.shipit.OnTracClient.OnTracClient)
- description and source-code
```javascript
function OnTracClient(options) {
  this.options = options;
  OnTracClient.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.shipit.OnTracClient.prototype"></a>[module shipit.OnTracClient.prototype](#apidoc.module.shipit.OnTracClient.prototype)

#### <a name="apidoc.element.shipit.OnTracClient.prototype.constructor"></a>[function <span class="apidocSignatureSpan">shipit.OnTracClient.prototype.</span>constructor (options)](#apidoc.element.shipit.OnTracClient.prototype.constructor)
- description and source-code
```javascript
function OnTracClient(options) {
  this.options = options;
  OnTracClient.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.shipit.OnTracClient.prototype.extractSummaryField"></a>[function <span class="apidocSignatureSpan">shipit.OnTracClient.prototype.</span>extractSummaryField (shipment, name)](#apidoc.element.shipit.OnTracClient.prototype.extractSummaryField)
- description and source-code
```javascript
extractSummaryField = function (shipment, name) {
  var $, value;
  value = null;
  $ = shipment;
  if ($ == null) {
    return;
  }
  $('td[bgcolor="#ffd204"]').each(function(index, element) {
    var regex, _ref1, _ref2;
    regex = new RegExp(name);
    if (!regex.test($(element).text())) {
      return;
    }
    value = (_ref1 = $(element).next()) != null ? (_ref2 = _ref1.text()) != null ? _ref2.trim() : void 0 : void 0;
    return false;
  });
  return value;
}
```
- example usage
```shell
...
  if (!(eta != null ? eta.length : void 0)) {
    return;
  }
  return moment("" + eta + " 23:59:59 +00:00").toDate();
};

DhlGmClient.prototype.getService = function(data) {
  return this.extractSummaryField(data, 'Service');
};

DhlGmClient.prototype.getWeight = function(data) {
  return this.extractSummaryField(data, 'Weight');
};

DhlGmClient.prototype.presentStatus = function(details) {
...
```

#### <a name="apidoc.element.shipit.OnTracClient.prototype.getActivitiesAndStatus"></a>[function <span class="apidocSignatureSpan">shipit.OnTracClient.prototype.</span>getActivitiesAndStatus (shipment)](#apidoc.element.shipit.OnTracClient.prototype.getActivitiesAndStatus)
- description and source-code
```javascript
getActivitiesAndStatus = function (shipment) {
  var $, activities, status;
  activities = [];
  status = this.presentStatus(this.extractSummaryField(shipment, 'Delivery Status'));
  $ = shipment;
  if ($ == null) {
    return {
      activities: activities,
      status: status
    };
  }
  $("#trkdetail table table").children('tr').each((function(_this) {
    return function(rowIndex, row) {
      var details, fields, location, timestamp;
      if (!(rowIndex > 0)) {
        return;
      }
      fields = [];
      $(row).find('td').each(function(colIndex, col) {
        return fields.push($(col).text().trim());
      });
      if (fields.length) {
        if (fields[0].length) {
          details = upperCaseFirst(lowerCase(fields[0]));
        }
        timestamp = _this.presentTimestamp(fields[1]);
        if (fields[2].length) {
          location = _this.presentAddress(fields[2]);
        }
        if ((details != null) && (timestamp != null)) {
          return activities.unshift({
            details: details,
            timestamp: timestamp,
            location: location
          });
        }
      }
    };
  })(this));
  return {
    activities: activities,
    status: status
  };
}
```
- example usage
```shell
...
    ShipperClient.prototype.presentResponse = function(response, requestData, cb) {
return this.validateResponse(response, (function(_this) {
  return function(err, shipment) {
    var activities, adjustedEta, eta, presentedResponse, status, _ref, _ref1;
    if ((err != null) || (shipment == null)) {
      return cb(err);
    }
    _ref = _this.getActivitiesAndStatus(shipment), activities = _ref.activities, status = _ref.status;
    eta = _this.getEta(shipment);
    if (eta != null) {
      adjustedEta = moment(eta).utc().format().replace(/T00:00:00/, 'T23:59:59');
    }
    if (adjustedEta != null) {
      adjustedEta = moment(adjustedEta).toDate();
    }
...
```

#### <a name="apidoc.element.shipit.OnTracClient.prototype.getDestination"></a>[function <span class="apidocSignatureSpan">shipit.OnTracClient.prototype.</span>getDestination (shipment)](#apidoc.element.shipit.OnTracClient.prototype.getDestination)
- description and source-code
```javascript
getDestination = function (shipment) {
  var destination;
  destination = this.extractSummaryField(shipment, 'Deliver To');
  return this.presentLocationString(destination);
}
```
- example usage
```shell
...
if (adjustedEta != null) {
  adjustedEta = moment(adjustedEta).toDate();
}
presentedResponse = {
  eta: adjustedEta,
  service: _this.getService(shipment),
  weight: _this.getWeight(shipment),
  destination: _this.getDestination(shipment),
  activities: activities,
  status: status
};
if ((requestData != null ? requestData.raw : void 0) != null) {
  if (requestData.raw) {
    presentedResponse.raw = response;
  }
...
```

#### <a name="apidoc.element.shipit.OnTracClient.prototype.getEta"></a>[function <span class="apidocSignatureSpan">shipit.OnTracClient.prototype.</span>getEta (shipment)](#apidoc.element.shipit.OnTracClient.prototype.getEta)
- description and source-code
```javascript
getEta = function (shipment) {
  var eta, regexMatch;
  eta = this.extractSummaryField(shipment, 'Service Commitment');
  if (eta == null) {
    return;
  }
  regexMatch = eta.match('(.*) by (.*)');
  if ((regexMatch != null ? regexMatch.length : void 0) > 1) {
    eta = "" + regexMatch[1] + " 23:59:59 +00:00";
  }
  return moment(eta).toDate();
}
```
- example usage
```shell
...
      return this.validateResponse(response, (function(_this) {
return function(err, shipment) {
  var activities, adjustedEta, eta, presentedResponse, status, _ref, _ref1;
  if ((err != null) || (shipment == null)) {
    return cb(err);
  }
  _ref = _this.getActivitiesAndStatus(shipment), activities = _ref.activities, status = _ref.status;
  eta = _this.getEta(shipment);
  if (eta != null) {
    adjustedEta = moment(eta).utc().format().replace(/T00:00:00/, 'T23:59:59');
  }
  if (adjustedEta != null) {
    adjustedEta = moment(adjustedEta).toDate();
  }
  presentedResponse = {
...
```

#### <a name="apidoc.element.shipit.OnTracClient.prototype.getService"></a>[function <span class="apidocSignatureSpan">shipit.OnTracClient.prototype.</span>getService (shipment)](#apidoc.element.shipit.OnTracClient.prototype.getService)
- description and source-code
```javascript
getService = function (shipment) {
  var service;
  service = this.extractSummaryField(shipment, 'Service Code');
  if (service == null) {
    return;
  }
  return titleCase(service);
}
```
- example usage
```shell
...
  adjustedEta = moment(eta).utc().format().replace(/T00:00:00/, 'T23:59:59');
}
if (adjustedEta != null) {
  adjustedEta = moment(adjustedEta).toDate();
}
presentedResponse = {
  eta: adjustedEta,
  service: _this.getService(shipment),
  weight: _this.getWeight(shipment),
  destination: _this.getDestination(shipment),
  activities: activities,
  status: status
};
if ((requestData != null ? requestData.raw : void 0) != null) {
  if (requestData.raw) {
...
```

#### <a name="apidoc.element.shipit.OnTracClient.prototype.getWeight"></a>[function <span class="apidocSignatureSpan">shipit.OnTracClient.prototype.</span>getWeight (shipment)](#apidoc.element.shipit.OnTracClient.prototype.getWeight)
- description and source-code
```javascript
getWeight = function (shipment) {
  return this.extractSummaryField(shipment, 'Weight');
}
```
- example usage
```shell
...
}
if (adjustedEta != null) {
  adjustedEta = moment(adjustedEta).toDate();
}
presentedResponse = {
  eta: adjustedEta,
  service: _this.getService(shipment),
  weight: _this.getWeight(shipment),
  destination: _this.getDestination(shipment),
  activities: activities,
  status: status
};
if ((requestData != null ? requestData.raw : void 0) != null) {
  if (requestData.raw) {
    presentedResponse.raw = response;
...
```

#### <a name="apidoc.element.shipit.OnTracClient.prototype.presentAddress"></a>[function <span class="apidocSignatureSpan">shipit.OnTracClient.prototype.</span>presentAddress (location)](#apidoc.element.shipit.OnTracClient.prototype.presentAddress)
- description and source-code
```javascript
presentAddress = function (location) {
  var addressState;
  addressState = LOCATION_STATES[location];
  if (addressState != null) {
    return "" + location + ", " + addressState;
  } else {
    return location;
  }
}
```
- example usage
```shell
...
var activities, activity, datetime, details, event_time, location, rawActivities, rawActivity, raw_timestamp, status, timestamp,
_i, _len, _ref, _ref1, _ref2, _ref3, _ref4;
activities = [];
status = null;
rawActivities = (_ref = shipment['TrackingEventHistory']) != null ? (_ref1 = _ref[0]) != null ? _ref1['TrackingEventDetail'] : void
 0 : void 0;
_ref2 = rawActivities || [];
for (_i = 0, _len = _ref2.length; _i < _len; _i++) {
  rawActivity = _ref2[_i];
  location = this.presentAddress(rawActivity != null ? (_ref3 = rawActivity['EventLocation']) != null ? _ref3[0] : void 0 : void
 0);
  raw_timestamp = rawActivity != null ? rawActivity['EventDateTime'][0] : void 0;
  if (raw_timestamp != null) {
    event_time = moment(raw_timestamp);
    timestamp = event_time.toDate();
    datetime = raw_timestamp.slice(0, 19);
  }
  details = rawActivity != null ? (_ref4 = rawActivity['EventCodeDesc']) != null ? _ref4[0] : void 0 : void 0;
...
```

#### <a name="apidoc.element.shipit.OnTracClient.prototype.presentStatus"></a>[function <span class="apidocSignatureSpan">shipit.OnTracClient.prototype.</span>presentStatus (status)](#apidoc.element.shipit.OnTracClient.prototype.presentStatus)
- description and source-code
```javascript
presentStatus = function (status) {
  var statusType, _ref1;
  status = status != null ? (_ref1 = status.replace('DETAILS', '')) != null ? _ref1.trim() : void 0 : void 0;
  if (!(status != null ? status.length : void 0)) {
    return ShipperClient.STATUS_TYPES.UNKNOWN;
  }
  statusType = STATUS_MAP[status];
  if (statusType != null) {
    return statusType;
  } else {
    return ShipperClient.STATUS_TYPES.UNKNOWN;
  }
}
```
- example usage
```shell
...
if (data == null) {
  return {
    activities: activities,
    status: status
  };
}
$ = data.$, rightNow = data.rightNow;
status = this.presentStatus($(".latest-event-status").text());
rows = $("div[data-a-expander-name=event-history-list] .a-box");
for (_i = 0, _len = rows.length; _i < _len; _i++) {
  row = rows[_i];
  columns = $($(row).find(".a-row")[0]).children('.a-column');
  if (columns.length === 2) {
    timeOfDay = $(columns[0]).text().trim();
    if (timeOfDay === '--') {
...
```

#### <a name="apidoc.element.shipit.OnTracClient.prototype.presentTimestamp"></a>[function <span class="apidocSignatureSpan">shipit.OnTracClient.prototype.</span>presentTimestamp (ts)](#apidoc.element.shipit.OnTracClient.prototype.presentTimestamp)
- description and source-code
```javascript
presentTimestamp = function (ts) {
  if (ts == null) {
    return;
  }
  ts = ts.replace(/AM$/, ' AM').replace(/PM$/, ' PM');
  return moment("" + ts + " +0000").toDate();
}
```
- example usage
```shell
...
}
rawActivities.reverse();
_ref1 = rawActivities || [];
for (_i = 0, _len = _ref1.length; _i < _len; _i++) {
  rawActivity = _ref1[_i];
  rawLocation = (_ref2 = rawActivity['ServiceArea']) != null ? (_ref3 = _ref2[0]) != null ? (_ref4 = _ref3['Description']) != null
 ? _ref4[0] : void 0 : void 0 : void 0;
  location = this.presentAddress(rawLocation);
  timestamp = this.presentTimestamp((_ref5 = rawActivity['Date']) != null ? _ref5[0] : void 0, (_ref6 = rawActivity['Time']) !=
null ? _ref6[0] : void 0);
  details = this.presentDetails(rawLocation, (_ref7 = rawActivity['ServiceEvent']) != null ? (_ref8 = _ref7[0]) != null ? (_ref9
 = _ref8['Description']) != null ? _ref9[0] : void 0 : void 0 : void 0);
  if ((details != null) && (timestamp != null)) {
    details = details.slice(-1) === '.' ? details.slice(0, -1) : details;
    activity = {
      timestamp: timestamp,
      location: location,
      details: details
...
```

#### <a name="apidoc.element.shipit.OnTracClient.prototype.requestOptions"></a>[function <span class="apidocSignatureSpan">shipit.OnTracClient.prototype.</span>requestOptions (_arg)](#apidoc.element.shipit.OnTracClient.prototype.requestOptions)
- description and source-code
```javascript
requestOptions = function (_arg) {
  var trackingNumber;
  trackingNumber = _arg.trackingNumber;
  return {
    method: 'GET',
    uri: "https://www.ontrac.com/trackingdetail.asp?tracking=" + trackingNumber + "&run=0"
  };
}
```
- example usage
```shell
...
      return cb(null, presentedResponse);
    };
  })(this));
};

ShipperClient.prototype.requestData = function(requestData, cb) {
  var opts, _ref;
  opts = this.requestOptions(requestData);
  opts.timeout = (requestData != null ? requestData.timeout : void 0) || ((_ref = this.options) != null ? _ref.timeout : void 0);
  return request(opts, (function(_this) {
    return function(err, response, body) {
      if ((body == null) || (err != null)) {
        return cb(err);
      }
      if (response.statusCode !== 200) {
...
```

#### <a name="apidoc.element.shipit.OnTracClient.prototype.validateResponse"></a>[function <span class="apidocSignatureSpan">shipit.OnTracClient.prototype.</span>validateResponse (response, cb)](#apidoc.element.shipit.OnTracClient.prototype.validateResponse)
- description and source-code
```javascript
validateResponse = function (response, cb) {
  var data;
  data = load(response, {
    normalizeWhitespace: true
  });
  return cb(null, data);
}
```
- example usage
```shell
...
  if (postalCode != null ? postalCode.length : void 0) {
    address = address != null ? "" + address + " " + postalCode : postalCode;
  }
  return address;
};

ShipperClient.prototype.presentResponse = function(response, requestData, cb) {
  return this.validateResponse(response, (function(_this) {
    return function(err, shipment) {
      var activities, adjustedEta, eta, presentedResponse, status, _ref, _ref1;
      if ((err != null) || (shipment == null)) {
        return cb(err);
      }
      _ref = _this.getActivitiesAndStatus(shipment), activities = _ref.activities, status = _ref.status;
      eta = _this.getEta(shipment);
...
```



# <a name="apidoc.module.shipit.PrestigeClient"></a>[module shipit.PrestigeClient](#apidoc.module.shipit.PrestigeClient)

#### <a name="apidoc.element.shipit.PrestigeClient.PrestigeClient"></a>[function <span class="apidocSignatureSpan">shipit.</span>PrestigeClient (options)](#apidoc.element.shipit.PrestigeClient.PrestigeClient)
- description and source-code
```javascript
function PrestigeClient(options) {
  this.options = options;
  PrestigeClient.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.shipit.PrestigeClient.prototype"></a>[module shipit.PrestigeClient.prototype](#apidoc.module.shipit.PrestigeClient.prototype)

#### <a name="apidoc.element.shipit.PrestigeClient.prototype.constructor"></a>[function <span class="apidocSignatureSpan">shipit.PrestigeClient.prototype.</span>constructor (options)](#apidoc.element.shipit.PrestigeClient.prototype.constructor)
- description and source-code
```javascript
function PrestigeClient(options) {
  this.options = options;
  PrestigeClient.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.shipit.PrestigeClient.prototype.getActivitiesAndStatus"></a>[function <span class="apidocSignatureSpan">shipit.PrestigeClient.prototype.</span>getActivitiesAndStatus (shipment)](#apidoc.element.shipit.PrestigeClient.prototype.getActivitiesAndStatus)
- description and source-code
```javascript
getActivitiesAndStatus = function (shipment) {
  var activities, activity, dateTime, details, location, rawActivities, rawActivity, status, timestamp, _i, _len, _ref;
  activities = [];
  status = null;
  rawActivities = shipment != null ? shipment['TrackingEventHistory'] : void 0;
  _ref = rawActivities || [];
  for (_i = 0, _len = _ref.length; _i < _len; _i++) {
    rawActivity = _ref[_i];
    location = this.presentAddress('EL', rawActivity);
    dateTime = "" + (rawActivity != null ? rawActivity['serverDate'] : void 0) + " " + (rawActivity != null ? rawActivity['serverTime
'] : void 0);
    timestamp = moment("" + dateTime + " +00:00").toDate();
    details = rawActivity != null ? rawActivity['EventCodeDesc'] : void 0;
    if ((details != null) && (timestamp != null)) {
      activity = {
        timestamp: timestamp,
        location: location,
        details: details
      };
      activities.push(activity);
    }
    if (!status) {
      status = this.presentStatus(rawActivity != null ? rawActivity['EventCode'] : void 0);
    }
  }
  return {
    activities: activities,
    status: status
  };
}
```
- example usage
```shell
...
    ShipperClient.prototype.presentResponse = function(response, requestData, cb) {
return this.validateResponse(response, (function(_this) {
  return function(err, shipment) {
    var activities, adjustedEta, eta, presentedResponse, status, _ref, _ref1;
    if ((err != null) || (shipment == null)) {
      return cb(err);
    }
    _ref = _this.getActivitiesAndStatus(shipment), activities = _ref.activities, status = _ref.status;
    eta = _this.getEta(shipment);
    if (eta != null) {
      adjustedEta = moment(eta).utc().format().replace(/T00:00:00/, 'T23:59:59');
    }
    if (adjustedEta != null) {
      adjustedEta = moment(adjustedEta).toDate();
    }
...
```

#### <a name="apidoc.element.shipit.PrestigeClient.prototype.getDestination"></a>[function <span class="apidocSignatureSpan">shipit.PrestigeClient.prototype.</span>getDestination (shipment)](#apidoc.element.shipit.PrestigeClient.prototype.getDestination)
- description and source-code
```javascript
getDestination = function (shipment) {
  var _ref;
  return this.presentAddress('PD', shipment != null ? (_ref = shipment['TrackingEventHistory']) != null ? _ref[0] : void 0 : void
 0);
}
```
- example usage
```shell
...
if (adjustedEta != null) {
  adjustedEta = moment(adjustedEta).toDate();
}
presentedResponse = {
  eta: adjustedEta,
  service: _this.getService(shipment),
  weight: _this.getWeight(shipment),
  destination: _this.getDestination(shipment),
  activities: activities,
  status: status
};
if ((requestData != null ? requestData.raw : void 0) != null) {
  if (requestData.raw) {
    presentedResponse.raw = response;
  }
...
```

#### <a name="apidoc.element.shipit.PrestigeClient.prototype.getEta"></a>[function <span class="apidocSignatureSpan">shipit.PrestigeClient.prototype.</span>getEta (shipment)](#apidoc.element.shipit.PrestigeClient.prototype.getEta)
- description and source-code
```javascript
getEta = function (shipment) {
  var eta, _ref, _ref1;
  eta = shipment != null ? (_ref = shipment['TrackingEventHistory']) != null ? (_ref1 = _ref[0]) != null ? _ref1['EstimatedDeliveryDate
'] : void 0 : void 0 : void 0;
  if (!(eta != null ? eta.length : void 0)) {
    return;
  }
  eta = "" + eta + " 00:00 +00:00";
  return moment(eta, 'MM/DD/YYYY HH:mm ZZ').toDate();
}
```
- example usage
```shell
...
      return this.validateResponse(response, (function(_this) {
return function(err, shipment) {
  var activities, adjustedEta, eta, presentedResponse, status, _ref, _ref1;
  if ((err != null) || (shipment == null)) {
    return cb(err);
  }
  _ref = _this.getActivitiesAndStatus(shipment), activities = _ref.activities, status = _ref.status;
  eta = _this.getEta(shipment);
  if (eta != null) {
    adjustedEta = moment(eta).utc().format().replace(/T00:00:00/, 'T23:59:59');
  }
  if (adjustedEta != null) {
    adjustedEta = moment(adjustedEta).toDate();
  }
  presentedResponse = {
...
```

#### <a name="apidoc.element.shipit.PrestigeClient.prototype.getService"></a>[function <span class="apidocSignatureSpan">shipit.PrestigeClient.prototype.</span>getService (shipment)](#apidoc.element.shipit.PrestigeClient.prototype.getService)
- description and source-code
```javascript
getService = function (shipment) {}
```
- example usage
```shell
...
  adjustedEta = moment(eta).utc().format().replace(/T00:00:00/, 'T23:59:59');
}
if (adjustedEta != null) {
  adjustedEta = moment(adjustedEta).toDate();
}
presentedResponse = {
  eta: adjustedEta,
  service: _this.getService(shipment),
  weight: _this.getWeight(shipment),
  destination: _this.getDestination(shipment),
  activities: activities,
  status: status
};
if ((requestData != null ? requestData.raw : void 0) != null) {
  if (requestData.raw) {
...
```

#### <a name="apidoc.element.shipit.PrestigeClient.prototype.getWeight"></a>[function <span class="apidocSignatureSpan">shipit.PrestigeClient.prototype.</span>getWeight (shipment)](#apidoc.element.shipit.PrestigeClient.prototype.getWeight)
- description and source-code
```javascript
getWeight = function (shipment) {
  var piece, units, weight, _ref;
  if (!(shipment != null ? (_ref = shipment['Pieces']) != null ? _ref.length : void 0 : void 0)) {
    return;
  }
  piece = shipment['Pieces'][0];
  weight = "" + piece['Weight'];
  units = piece['WeightUnit'];
  if (units != null) {
    weight = "" + weight + " " + units;
  }
  return weight;
}
```
- example usage
```shell
...
}
if (adjustedEta != null) {
  adjustedEta = moment(adjustedEta).toDate();
}
presentedResponse = {
  eta: adjustedEta,
  service: _this.getService(shipment),
  weight: _this.getWeight(shipment),
  destination: _this.getDestination(shipment),
  activities: activities,
  status: status
};
if ((requestData != null ? requestData.raw : void 0) != null) {
  if (requestData.raw) {
    presentedResponse.raw = response;
...
```

#### <a name="apidoc.element.shipit.PrestigeClient.prototype.presentAddress"></a>[function <span class="apidocSignatureSpan">shipit.PrestigeClient.prototype.</span>presentAddress (prefix, event)](#apidoc.element.shipit.PrestigeClient.prototype.presentAddress)
- description and source-code
```javascript
presentAddress = function (prefix, event) {
  var address, city, postalCode, stateCode;
  if (event == null) {
    return;
  }
  address = reduce(ADDR_ATTRS, (function(d, v) {
    d[v] = event["" + prefix + v];
    return d;
  }), {});
  city = address['City'];
  stateCode = address['State'];
  postalCode = address['Zip'];
  return this.presentLocation({
    city: city,
    stateCode: stateCode,
    postalCode: postalCode
  });
}
```
- example usage
```shell
...
var activities, activity, datetime, details, event_time, location, rawActivities, rawActivity, raw_timestamp, status, timestamp,
_i, _len, _ref, _ref1, _ref2, _ref3, _ref4;
activities = [];
status = null;
rawActivities = (_ref = shipment['TrackingEventHistory']) != null ? (_ref1 = _ref[0]) != null ? _ref1['TrackingEventDetail'] : void
 0 : void 0;
_ref2 = rawActivities || [];
for (_i = 0, _len = _ref2.length; _i < _len; _i++) {
  rawActivity = _ref2[_i];
  location = this.presentAddress(rawActivity != null ? (_ref3 = rawActivity['EventLocation']) != null ? _ref3[0] : void 0 : void
 0);
  raw_timestamp = rawActivity != null ? rawActivity['EventDateTime'][0] : void 0;
  if (raw_timestamp != null) {
    event_time = moment(raw_timestamp);
    timestamp = event_time.toDate();
    datetime = raw_timestamp.slice(0, 19);
  }
  details = rawActivity != null ? (_ref4 = rawActivity['EventCodeDesc']) != null ? _ref4[0] : void 0 : void 0;
...
```

#### <a name="apidoc.element.shipit.PrestigeClient.prototype.presentStatus"></a>[function <span class="apidocSignatureSpan">shipit.PrestigeClient.prototype.</span>presentStatus (eventType)](#apidoc.element.shipit.PrestigeClient.prototype.presentStatus)
- description and source-code
```javascript
presentStatus = function (eventType) {
  var codeStr, eventCode, status, _ref;
  codeStr = (_ref = eventType.match('EVENT_(.*)$')) != null ? _ref[1] : void 0;
  if (!(codeStr != null ? codeStr.length : void 0)) {
    return;
  }
  eventCode = parseInt(codeStr);
  if (isNaN(eventCode)) {
    return;
  }
  status = STATUS_MAP[eventCode];
  if (status != null) {
    return status;
  }
  if (eventCode < 300 && eventCode > 101) {
    return ShipperClient.STATUS_TYPES.EN_ROUTE;
  }
}
```
- example usage
```shell
...
if (data == null) {
  return {
    activities: activities,
    status: status
  };
}
$ = data.$, rightNow = data.rightNow;
status = this.presentStatus($(".latest-event-status").text());
rows = $("div[data-a-expander-name=event-history-list] .a-box");
for (_i = 0, _len = rows.length; _i < _len; _i++) {
  row = rows[_i];
  columns = $($(row).find(".a-row")[0]).children('.a-column');
  if (columns.length === 2) {
    timeOfDay = $(columns[0]).text().trim();
    if (timeOfDay === '--') {
...
```

#### <a name="apidoc.element.shipit.PrestigeClient.prototype.requestOptions"></a>[function <span class="apidocSignatureSpan">shipit.PrestigeClient.prototype.</span>requestOptions (_arg)](#apidoc.element.shipit.PrestigeClient.prototype.requestOptions)
- description and source-code
```javascript
requestOptions = function (_arg) {
  var trackingNumber;
  trackingNumber = _arg.trackingNumber;
  return {
    method: 'GET',
    uri: "http://www.prestigedelivery.com/TrackingHandler.ashx?trackingNumbers=" + trackingNumber
  };
}
```
- example usage
```shell
...
      return cb(null, presentedResponse);
    };
  })(this));
};

ShipperClient.prototype.requestData = function(requestData, cb) {
  var opts, _ref;
  opts = this.requestOptions(requestData);
  opts.timeout = (requestData != null ? requestData.timeout : void 0) || ((_ref = this.options) != null ? _ref.timeout : void 0);
  return request(opts, (function(_this) {
    return function(err, response, body) {
      if ((body == null) || (err != null)) {
        return cb(err);
      }
      if (response.statusCode !== 200) {
...
```

#### <a name="apidoc.element.shipit.PrestigeClient.prototype.validateResponse"></a>[function <span class="apidocSignatureSpan">shipit.PrestigeClient.prototype.</span>validateResponse (response, cb)](#apidoc.element.shipit.PrestigeClient.prototype.validateResponse)
- description and source-code
```javascript
validateResponse = function (response, cb) {
  response = JSON.parse(response);
  if (!(response != null ? response.length : void 0)) {
    return cb({
      error: 'no tracking info found'
    });
  }
  response = response[0];
  if (response['TrackingEventHistory'] == null) {
    return cb({
      error: 'missing events'
    });
  }
  return cb(null, response);
}
```
- example usage
```shell
...
  if (postalCode != null ? postalCode.length : void 0) {
    address = address != null ? "" + address + " " + postalCode : postalCode;
  }
  return address;
};

ShipperClient.prototype.presentResponse = function(response, requestData, cb) {
  return this.validateResponse(response, (function(_this) {
    return function(err, shipment) {
      var activities, adjustedEta, eta, presentedResponse, status, _ref, _ref1;
      if ((err != null) || (shipment == null)) {
        return cb(err);
      }
      _ref = _this.getActivitiesAndStatus(shipment), activities = _ref.activities, status = _ref.status;
      eta = _this.getEta(shipment);
...
```



# <a name="apidoc.module.shipit.UpsClient"></a>[module shipit.UpsClient](#apidoc.module.shipit.UpsClient)

#### <a name="apidoc.element.shipit.UpsClient.UpsClient"></a>[function <span class="apidocSignatureSpan">shipit.</span>UpsClient (_arg, options)](#apidoc.element.shipit.UpsClient.UpsClient)
- description and source-code
```javascript
function UpsClient(_arg, options) {
  this.licenseNumber = _arg.licenseNumber, this.userId = _arg.userId, this.password = _arg.password;
  this.options = options;
  UpsClient.__super__.constructor.apply(this, arguments);
  this.parser = new Parser();
  this.builder = new Builder({
    renderOpts: {
      pretty: false
    }
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.shipit.UpsClient.prototype"></a>[module shipit.UpsClient.prototype](#apidoc.module.shipit.UpsClient.prototype)

#### <a name="apidoc.element.shipit.UpsClient.prototype.constructor"></a>[function <span class="apidocSignatureSpan">shipit.UpsClient.prototype.</span>constructor (_arg, options)](#apidoc.element.shipit.UpsClient.prototype.constructor)
- description and source-code
```javascript
function UpsClient(_arg, options) {
  this.licenseNumber = _arg.licenseNumber, this.userId = _arg.userId, this.password = _arg.password;
  this.options = options;
  UpsClient.__super__.constructor.apply(this, arguments);
  this.parser = new Parser();
  this.builder = new Builder({
    renderOpts: {
      pretty: false
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.shipit.UpsClient.prototype.generateRequest"></a>[function <span class="apidocSignatureSpan">shipit.UpsClient.prototype.</span>generateRequest (trk, reference)](#apidoc.element.shipit.UpsClient.prototype.generateRequest)
- description and source-code
```javascript
generateRequest = function (trk, reference) {
  var accessRequest, trackRequest;
  if (reference == null) {
    reference = 'n/a';
  }
  accessRequest = this.builder.buildObject({
    'AccessRequest': {
      'AccessLicenseNumber': this.licenseNumber,
      'UserId': this.userId,
      'Password': this.password
    }
  });
  trackRequest = this.builder.buildObject({
    'TrackRequest': {
      'Request': {
        'TransactionReference': {
          'CustomerContext': reference
        },
        'RequestAction': 'track',
        'RequestOption': 3
      },
      'TrackingNumber': trk
    }
  });
  return "" + accessRequest + trackRequest;
}
```
- example usage
```shell
...

  DhlClient.prototype.requestOptions = function(_arg) {
    var trackingNumber;
    trackingNumber = _arg.trackingNumber;
    return {
      method: 'POST',
      uri: 'http://xmlpi-ea.dhl.com/XMLShippingServlet',
      body: this.generateRequest(trackingNumber)
    };
  };

  return DhlClient;

})(ShipperClient);
...
```

#### <a name="apidoc.element.shipit.UpsClient.prototype.getActivitiesAndStatus"></a>[function <span class="apidocSignatureSpan">shipit.UpsClient.prototype.</span>getActivitiesAndStatus (shipment)](#apidoc.element.shipit.UpsClient.prototype.getActivitiesAndStatus)
- description and source-code
```javascript
getActivitiesAndStatus = function (shipment) {
  var activities, activity, details, lastStatus, location, rawActivities, rawActivity, status, statusObj, timestamp, _i, _len, _ref10
, _ref11, _ref12, _ref13, _ref14, _ref15, _ref16, _ref17, _ref18, _ref19, _ref2, _ref20, _ref21, _ref3, _ref4, _ref5, _ref6, _ref7
, _ref8, _ref9;
  activities = [];
  status = null;
  rawActivities = shipment != null ? (_ref2 = shipment['Package']) != null ? (_ref3 = _ref2[0]) != null ? _ref3['Activity'] : void
 0 : void 0 : void 0;
  _ref4 = rawActivities || [];
  for (_i = 0, _len = _ref4.length; _i < _len; _i++) {
    rawActivity = _ref4[_i];
    location = this.presentAddress((_ref5 = rawActivity['ActivityLocation']) != null ? (_ref6 = _ref5[0]) != null ? (_ref7 = _ref6
['Address']) != null ? _ref7[0] : void 0 : void 0 : void 0);
    timestamp = this.presentTimestamp((_ref8 = rawActivity['Date']) != null ? _ref8[0] : void 0, (_ref9 = rawActivity['Time']) !=
null ? _ref9[0] : void 0);
    lastStatus = (_ref10 = rawActivity['Status']) != null ? _ref10[0] : void 0;
    details = lastStatus != null ? (_ref11 = lastStatus['StatusType']) != null ? (_ref12 = _ref11[0]) != null ? (_ref13 = _ref12
['Description']) != null ? _ref13[0] : void 0 : void 0 : void 0 : void 0;
    if ((details != null) && (timestamp != null)) {
      details = upperCaseFirst(lowerCase(details));
      activity = {
        timestamp: timestamp,
        location: location,
        details: details
      };
      if (statusObj = (_ref14 = rawActivity['Status']) != null ? _ref14[0] : void 0) {
        activity.statusType = (_ref15 = statusObj['StatusType']) != null ? (_ref16 = _ref15[0]) != null ? (_ref17 = _ref16['Code
']) != null ? _ref17[0] : void 0 : void 0 : void 0;
        activity.statusCode = (_ref18 = statusObj['StatusCode']) != null ? (_ref19 = _ref18[0]) != null ? (_ref20 = _ref19['Code
']) != null ? _ref20[0] : void 0 : void 0 : void 0;
      }
      activities.push(activity);
    }
    if (!status) {
      status = this.presentStatus((_ref21 = rawActivity['Status']) != null ? _ref21[0] : void 0);
    }
  }
  return {
    activities: activities,
    status: status
  };
}
```
- example usage
```shell
...
    ShipperClient.prototype.presentResponse = function(response, requestData, cb) {
return this.validateResponse(response, (function(_this) {
  return function(err, shipment) {
    var activities, adjustedEta, eta, presentedResponse, status, _ref, _ref1;
    if ((err != null) || (shipment == null)) {
      return cb(err);
    }
    _ref = _this.getActivitiesAndStatus(shipment), activities = _ref.activities, status = _ref.status;
    eta = _this.getEta(shipment);
    if (eta != null) {
      adjustedEta = moment(eta).utc().format().replace(/T00:00:00/, 'T23:59:59');
    }
    if (adjustedEta != null) {
      adjustedEta = moment(adjustedEta).toDate();
    }
...
```

#### <a name="apidoc.element.shipit.UpsClient.prototype.getDestination"></a>[function <span class="apidocSignatureSpan">shipit.UpsClient.prototype.</span>getDestination (shipment)](#apidoc.element.shipit.UpsClient.prototype.getDestination)
- description and source-code
```javascript
getDestination = function (shipment) {
  var _ref2, _ref3, _ref4;
  return this.presentAddress((_ref2 = shipment['ShipTo']) != null ? (_ref3 = _ref2[0]) != null ? (_ref4 = _ref3['Address']) != null
 ? _ref4[0] : void 0 : void 0 : void 0);
}
```
- example usage
```shell
...
if (adjustedEta != null) {
  adjustedEta = moment(adjustedEta).toDate();
}
presentedResponse = {
  eta: adjustedEta,
  service: _this.getService(shipment),
  weight: _this.getWeight(shipment),
  destination: _this.getDestination(shipment),
  activities: activities,
  status: status
};
if ((requestData != null ? requestData.raw : void 0) != null) {
  if (requestData.raw) {
    presentedResponse.raw = response;
  }
...
```

#### <a name="apidoc.element.shipit.UpsClient.prototype.getEta"></a>[function <span class="apidocSignatureSpan">shipit.UpsClient.prototype.</span>getEta (shipment)](#apidoc.element.shipit.UpsClient.prototype.getEta)
- description and source-code
```javascript
getEta = function (shipment) {
  var _ref2, _ref3, _ref4, _ref5;
  return this.presentTimestamp(((_ref2 = shipment['Package']) != null ? (_ref3 = _ref2[0]) != null ? (_ref4 = _ref3['RescheduledDeliveryDate
']) != null ? _ref4[0] : void 0 : void 0 : void 0) || ((_ref5 = shipment['ScheduledDeliveryDate']) != null ? _ref5[0] : void 0));
}
```
- example usage
```shell
...
      return this.validateResponse(response, (function(_this) {
return function(err, shipment) {
  var activities, adjustedEta, eta, presentedResponse, status, _ref, _ref1;
  if ((err != null) || (shipment == null)) {
    return cb(err);
  }
  _ref = _this.getActivitiesAndStatus(shipment), activities = _ref.activities, status = _ref.status;
  eta = _this.getEta(shipment);
  if (eta != null) {
    adjustedEta = moment(eta).utc().format().replace(/T00:00:00/, 'T23:59:59');
  }
  if (adjustedEta != null) {
    adjustedEta = moment(adjustedEta).toDate();
  }
  presentedResponse = {
...
```

#### <a name="apidoc.element.shipit.UpsClient.prototype.getService"></a>[function <span class="apidocSignatureSpan">shipit.UpsClient.prototype.</span>getService (shipment)](#apidoc.element.shipit.UpsClient.prototype.getService)
- description and source-code
```javascript
getService = function (shipment) {
  var service, _ref2, _ref3, _ref4;
  if (service = (_ref2 = shipment['Service']) != null ? (_ref3 = _ref2[0]) != null ? (_ref4 = _ref3['Description']) != null ? _ref4
[0] : void 0 : void 0 : void 0) {
    return titleCase(service);
  }
}
```
- example usage
```shell
...
  adjustedEta = moment(eta).utc().format().replace(/T00:00:00/, 'T23:59:59');
}
if (adjustedEta != null) {
  adjustedEta = moment(adjustedEta).toDate();
}
presentedResponse = {
  eta: adjustedEta,
  service: _this.getService(shipment),
  weight: _this.getWeight(shipment),
  destination: _this.getDestination(shipment),
  activities: activities,
  status: status
};
if ((requestData != null ? requestData.raw : void 0) != null) {
  if (requestData.raw) {
...
```

#### <a name="apidoc.element.shipit.UpsClient.prototype.getWeight"></a>[function <span class="apidocSignatureSpan">shipit.UpsClient.prototype.</span>getWeight (shipment)](#apidoc.element.shipit.UpsClient.prototype.getWeight)
- description and source-code
```javascript
getWeight = function (shipment) {
  var units, weight, weightData, _ref2, _ref3, _ref4, _ref5, _ref6, _ref7, _ref8;
  weight = null;
  if (weightData = (_ref2 = shipment['Package']) != null ? (_ref3 = _ref2[0]) != null ? (_ref4 = _ref3['PackageWeight']) != null
 ? _ref4[0] : void 0 : void 0 : void 0) {
    weight = (_ref5 = weightData['Weight']) != null ? _ref5[0] : void 0;
    if ((weight != null) && (units = (_ref6 = weightData['UnitOfMeasurement']) != null ? (_ref7 = _ref6[0]) != null ? (_ref8 = _ref7
['Code']) != null ? _ref8[0] : void 0 : void 0 : void 0)) {
      weight = "" + weight + " " + units;
    }
  }
  return weight;
}
```
- example usage
```shell
...
}
if (adjustedEta != null) {
  adjustedEta = moment(adjustedEta).toDate();
}
presentedResponse = {
  eta: adjustedEta,
  service: _this.getService(shipment),
  weight: _this.getWeight(shipment),
  destination: _this.getDestination(shipment),
  activities: activities,
  status: status
};
if ((requestData != null ? requestData.raw : void 0) != null) {
  if (requestData.raw) {
    presentedResponse.raw = response;
...
```

#### <a name="apidoc.element.shipit.UpsClient.prototype.presentAddress"></a>[function <span class="apidocSignatureSpan">shipit.UpsClient.prototype.</span>presentAddress (rawAddress)](#apidoc.element.shipit.UpsClient.prototype.presentAddress)
- description and source-code
```javascript
presentAddress = function (rawAddress) {
  var city, countryCode, postalCode, stateCode, _ref2, _ref3, _ref4, _ref5;
  if (!rawAddress) {
    return;
  }
  city = (_ref2 = rawAddress['City']) != null ? _ref2[0] : void 0;
  stateCode = (_ref3 = rawAddress['StateProvinceCode']) != null ? _ref3[0] : void 0;
  countryCode = (_ref4 = rawAddress['CountryCode']) != null ? _ref4[0] : void 0;
  postalCode = (_ref5 = rawAddress['PostalCode']) != null ? _ref5[0] : void 0;
  return this.presentLocation({
    city: city,
    stateCode: stateCode,
    countryCode: countryCode,
    postalCode: postalCode
  });
}
```
- example usage
```shell
...
var activities, activity, datetime, details, event_time, location, rawActivities, rawActivity, raw_timestamp, status, timestamp,
_i, _len, _ref, _ref1, _ref2, _ref3, _ref4;
activities = [];
status = null;
rawActivities = (_ref = shipment['TrackingEventHistory']) != null ? (_ref1 = _ref[0]) != null ? _ref1['TrackingEventDetail'] : void
 0 : void 0;
_ref2 = rawActivities || [];
for (_i = 0, _len = _ref2.length; _i < _len; _i++) {
  rawActivity = _ref2[_i];
  location = this.presentAddress(rawActivity != null ? (_ref3 = rawActivity['EventLocation']) != null ? _ref3[0] : void 0 : void
 0);
  raw_timestamp = rawActivity != null ? rawActivity['EventDateTime'][0] : void 0;
  if (raw_timestamp != null) {
    event_time = moment(raw_timestamp);
    timestamp = event_time.toDate();
    datetime = raw_timestamp.slice(0, 19);
  }
  details = rawActivity != null ? (_ref4 = rawActivity['EventCodeDesc']) != null ? _ref4[0] : void 0 : void 0;
...
```

#### <a name="apidoc.element.shipit.UpsClient.prototype.presentStatus"></a>[function <span class="apidocSignatureSpan">shipit.UpsClient.prototype.</span>presentStatus (status)](#apidoc.element.shipit.UpsClient.prototype.presentStatus)
- description and source-code
```javascript
presentStatus = function (status) {
  var statusCode, statusType, _ref2, _ref3, _ref4, _ref5, _ref6, _ref7;
  if (status == null) {
    return ShipperClient.STATUS_TYPES.UNKNOWN;
  }
  statusType = (_ref2 = status['StatusType']) != null ? (_ref3 = _ref2[0]) != null ? (_ref4 = _ref3['Code']) != null ? _ref4[0] :
void 0 : void 0 : void 0;
  statusCode = (_ref5 = status['StatusCode']) != null ? (_ref6 = _ref5[0]) != null ? (_ref7 = _ref6['Code']) != null ? _ref7[0] :
void 0 : void 0 : void 0;
  if (STATUS_MAP[statusType] != null) {
    return STATUS_MAP[statusType];
  }
  switch (statusType) {
    case 'I':
      switch (statusCode) {
        case 'OF':
          return ShipperClient.STATUS_TYPES.OUT_FOR_DELIVERY;
        default:
          return ShipperClient.STATUS_TYPES.EN_ROUTE;
      }
      break;
    case 'X':
      switch (statusCode) {
        case 'U2':
          return ShipperClient.STATUS_TYPES.EN_ROUTE;
        default:
          return ShipperClient.STATUS_TYPES.DELAYED;
      }
      break;
    default:
      return ShipperClient.STATUS_TYPES.UNKNOWN;
  }
}
```
- example usage
```shell
...
if (data == null) {
  return {
    activities: activities,
    status: status
  };
}
$ = data.$, rightNow = data.rightNow;
status = this.presentStatus($(".latest-event-status").text());
rows = $("div[data-a-expander-name=event-history-list] .a-box");
for (_i = 0, _len = rows.length; _i < _len; _i++) {
  row = rows[_i];
  columns = $($(row).find(".a-row")[0]).children('.a-column');
  if (columns.length === 2) {
    timeOfDay = $(columns[0]).text().trim();
    if (timeOfDay === '--') {
...
```

#### <a name="apidoc.element.shipit.UpsClient.prototype.presentTimestamp"></a>[function <span class="apidocSignatureSpan">shipit.UpsClient.prototype.</span>presentTimestamp (dateString, timeString)](#apidoc.element.shipit.UpsClient.prototype.presentTimestamp)
- description and source-code
```javascript
presentTimestamp = function (dateString, timeString) {
  var formatSpec;
  if (dateString == null) {
    return;
  }
  if (timeString == null) {
    timeString = '00:00:00';
  }
  formatSpec = 'YYYYMMDD HHmmss ZZ';
  return moment("" + dateString + " " + timeString + " +0000", formatSpec).toDate();
}
```
- example usage
```shell
...
}
rawActivities.reverse();
_ref1 = rawActivities || [];
for (_i = 0, _len = _ref1.length; _i < _len; _i++) {
  rawActivity = _ref1[_i];
  rawLocation = (_ref2 = rawActivity['ServiceArea']) != null ? (_ref3 = _ref2[0]) != null ? (_ref4 = _ref3['Description']) != null
 ? _ref4[0] : void 0 : void 0 : void 0;
  location = this.presentAddress(rawLocation);
  timestamp = this.presentTimestamp((_ref5 = rawActivity['Date']) != null ? _ref5[0] : void 0, (_ref6 = rawActivity['Time']) !=
null ? _ref6[0] : void 0);
  details = this.presentDetails(rawLocation, (_ref7 = rawActivity['ServiceEvent']) != null ? (_ref8 = _ref7[0]) != null ? (_ref9
 = _ref8['Description']) != null ? _ref9[0] : void 0 : void 0 : void 0);
  if ((details != null) && (timestamp != null)) {
    details = details.slice(-1) === '.' ? details.slice(0, -1) : details;
    activity = {
      timestamp: timestamp,
      location: location,
      details: details
...
```

#### <a name="apidoc.element.shipit.UpsClient.prototype.requestOptions"></a>[function <span class="apidocSignatureSpan">shipit.UpsClient.prototype.</span>requestOptions (_arg)](#apidoc.element.shipit.UpsClient.prototype.requestOptions)
- description and source-code
```javascript
requestOptions = function (_arg) {
  var hostname, reference, test, trackingNumber;
  trackingNumber = _arg.trackingNumber, reference = _arg.reference, test = _arg.test;
  hostname = test ? 'wwwcie.ups.com' : 'www.ups.com';
  return {
    method: 'POST',
    uri: "https://" + hostname + "/ups.app/xml/Track",
    body: this.generateRequest(trackingNumber, reference)
  };
}
```
- example usage
```shell
...
      return cb(null, presentedResponse);
    };
  })(this));
};

ShipperClient.prototype.requestData = function(requestData, cb) {
  var opts, _ref;
  opts = this.requestOptions(requestData);
  opts.timeout = (requestData != null ? requestData.timeout : void 0) || ((_ref = this.options) != null ? _ref.timeout : void 0);
  return request(opts, (function(_this) {
    return function(err, response, body) {
      if ((body == null) || (err != null)) {
        return cb(err);
      }
      if (response.statusCode !== 200) {
...
```

#### <a name="apidoc.element.shipit.UpsClient.prototype.validateResponse"></a>[function <span class="apidocSignatureSpan">shipit.UpsClient.prototype.</span>validateResponse (response, cb)](#apidoc.element.shipit.UpsClient.prototype.validateResponse)
- description and source-code
```javascript
validateResponse = function (response, cb) {
  var handleResponse;
  handleResponse = function(xmlErr, trackResult) {
    var error, errorMsg, responseStatus, shipment, _ref10, _ref11, _ref12, _ref2, _ref3, _ref4, _ref5, _ref6, _ref7, _ref8, _ref9
;
    if ((xmlErr != null) || (trackResult == null)) {
      return cb(xmlErr);
    }
    responseStatus = (_ref2 = trackResult['TrackResponse']) != null ? (_ref3 = _ref2['Response']) != null ? (_ref4 = _ref3[0]) !=
null ? (_ref5 = _ref4['ResponseStatusDescription']) != null ? _ref5[0] : void 0 : void 0 : void 0 : void 0;
    if (responseStatus !== 'Success') {
      error = (_ref6 = trackResult['TrackResponse']) != null ? (_ref7 = _ref6['Response']) != null ? (_ref8 = _ref7[0]) != null ? (
_ref9 = _ref8['Error']) != null ? (_ref10 = _ref9[0]) != null ? (_ref11 = _ref10['ErrorDescription']) != null ? _ref11[0] : void
 0 : void 0 : void 0 : void 0 : void 0 : void 0;
      errorMsg = error || "unknown error";
      shipment = null;
    } else {
      shipment = (_ref12 = trackResult['TrackResponse']['Shipment']) != null ? _ref12[0] : void 0;
      if (shipment == null) {
        errorMsg = "missing shipment data";
      }
    }
    if (errorMsg != null) {
      return cb(errorMsg);
    }
    return cb(null, shipment);
  };
  this.parser.reset();
  return this.parser.parseString(response, handleResponse);
}
```
- example usage
```shell
...
  if (postalCode != null ? postalCode.length : void 0) {
    address = address != null ? "" + address + " " + postalCode : postalCode;
  }
  return address;
};

ShipperClient.prototype.presentResponse = function(response, requestData, cb) {
  return this.validateResponse(response, (function(_this) {
    return function(err, shipment) {
      var activities, adjustedEta, eta, presentedResponse, status, _ref, _ref1;
      if ((err != null) || (shipment == null)) {
        return cb(err);
      }
      _ref = _this.getActivitiesAndStatus(shipment), activities = _ref.activities, status = _ref.status;
      eta = _this.getEta(shipment);
...
```



# <a name="apidoc.module.shipit.UpsMiClient"></a>[module shipit.UpsMiClient](#apidoc.module.shipit.UpsMiClient)

#### <a name="apidoc.element.shipit.UpsMiClient.UpsMiClient"></a>[function <span class="apidocSignatureSpan">shipit.</span>UpsMiClient (options)](#apidoc.element.shipit.UpsMiClient.UpsMiClient)
- description and source-code
```javascript
function UpsMiClient(options) {
  this.options = options;
  STATUS_MAP[ShipperClient.STATUS_TYPES.DELIVERED] = ['delivered'];
  STATUS_MAP[ShipperClient.STATUS_TYPES.EN_ROUTE] = ['transferred', 'received', 'processed', 'sorted', 'post office entry'];
  STATUS_MAP[ShipperClient.STATUS_TYPES.OUT_FOR_DELIVERY] = ['out for post office delivery'];
  STATUS_MAP[ShipperClient.STATUS_TYPES.SHIPPING] = ['shipment information received'];
  UpsMiClient.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.shipit.UpsMiClient.prototype"></a>[module shipit.UpsMiClient.prototype](#apidoc.module.shipit.UpsMiClient.prototype)

#### <a name="apidoc.element.shipit.UpsMiClient.prototype.constructor"></a>[function <span class="apidocSignatureSpan">shipit.UpsMiClient.prototype.</span>constructor (options)](#apidoc.element.shipit.UpsMiClient.prototype.constructor)
- description and source-code
```javascript
function UpsMiClient(options) {
  this.options = options;
  STATUS_MAP[ShipperClient.STATUS_TYPES.DELIVERED] = ['delivered'];
  STATUS_MAP[ShipperClient.STATUS_TYPES.EN_ROUTE] = ['transferred', 'received', 'processed', 'sorted', 'post office entry'];
  STATUS_MAP[ShipperClient.STATUS_TYPES.OUT_FOR_DELIVERY] = ['out for post office delivery'];
  STATUS_MAP[ShipperClient.STATUS_TYPES.SHIPPING] = ['shipment information received'];
  UpsMiClient.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.shipit.UpsMiClient.prototype.extractActivities"></a>[function <span class="apidocSignatureSpan">shipit.UpsMiClient.prototype.</span>extractActivities ($, table)](#apidoc.element.shipit.UpsMiClient.prototype.extractActivities)
- description and source-code
```javascript
extractActivities = function ($, table) {
  var activities;
  activities = [];
  $(table).children('tr').each((function(_this) {
    return function(rindex, row) {
      var details, location, timestamp;
      if (rindex === 0) {
        return;
      }
      details = location = timestamp = null;
      $(row).children('td').each(function(cindex, col) {
        var value, _ref1, _ref2;
        value = (_ref1 = $(col)) != null ? (_ref2 = _ref1.text()) != null ? _ref2.trim() : void 0 : void 0;
        switch (cindex) {
          case 0:
            return timestamp = _this.extractTimestamp(value);
          case 1:
            return details = value;
          case 2:
            return location = _this.presentLocationString(value);
        }
      });
      if ((details != null) && (timestamp != null)) {
        return activities.push({
          details: details,
          location: location,
          timestamp: timestamp
        });
      }
    };
  })(this));
  return activities;
}
```
- example usage
```shell
...
  return activities;
};

UpsMiClient.prototype.getActivitiesAndStatus = function(data) {
  var $, activities, activity, miDetails, set1, set2, status, uspsDetails, _i, _len, _ref1;
  status = null;
  $ = data.$, uspsDetails = data.uspsDetails, miDetails = data.miDetails;
  set1 = this.extractActivities($, uspsDetails);
  set2 = this.extractActivities($, miDetails);
  activities = set1.concat(set2);
  _ref1 = activities || [];
  for (_i = 0, _len = _ref1.length; _i < _len; _i++) {
    activity = _ref1[_i];
    if (status != null) {
      break;
...
```

#### <a name="apidoc.element.shipit.UpsMiClient.prototype.extractSummaryField"></a>[function <span class="apidocSignatureSpan">shipit.UpsMiClient.prototype.</span>extractSummaryField (data, name)](#apidoc.element.shipit.UpsMiClient.prototype.extractSummaryField)
- description and source-code
```javascript
extractSummaryField = function (data, name) {
  var $, summary, value;
  value = null;
  $ = data.$, summary = data.summary;
  if (summary == null) {
    return;
  }
  $(summary).children('tr').each(function(rindex, row) {
    $(row).children('td').each(function(cindex, col) {
      var regex, _ref1, _ref2;
      regex = new RegExp(name);
      if (regex.test($(col).text())) {
        value = (_ref1 = $(col).next()) != null ? (_ref2 = _ref1.text()) != null ? _ref2.trim() : void 0 : void 0;
      }
      if (value != null) {
        return false;
      }
    });
    if (value != null) {
      return false;
    }
  });
  return value;
}
```
- example usage
```shell
...
  if (!(eta != null ? eta.length : void 0)) {
    return;
  }
  return moment("" + eta + " 23:59:59 +00:00").toDate();
};

DhlGmClient.prototype.getService = function(data) {
  return this.extractSummaryField(data, 'Service');
};

DhlGmClient.prototype.getWeight = function(data) {
  return this.extractSummaryField(data, 'Weight');
};

DhlGmClient.prototype.presentStatus = function(details) {
...
```

#### <a name="apidoc.element.shipit.UpsMiClient.prototype.extractTimestamp"></a>[function <span class="apidocSignatureSpan">shipit.UpsMiClient.prototype.</span>extractTimestamp (tsString)](#apidoc.element.shipit.UpsMiClient.prototype.extractTimestamp)
- description and source-code
```javascript
extractTimestamp = function (tsString) {
  if (tsString.match(':')) {
    return moment("" + tsString + " +0000").toDate();
  } else {
    return moment("" + tsString + " 00:00 +0000").toDate();
  }
}
```
- example usage
```shell
...
}
details = location = timestamp = null;
$(row).children('td').each(function(cindex, col) {
  var value, _ref1, _ref2;
  value = (_ref1 = $(col)) != null ? (_ref2 = _ref1.text()) != null ? _ref2.trim() : void 0 : void 0;
  switch (cindex) {
    case 0:
      return timestamp = _this.extractTimestamp(value);
    case 1:
      return details = value;
    case 2:
      return location = _this.presentLocationString(value);
  }
});
if ((details != null) && (timestamp != null)) {
...
```

#### <a name="apidoc.element.shipit.UpsMiClient.prototype.getActivitiesAndStatus"></a>[function <span class="apidocSignatureSpan">shipit.UpsMiClient.prototype.</span>getActivitiesAndStatus (data)](#apidoc.element.shipit.UpsMiClient.prototype.getActivitiesAndStatus)
- description and source-code
```javascript
getActivitiesAndStatus = function (data) {
  var $, activities, activity, miDetails, set1, set2, status, uspsDetails, _i, _len, _ref1;
  status = null;
  $ = data.$, uspsDetails = data.uspsDetails, miDetails = data.miDetails;
  set1 = this.extractActivities($, uspsDetails);
  set2 = this.extractActivities($, miDetails);
  activities = set1.concat(set2);
  _ref1 = activities || [];
  for (_i = 0, _len = _ref1.length; _i < _len; _i++) {
    activity = _ref1[_i];
    if (status != null) {
      break;
    }
    status = this.presentStatus(activity != null ? activity.details : void 0);
  }
  return {
    activities: activities,
    status: status
  };
}
```
- example usage
```shell
...
    ShipperClient.prototype.presentResponse = function(response, requestData, cb) {
return this.validateResponse(response, (function(_this) {
  return function(err, shipment) {
    var activities, adjustedEta, eta, presentedResponse, status, _ref, _ref1;
    if ((err != null) || (shipment == null)) {
      return cb(err);
    }
    _ref = _this.getActivitiesAndStatus(shipment), activities = _ref.activities, status = _ref.status;
    eta = _this.getEta(shipment);
    if (eta != null) {
      adjustedEta = moment(eta).utc().format().replace(/T00:00:00/, 'T23:59:59');
    }
    if (adjustedEta != null) {
      adjustedEta = moment(adjustedEta).toDate();
    }
...
```

#### <a name="apidoc.element.shipit.UpsMiClient.prototype.getDestination"></a>[function <span class="apidocSignatureSpan">shipit.UpsMiClient.prototype.</span>getDestination (data)](#apidoc.element.shipit.UpsMiClient.prototype.getDestination)
- description and source-code
```javascript
getDestination = function (data) {
  var destination;
  destination = this.extractSummaryField(data, 'Zip Code');
  if (destination != null ? destination.length : void 0) {
    return destination;
  }
}
```
- example usage
```shell
...
if (adjustedEta != null) {
  adjustedEta = moment(adjustedEta).toDate();
}
presentedResponse = {
  eta: adjustedEta,
  service: _this.getService(shipment),
  weight: _this.getWeight(shipment),
  destination: _this.getDestination(shipment),
  activities: activities,
  status: status
};
if ((requestData != null ? requestData.raw : void 0) != null) {
  if (requestData.raw) {
    presentedResponse.raw = response;
  }
...
```

#### <a name="apidoc.element.shipit.UpsMiClient.prototype.getEta"></a>[function <span class="apidocSignatureSpan">shipit.UpsMiClient.prototype.</span>getEta (data)](#apidoc.element.shipit.UpsMiClient.prototype.getEta)
- description and source-code
```javascript
getEta = function (data) {
  var eta, formattedEta;
  eta = this.extractSummaryField(data, 'Projected Delivery Date');
  if (eta != null) {
    formattedEta = moment("" + eta + " 00:00 +0000");
  }
  if (formattedEta != null ? formattedEta.isValid() : void 0) {
    return formattedEta.toDate();
  } else {
    return void 0;
  }
}
```
- example usage
```shell
...
      return this.validateResponse(response, (function(_this) {
return function(err, shipment) {
  var activities, adjustedEta, eta, presentedResponse, status, _ref, _ref1;
  if ((err != null) || (shipment == null)) {
    return cb(err);
  }
  _ref = _this.getActivitiesAndStatus(shipment), activities = _ref.activities, status = _ref.status;
  eta = _this.getEta(shipment);
  if (eta != null) {
    adjustedEta = moment(eta).utc().format().replace(/T00:00:00/, 'T23:59:59');
  }
  if (adjustedEta != null) {
    adjustedEta = moment(adjustedEta).toDate();
  }
  presentedResponse = {
...
```

#### <a name="apidoc.element.shipit.UpsMiClient.prototype.getService"></a>[function <span class="apidocSignatureSpan">shipit.UpsMiClient.prototype.</span>getService ()](#apidoc.element.shipit.UpsMiClient.prototype.getService)
- description and source-code
```javascript
getService = function () {}
```
- example usage
```shell
...
  adjustedEta = moment(eta).utc().format().replace(/T00:00:00/, 'T23:59:59');
}
if (adjustedEta != null) {
  adjustedEta = moment(adjustedEta).toDate();
}
presentedResponse = {
  eta: adjustedEta,
  service: _this.getService(shipment),
  weight: _this.getWeight(shipment),
  destination: _this.getDestination(shipment),
  activities: activities,
  status: status
};
if ((requestData != null ? requestData.raw : void 0) != null) {
  if (requestData.raw) {
...
```

#### <a name="apidoc.element.shipit.UpsMiClient.prototype.getWeight"></a>[function <span class="apidocSignatureSpan">shipit.UpsMiClient.prototype.</span>getWeight (data)](#apidoc.element.shipit.UpsMiClient.prototype.getWeight)
- description and source-code
```javascript
getWeight = function (data) {
  var weight;
  weight = this.extractSummaryField(data, 'Weight');
  if (weight != null ? weight.length : void 0) {
    return "" + weight + " lbs.";
  }
}
```
- example usage
```shell
...
}
if (adjustedEta != null) {
  adjustedEta = moment(adjustedEta).toDate();
}
presentedResponse = {
  eta: adjustedEta,
  service: _this.getService(shipment),
  weight: _this.getWeight(shipment),
  destination: _this.getDestination(shipment),
  activities: activities,
  status: status
};
if ((requestData != null ? requestData.raw : void 0) != null) {
  if (requestData.raw) {
    presentedResponse.raw = response;
...
```

#### <a name="apidoc.element.shipit.UpsMiClient.prototype.presentStatus"></a>[function <span class="apidocSignatureSpan">shipit.UpsMiClient.prototype.</span>presentStatus (details)](#apidoc.element.shipit.UpsMiClient.prototype.presentStatus)
- description and source-code
```javascript
presentStatus = function (details) {
  var matchStrings, regex, status, statusCode, text, _i, _len;
  status = null;
  for (statusCode in STATUS_MAP) {
    matchStrings = STATUS_MAP[statusCode];
    for (_i = 0, _len = matchStrings.length; _i < _len; _i++) {
      text = matchStrings[_i];
      regex = new RegExp(text, 'i');
      if (regex.test(lowerCase(details))) {
        status = statusCode;
        break;
      }
    }
    if (status != null) {
      break;
    }
  }
  if (status != null) {
    return parseInt(status, 10);
  }
}
```
- example usage
```shell
...
if (data == null) {
  return {
    activities: activities,
    status: status
  };
}
$ = data.$, rightNow = data.rightNow;
status = this.presentStatus($(".latest-event-status").text());
rows = $("div[data-a-expander-name=event-history-list] .a-box");
for (_i = 0, _len = rows.length; _i < _len; _i++) {
  row = rows[_i];
  columns = $($(row).find(".a-row")[0]).children('.a-column');
  if (columns.length === 2) {
    timeOfDay = $(columns[0]).text().trim();
    if (timeOfDay === '--') {
...
```

#### <a name="apidoc.element.shipit.UpsMiClient.prototype.requestOptions"></a>[function <span class="apidocSignatureSpan">shipit.UpsMiClient.prototype.</span>requestOptions (_arg)](#apidoc.element.shipit.UpsMiClient.prototype.requestOptions)
- description and source-code
```javascript
requestOptions = function (_arg) {
  var trackingNumber;
  trackingNumber = _arg.trackingNumber;
  return {
    method: 'GET',
    uri: "http://www.ups-mi.net/packageID/PackageID.aspx?PID=" + trackingNumber
  };
}
```
- example usage
```shell
...
      return cb(null, presentedResponse);
    };
  })(this));
};

ShipperClient.prototype.requestData = function(requestData, cb) {
  var opts, _ref;
  opts = this.requestOptions(requestData);
  opts.timeout = (requestData != null ? requestData.timeout : void 0) || ((_ref = this.options) != null ? _ref.timeout : void 0);
  return request(opts, (function(_this) {
    return function(err, response, body) {
      if ((body == null) || (err != null)) {
        return cb(err);
      }
      if (response.statusCode !== 200) {
...
```

#### <a name="apidoc.element.shipit.UpsMiClient.prototype.validateResponse"></a>[function <span class="apidocSignatureSpan">shipit.UpsMiClient.prototype.</span>validateResponse (response, cb)](#apidoc.element.shipit.UpsMiClient.prototype.validateResponse)
- description and source-code
```javascript
validateResponse = function (response, cb) {
  var $, miDetails, summary, uspsDetails, _ref1;
  $ = load(response, {
    normalizeWhitespace: true
  });
  summary = (_ref1 = $('#Table6').find('table')) != null ? _ref1[0] : void 0;
  uspsDetails = $('#ctl00_mainContent_ctl00_pnlUSPS > table');
  miDetails = $('#ctl00_mainContent_ctl00_pnlMI > table');
  return cb(null, {
    $: $,
    summary: summary,
    uspsDetails: uspsDetails,
    miDetails: miDetails
  });
}
```
- example usage
```shell
...
  if (postalCode != null ? postalCode.length : void 0) {
    address = address != null ? "" + address + " " + postalCode : postalCode;
  }
  return address;
};

ShipperClient.prototype.presentResponse = function(response, requestData, cb) {
  return this.validateResponse(response, (function(_this) {
    return function(err, shipment) {
      var activities, adjustedEta, eta, presentedResponse, status, _ref, _ref1;
      if ((err != null) || (shipment == null)) {
        return cb(err);
      }
      _ref = _this.getActivitiesAndStatus(shipment), activities = _ref.activities, status = _ref.status;
      eta = _this.getEta(shipment);
...
```



# <a name="apidoc.module.shipit.UspsClient"></a>[module shipit.UspsClient](#apidoc.module.shipit.UspsClient)

#### <a name="apidoc.element.shipit.UspsClient.UspsClient"></a>[function <span class="apidocSignatureSpan">shipit.</span>UspsClient (_arg, options)](#apidoc.element.shipit.UspsClient.UspsClient)
- description and source-code
```javascript
function UspsClient(_arg, options) {
  this.userId = _arg.userId;
  this.options = options;
  UspsClient.__super__.constructor.apply(this, arguments);
  this.parser = new Parser();
  this.builder = new Builder({
    renderOpts: {
      pretty: false
    }
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.shipit.UspsClient.prototype"></a>[module shipit.UspsClient.prototype](#apidoc.module.shipit.UspsClient.prototype)

#### <a name="apidoc.element.shipit.UspsClient.prototype.constructor"></a>[function <span class="apidocSignatureSpan">shipit.UspsClient.prototype.</span>constructor (_arg, options)](#apidoc.element.shipit.UspsClient.prototype.constructor)
- description and source-code
```javascript
function UspsClient(_arg, options) {
  this.userId = _arg.userId;
  this.options = options;
  UspsClient.__super__.constructor.apply(this, arguments);
  this.parser = new Parser();
  this.builder = new Builder({
    renderOpts: {
      pretty: false
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.shipit.UspsClient.prototype.findStatusFromMap"></a>[function <span class="apidocSignatureSpan">shipit.UspsClient.prototype.</span>findStatusFromMap (statusText)](#apidoc.element.shipit.UspsClient.prototype.findStatusFromMap)
- description and source-code
```javascript
findStatusFromMap = function (statusText) {
  var regex, status, statusCode, text;
  status = ShipperClient.STATUS_TYPES.UNKNOWN;
  for (text in STATUS_MAP) {
    statusCode = STATUS_MAP[text];
    regex = new RegExp(text, 'i');
    if (regex.test(statusText)) {
      status = statusCode;
      break;
    }
  }
  return status;
}
```
- example usage
```shell
...
      break;
    }
  }
  return status;
};

CanadaPostClient.prototype.getStatus = function(lastEvent) {
  return this.findStatusFromMap(lastEvent != null ? lastEvent.details : void 0);
};

CanadaPostClient.prototype.getActivitiesAndStatus = function(shipment) {
  var activities, activity, city, details, event, events, location, stateCode, status, timestamp, _i, _len, _ref, _ref1, _ref2,
_ref3, _ref4, _ref5, _ref6, _ref7;
  activities = [];
  status = null;
  events = (_ref = shipment['significant-events']) != null ? (_ref1 = _ref[0]) != null ? _ref1['occurrence'] : void 0 : void 0;
...
```

#### <a name="apidoc.element.shipit.UspsClient.prototype.generateRequest"></a>[function <span class="apidocSignatureSpan">shipit.UspsClient.prototype.</span>generateRequest (trk, clientIp)](#apidoc.element.shipit.UspsClient.prototype.generateRequest)
- description and source-code
```javascript
generateRequest = function (trk, clientIp) {
  if (clientIp == null) {
    clientIp = '127.0.0.1';
  }
  return this.builder.buildObject({
    'TrackFieldRequest': {
      '$': {
        'USERID': this.userId
      },
      'Revision': '1',
      'ClientIp': clientIp,
      'SourceId': 'shipit',
      'TrackID': {
        '$': {
          'ID': trk
        }
      }
    }
  });
}
```
- example usage
```shell
...

  DhlClient.prototype.requestOptions = function(_arg) {
    var trackingNumber;
    trackingNumber = _arg.trackingNumber;
    return {
      method: 'POST',
      uri: 'http://xmlpi-ea.dhl.com/XMLShippingServlet',
      body: this.generateRequest(trackingNumber)
    };
  };

  return DhlClient;

})(ShipperClient);
...
```

#### <a name="apidoc.element.shipit.UspsClient.prototype.getActivitiesAndStatus"></a>[function <span class="apidocSignatureSpan">shipit.UspsClient.prototype.</span>getActivitiesAndStatus (shipment)](#apidoc.element.shipit.UspsClient.prototype.getActivitiesAndStatus)
- description and source-code
```javascript
getActivitiesAndStatus = function (shipment) {
  var activities, activity, rawActivity, trackSummary, _i, _len, _ref2, _ref3;
  activities = [];
  trackSummary = this.presentActivity(shipment != null ? (_ref2 = shipment['TrackSummary']) != null ? _ref2[0] : void 0 : void 0
);
  if (trackSummary != null) {
    activities.push(trackSummary);
  }
  _ref3 = (shipment != null ? shipment['TrackDetail'] : void 0) || [];
  for (_i = 0, _len = _ref3.length; _i < _len; _i++) {
    rawActivity = _ref3[_i];
    activity = this.presentActivity(rawActivity);
    if (activity != null) {
      activities.push(activity);
    }
  }
  return {
    activities: activities,
    status: this.getStatus(shipment)
  };
}
```
- example usage
```shell
...
    ShipperClient.prototype.presentResponse = function(response, requestData, cb) {
return this.validateResponse(response, (function(_this) {
  return function(err, shipment) {
    var activities, adjustedEta, eta, presentedResponse, status, _ref, _ref1;
    if ((err != null) || (shipment == null)) {
      return cb(err);
    }
    _ref = _this.getActivitiesAndStatus(shipment), activities = _ref.activities, status = _ref.status;
    eta = _this.getEta(shipment);
    if (eta != null) {
      adjustedEta = moment(eta).utc().format().replace(/T00:00:00/, 'T23:59:59');
    }
    if (adjustedEta != null) {
      adjustedEta = moment(adjustedEta).toDate();
    }
...
```

#### <a name="apidoc.element.shipit.UspsClient.prototype.getDestination"></a>[function <span class="apidocSignatureSpan">shipit.UspsClient.prototype.</span>getDestination (shipment)](#apidoc.element.shipit.UspsClient.prototype.getDestination)
- description and source-code
```javascript
getDestination = function (shipment) {
  var city, postalCode, stateCode, _ref2, _ref3, _ref4;
  city = (_ref2 = shipment['DestinationCity']) != null ? _ref2[0] : void 0;
  stateCode = (_ref3 = shipment['DestinationState']) != null ? _ref3[0] : void 0;
  postalCode = (_ref4 = shipment['DestinationZip']) != null ? _ref4[0] : void 0;
  return this.presentLocation({
    city: city,
    stateCode: stateCode,
    postalCode: postalCode
  });
}
```
- example usage
```shell
...
if (adjustedEta != null) {
  adjustedEta = moment(adjustedEta).toDate();
}
presentedResponse = {
  eta: adjustedEta,
  service: _this.getService(shipment),
  weight: _this.getWeight(shipment),
  destination: _this.getDestination(shipment),
  activities: activities,
  status: status
};
if ((requestData != null ? requestData.raw : void 0) != null) {
  if (requestData.raw) {
    presentedResponse.raw = response;
  }
...
```

#### <a name="apidoc.element.shipit.UspsClient.prototype.getEta"></a>[function <span class="apidocSignatureSpan">shipit.UspsClient.prototype.</span>getEta (shipment)](#apidoc.element.shipit.UspsClient.prototype.getEta)
- description and source-code
```javascript
getEta = function (shipment) {
  var rawEta, _ref2, _ref3;
  rawEta = ((_ref2 = shipment['PredictedDeliveryDate']) != null ? _ref2[0] : void 0) || ((_ref3 = shipment['ExpectedDeliveryDate
']) != null ? _ref3[0] : void 0);
  if (rawEta != null) {
    return moment("" + rawEta + " 00:00:00Z").toDate();
  }
}
```
- example usage
```shell
...
      return this.validateResponse(response, (function(_this) {
return function(err, shipment) {
  var activities, adjustedEta, eta, presentedResponse, status, _ref, _ref1;
  if ((err != null) || (shipment == null)) {
    return cb(err);
  }
  _ref = _this.getActivitiesAndStatus(shipment), activities = _ref.activities, status = _ref.status;
  eta = _this.getEta(shipment);
  if (eta != null) {
    adjustedEta = moment(eta).utc().format().replace(/T00:00:00/, 'T23:59:59');
  }
  if (adjustedEta != null) {
    adjustedEta = moment(adjustedEta).toDate();
  }
  presentedResponse = {
...
```

#### <a name="apidoc.element.shipit.UspsClient.prototype.getService"></a>[function <span class="apidocSignatureSpan">shipit.UspsClient.prototype.</span>getService (shipment)](#apidoc.element.shipit.UspsClient.prototype.getService)
- description and source-code
```javascript
getService = function (shipment) {
  var service, _ref2;
  service = (_ref2 = shipment['Class']) != null ? _ref2[0] : void 0;
  if (service != null) {
    return service.replace(/\<SUP\>.*\<\/SUP\>/, '');
  }
}
```
- example usage
```shell
...
  adjustedEta = moment(eta).utc().format().replace(/T00:00:00/, 'T23:59:59');
}
if (adjustedEta != null) {
  adjustedEta = moment(adjustedEta).toDate();
}
presentedResponse = {
  eta: adjustedEta,
  service: _this.getService(shipment),
  weight: _this.getWeight(shipment),
  destination: _this.getDestination(shipment),
  activities: activities,
  status: status
};
if ((requestData != null ? requestData.raw : void 0) != null) {
  if (requestData.raw) {
...
```

#### <a name="apidoc.element.shipit.UspsClient.prototype.getStatus"></a>[function <span class="apidocSignatureSpan">shipit.UspsClient.prototype.</span>getStatus (shipment)](#apidoc.element.shipit.UspsClient.prototype.getStatus)
- description and source-code
```javascript
getStatus = function (shipment) {
  var statusCategory, _ref2, _ref3;
  statusCategory = shipment != null ? (_ref2 = shipment['StatusCategory']) != null ? _ref2[0] : void 0 : void 0;
  switch (statusCategory) {
    case 'Pre-Shipment':
      return ShipperClient.STATUS_TYPES.SHIPPING;
    case 'Delivered':
      return ShipperClient.STATUS_TYPES.DELIVERED;
    default:
      return this.findStatusFromMap(shipment != null ? (_ref3 = shipment['Status']) != null ? _ref3[0] : void 0 : void 0);
  }
}
```
- example usage
```shell
...
        details: details
      };
      activities.push(activity);
    }
  }
  return {
    activities: activities,
    status: this.getStatus(shipment)
  };
};

A1Client.prototype.getEta = function(shipment) {
  var activities, firstActivity, _ref, _ref1, _ref2, _ref3;
  activities = ((_ref = shipment['TrackingEventHistory']) != null ? (_ref1 = _ref[0]) != null ? _ref1['TrackingEventDetail'] : void
 0 : void 0) || [];
  firstActivity = activities[activities.length - 1];
...
```

#### <a name="apidoc.element.shipit.UspsClient.prototype.getWeight"></a>[function <span class="apidocSignatureSpan">shipit.UspsClient.prototype.</span>getWeight (shipment)](#apidoc.element.shipit.UspsClient.prototype.getWeight)
- description and source-code
```javascript
getWeight = function (shipment) {}
```
- example usage
```shell
...
}
if (adjustedEta != null) {
  adjustedEta = moment(adjustedEta).toDate();
}
presentedResponse = {
  eta: adjustedEta,
  service: _this.getService(shipment),
  weight: _this.getWeight(shipment),
  destination: _this.getDestination(shipment),
  activities: activities,
  status: status
};
if ((requestData != null ? requestData.raw : void 0) != null) {
  if (requestData.raw) {
    presentedResponse.raw = response;
...
```

#### <a name="apidoc.element.shipit.UspsClient.prototype.presentActivity"></a>[function <span class="apidocSignatureSpan">shipit.UspsClient.prototype.</span>presentActivity (rawActivity)](#apidoc.element.shipit.UspsClient.prototype.presentActivity)
- description and source-code
```javascript
presentActivity = function (rawActivity) {
  var activity, city, countryCode, details, location, postalCode, stateCode, timestamp, _ref10, _ref11, _ref12, _ref13, _ref14,
_ref2, _ref3, _ref4, _ref5, _ref6, _ref7, _ref8, _ref9;
  if (rawActivity == null) {
    return;
  }
  activity = null;
  city = (_ref2 = rawActivity['EventCity']) != null ? _ref2[0] : void 0;
  if ((_ref3 = rawActivity['EventState']) != null ? (_ref4 = _ref3[0]) != null ? _ref4.length : void 0 : void 0) {
    stateCode = (_ref5 = rawActivity['EventState']) != null ? _ref5[0] : void 0;
  }
  if ((_ref6 = rawActivity['EventZIPCode']) != null ? (_ref7 = _ref6[0]) != null ? _ref7.length : void 0 : void 0) {
    postalCode = (_ref8 = rawActivity['EventZIPCode']) != null ? _ref8[0] : void 0;
  }
  if ((_ref9 = rawActivity['EventCountry']) != null ? (_ref10 = _ref9[0]) != null ? _ref10.length : void 0 : void 0) {
    countryCode = (_ref11 = rawActivity['EventCountry']) != null ? _ref11[0] : void 0;
  }
  location = this.presentLocation({
    city: city,
    stateCode: stateCode,
    countryCode: countryCode,
    postalCode: postalCode
  });
  timestamp = this.presentTimestamp(rawActivity != null ? (_ref12 = rawActivity['EventDate']) != null ? _ref12[0] : void 0 : void
 0, rawActivity != null ? (_ref13 = rawActivity['EventTime']) != null ? _ref13[0] : void 0 : void 0);
  details = rawActivity != null ? (_ref14 = rawActivity['Event']) != null ? _ref14[0] : void 0 : void 0;
  if ((details != null) && (timestamp != null)) {
    activity = {
      timestamp: timestamp,
      location: location,
      details: details
    };
  }
  return activity;
}
```
- example usage
```shell
...
  }
  return activity;
};

UspsClient.prototype.getActivitiesAndStatus = function(shipment) {
  var activities, activity, rawActivity, trackSummary, _i, _len, _ref2, _ref3;
  activities = [];
  trackSummary = this.presentActivity(shipment != null ? (_ref2 = shipment['TrackSummary']) != null ? _ref2[0] : void 0 : void 0
);
  if (trackSummary != null) {
    activities.push(trackSummary);
  }
  _ref3 = (shipment != null ? shipment['TrackDetail'] : void 0) || [];
  for (_i = 0, _len = _ref3.length; _i < _len; _i++) {
    rawActivity = _ref3[_i];
    activity = this.presentActivity(rawActivity);
...
```

#### <a name="apidoc.element.shipit.UspsClient.prototype.presentStatus"></a>[function <span class="apidocSignatureSpan">shipit.UspsClient.prototype.</span>presentStatus (status)](#apidoc.element.shipit.UspsClient.prototype.presentStatus)
- description and source-code
```javascript
presentStatus = function (status) {
  return ShipperClient.STATUS_TYPES.UNKNOWN;
}
```
- example usage
```shell
...
if (data == null) {
  return {
    activities: activities,
    status: status
  };
}
$ = data.$, rightNow = data.rightNow;
status = this.presentStatus($(".latest-event-status").text());
rows = $("div[data-a-expander-name=event-history-list] .a-box");
for (_i = 0, _len = rows.length; _i < _len; _i++) {
  row = rows[_i];
  columns = $($(row).find(".a-row")[0]).children('.a-column');
  if (columns.length === 2) {
    timeOfDay = $(columns[0]).text().trim();
    if (timeOfDay === '--') {
...
```

#### <a name="apidoc.element.shipit.UspsClient.prototype.presentTimestamp"></a>[function <span class="apidocSignatureSpan">shipit.UspsClient.prototype.</span>presentTimestamp (dateString, timeString)](#apidoc.element.shipit.UspsClient.prototype.presentTimestamp)
- description and source-code
```javascript
presentTimestamp = function (dateString, timeString) {
  if (dateString == null) {
    return;
  }
  timeString = (timeString != null ? timeString.length : void 0) ? timeString : '12:00 am';
  return moment("" + dateString + " " + timeString + " +0000").toDate();
}
```
- example usage
```shell
...
}
rawActivities.reverse();
_ref1 = rawActivities || [];
for (_i = 0, _len = _ref1.length; _i < _len; _i++) {
  rawActivity = _ref1[_i];
  rawLocation = (_ref2 = rawActivity['ServiceArea']) != null ? (_ref3 = _ref2[0]) != null ? (_ref4 = _ref3['Description']) != null
 ? _ref4[0] : void 0 : void 0 : void 0;
  location = this.presentAddress(rawLocation);
  timestamp = this.presentTimestamp((_ref5 = rawActivity['Date']) != null ? _ref5[0] : void 0, (_ref6 = rawActivity['Time']) !=
null ? _ref6[0] : void 0);
  details = this.presentDetails(rawLocation, (_ref7 = rawActivity['ServiceEvent']) != null ? (_ref8 = _ref7[0]) != null ? (_ref9
 = _ref8['Description']) != null ? _ref9[0] : void 0 : void 0 : void 0);
  if ((details != null) && (timestamp != null)) {
    details = details.slice(-1) === '.' ? details.slice(0, -1) : details;
    activity = {
      timestamp: timestamp,
      location: location,
      details: details
...
```

#### <a name="apidoc.element.shipit.UspsClient.prototype.requestOptions"></a>[function <span class="apidocSignatureSpan">shipit.UspsClient.prototype.</span>requestOptions (_arg)](#apidoc.element.shipit.UspsClient.prototype.requestOptions)
- description and source-code
```javascript
requestOptions = function (_arg) {
  var clientIp, endpoint, test, trackingNumber, xml;
  trackingNumber = _arg.trackingNumber, clientIp = _arg.clientIp, test = _arg.test;
  endpoint = test ? 'ShippingAPITest.dll' : 'ShippingAPI.dll';
  xml = this.generateRequest(trackingNumber, clientIp);
  return {
    method: 'GET',
    uri: "http://production.shippingapis.com/" + endpoint + "?API=TrackV2&XML=" + xml
  };
}
```
- example usage
```shell
...
      return cb(null, presentedResponse);
    };
  })(this));
};

ShipperClient.prototype.requestData = function(requestData, cb) {
  var opts, _ref;
  opts = this.requestOptions(requestData);
  opts.timeout = (requestData != null ? requestData.timeout : void 0) || ((_ref = this.options) != null ? _ref.timeout : void 0);
  return request(opts, (function(_this) {
    return function(err, response, body) {
      if ((body == null) || (err != null)) {
        return cb(err);
      }
      if (response.statusCode !== 200) {
...
```

#### <a name="apidoc.element.shipit.UspsClient.prototype.validateResponse"></a>[function <span class="apidocSignatureSpan">shipit.UspsClient.prototype.</span>validateResponse (response, cb)](#apidoc.element.shipit.UspsClient.prototype.validateResponse)
- description and source-code
```javascript
validateResponse = function (response, cb) {
  var handleResponse;
  handleResponse = function(xmlErr, trackResult) {
    var trackInfo, _ref2, _ref3;
    trackInfo = trackResult != null ? (_ref2 = trackResult['TrackResponse']) != null ? (_ref3 = _ref2['TrackInfo']) != null ? _ref3
[0] : void 0 : void 0 : void 0;
    if ((xmlErr != null) || (trackInfo == null)) {
      return cb(xmlErr);
    }
    return cb(null, trackInfo);
  };
  this.parser.reset();
  return this.parser.parseString(response, handleResponse);
}
```
- example usage
```shell
...
  if (postalCode != null ? postalCode.length : void 0) {
    address = address != null ? "" + address + " " + postalCode : postalCode;
  }
  return address;
};

ShipperClient.prototype.presentResponse = function(response, requestData, cb) {
  return this.validateResponse(response, (function(_this) {
    return function(err, shipment) {
      var activities, adjustedEta, eta, presentedResponse, status, _ref, _ref1;
      if ((err != null) || (shipment == null)) {
        return cb(err);
      }
      _ref = _this.getActivitiesAndStatus(shipment), activities = _ref.activities, status = _ref.status;
      eta = _this.getEta(shipment);
...
```



# <a name="apidoc.module.shipit.a1"></a>[module shipit.a1](#apidoc.module.shipit.a1)

#### <a name="apidoc.element.shipit.a1.A1Client"></a>[function <span class="apidocSignatureSpan">shipit.a1.</span>A1Client (options)](#apidoc.element.shipit.a1.A1Client)
- description and source-code
```javascript
function A1Client(options) {
  this.options = options;
  A1Client.__super__.constructor.apply(this, arguments);
  this.parser = new Parser();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.shipit.amazon"></a>[module shipit.amazon](#apidoc.module.shipit.amazon)

#### <a name="apidoc.element.shipit.amazon.AmazonClient"></a>[function <span class="apidocSignatureSpan">shipit.amazon.</span>AmazonClient (options)](#apidoc.element.shipit.amazon.AmazonClient)
- description and source-code
```javascript
function AmazonClient(options) {
  this.options = options;
  STATUS_MAP[ShipperClient.STATUS_TYPES.DELAYED] = ['delivery attempted'];
  STATUS_MAP[ShipperClient.STATUS_TYPES.DELIVERED] = ['delivered'];
  STATUS_MAP[ShipperClient.STATUS_TYPES.OUT_FOR_DELIVERY] = ['out for delivery'];
  STATUS_MAP[ShipperClient.STATUS_TYPES.SHIPPING] = ['in transit to carrier', 'shipping soon'];
  STATUS_MAP[ShipperClient.STATUS_TYPES.EN_ROUTE] = ['on the way', 'package arrived', 'package received', 'shipment departed', '
shipment arrived'];
  DAYS_OF_THE_WEEK['SUNDAY'] = 0;
  DAYS_OF_THE_WEEK['MONDAY'] = 1;
  DAYS_OF_THE_WEEK['TUESDAY'] = 2;
  DAYS_OF_THE_WEEK['WEDNESDAY'] = 3;
  DAYS_OF_THE_WEEK['THURSDAY'] = 4;
  DAYS_OF_THE_WEEK['FRIDAY'] = 5;
  DAYS_OF_THE_WEEK['SATURDAY'] = 6;
  AmazonClient.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.shipit.canada_post"></a>[module shipit.canada_post](#apidoc.module.shipit.canada_post)

#### <a name="apidoc.element.shipit.canada_post.CanadaPostClient"></a>[function <span class="apidocSignatureSpan">shipit.canada_post.</span>CanadaPostClient (_arg, options)](#apidoc.element.shipit.canada_post.CanadaPostClient)
- description and source-code
```javascript
function CanadaPostClient(_arg, options) {
  this.username = _arg.username, this.password = _arg.password;
  this.options = options;
  CanadaPostClient.__super__.constructor.apply(this, arguments);
  this.parser = new Parser();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.shipit.dhl"></a>[module shipit.dhl](#apidoc.module.shipit.dhl)

#### <a name="apidoc.element.shipit.dhl.DhlClient"></a>[function <span class="apidocSignatureSpan">shipit.dhl.</span>DhlClient (_arg, options)](#apidoc.element.shipit.dhl.DhlClient)
- description and source-code
```javascript
function DhlClient(_arg, options) {
  this.userId = _arg.userId, this.password = _arg.password;
  this.options = options;
  DhlClient.__super__.constructor.apply(this, arguments);
  this.parser = new Parser();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.shipit.dhlgm"></a>[module shipit.dhlgm](#apidoc.module.shipit.dhlgm)

#### <a name="apidoc.element.shipit.dhlgm.DhlGmClient"></a>[function <span class="apidocSignatureSpan">shipit.dhlgm.</span>DhlGmClient (options)](#apidoc.element.shipit.dhlgm.DhlGmClient)
- description and source-code
```javascript
function DhlGmClient(options) {
  this.options = options;
  STATUS_MAP[ShipperClient.STATUS_TYPES.DELIVERED] = ['delivered'];
  STATUS_MAP[ShipperClient.STATUS_TYPES.EN_ROUTE] = ['transferred', 'cleared', 'received', 'processed', 'sorted', 'sorting complete
', 'arrival', 'tendered'];
  STATUS_MAP[ShipperClient.STATUS_TYPES.OUT_FOR_DELIVERY] = ['out for delivery'];
  STATUS_MAP[ShipperClient.STATUS_TYPES.SHIPPING] = ['electronic notification received'];
  DhlGmClient.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.shipit.fedex"></a>[module shipit.fedex](#apidoc.module.shipit.fedex)

#### <a name="apidoc.element.shipit.fedex.FedexClient"></a>[function <span class="apidocSignatureSpan">shipit.fedex.</span>FedexClient (_arg, options)](#apidoc.element.shipit.fedex.FedexClient)
- description and source-code
```javascript
function FedexClient(_arg, options) {
  this.key = _arg.key, this.password = _arg.password, this.account = _arg.account, this.meter = _arg.meter;
  this.options = options;
  FedexClient.__super__.constructor.apply(this, arguments);
  this.parser = new Parser();
  this.builder = new Builder({
    renderOpts: {
      pretty: false
    }
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.shipit.lasership"></a>[module shipit.lasership](#apidoc.module.shipit.lasership)

#### <a name="apidoc.element.shipit.lasership.LasershipClient"></a>[function <span class="apidocSignatureSpan">shipit.lasership.</span>LasershipClient (options)](#apidoc.element.shipit.lasership.LasershipClient)
- description and source-code
```javascript
function LasershipClient(options) {
  this.options = options;
  LasershipClient.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.shipit.ontrac"></a>[module shipit.ontrac](#apidoc.module.shipit.ontrac)

#### <a name="apidoc.element.shipit.ontrac.OnTracClient"></a>[function <span class="apidocSignatureSpan">shipit.ontrac.</span>OnTracClient (options)](#apidoc.element.shipit.ontrac.OnTracClient)
- description and source-code
```javascript
function OnTracClient(options) {
  this.options = options;
  OnTracClient.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.shipit.prestige"></a>[module shipit.prestige](#apidoc.module.shipit.prestige)

#### <a name="apidoc.element.shipit.prestige.PrestigeClient"></a>[function <span class="apidocSignatureSpan">shipit.prestige.</span>PrestigeClient (options)](#apidoc.element.shipit.prestige.PrestigeClient)
- description and source-code
```javascript
function PrestigeClient(options) {
  this.options = options;
  PrestigeClient.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.shipit.shipper"></a>[module shipit.shipper](#apidoc.module.shipit.shipper)

#### <a name="apidoc.element.shipit.shipper.ShipperClient"></a>[function <span class="apidocSignatureSpan">shipit.shipper.</span>ShipperClient ()](#apidoc.element.shipit.shipper.ShipperClient)
- description and source-code
```javascript
function ShipperClient() {}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.shipit.ups"></a>[module shipit.ups](#apidoc.module.shipit.ups)

#### <a name="apidoc.element.shipit.ups.UpsClient"></a>[function <span class="apidocSignatureSpan">shipit.ups.</span>UpsClient (_arg, options)](#apidoc.element.shipit.ups.UpsClient)
- description and source-code
```javascript
function UpsClient(_arg, options) {
  this.licenseNumber = _arg.licenseNumber, this.userId = _arg.userId, this.password = _arg.password;
  this.options = options;
  UpsClient.__super__.constructor.apply(this, arguments);
  this.parser = new Parser();
  this.builder = new Builder({
    renderOpts: {
      pretty: false
    }
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.shipit.upsmi"></a>[module shipit.upsmi](#apidoc.module.shipit.upsmi)

#### <a name="apidoc.element.shipit.upsmi.UpsMiClient"></a>[function <span class="apidocSignatureSpan">shipit.upsmi.</span>UpsMiClient (options)](#apidoc.element.shipit.upsmi.UpsMiClient)
- description and source-code
```javascript
function UpsMiClient(options) {
  this.options = options;
  STATUS_MAP[ShipperClient.STATUS_TYPES.DELIVERED] = ['delivered'];
  STATUS_MAP[ShipperClient.STATUS_TYPES.EN_ROUTE] = ['transferred', 'received', 'processed', 'sorted', 'post office entry'];
  STATUS_MAP[ShipperClient.STATUS_TYPES.OUT_FOR_DELIVERY] = ['out for post office delivery'];
  STATUS_MAP[ShipperClient.STATUS_TYPES.SHIPPING] = ['shipment information received'];
  UpsMiClient.__super__.constructor.apply(this, arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.shipit.usps"></a>[module shipit.usps](#apidoc.module.shipit.usps)

#### <a name="apidoc.element.shipit.usps.UspsClient"></a>[function <span class="apidocSignatureSpan">shipit.usps.</span>UspsClient (_arg, options)](#apidoc.element.shipit.usps.UspsClient)
- description and source-code
```javascript
function UspsClient(_arg, options) {
  this.userId = _arg.userId;
  this.options = options;
  UspsClient.__super__.constructor.apply(this, arguments);
  this.parser = new Parser();
  this.builder = new Builder({
    renderOpts: {
      pretty: false
    }
  });
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
