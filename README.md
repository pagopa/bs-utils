# bs-utils

A collective list of APIs for PSP Added Value Services for Banking Services Platform
Official Product documentation is available [here](https://bankingservices.pagopa.it/docs/platform/apis/pagopa-banking-v4.0)

## Overview
Banking Services platform ( named `BS` ) is connected to many value added value services ( `VAS` ) provided by Payment Services Providers in order to provides a common API interfaces to Public Administration Clients.


<!-- 
@startuml docs/media/img1
autonumber 
component bs as "Banking Services"
component psp1 as "PSP 1 VAS A" 
component psp2 as "PSP 2 VAS A"
component client as "Client"

client -> bs
bs -> psp1
bs -> psp2

@enduml 
-->

![](docs/media/img1.svg)

The platform provides the following services  :

- CheckIban
- Payment Instruments

### Check-Iban

This service lets the client retrieve the account holder validation for a specific fiscal code.

for complete description , see [here](https://bankingservices.pagopa.it/docs/platform/apis/pagopa-banking-v4.0)

### Search Payment Instruments ( SPI service)

This service lets the client retrieve the payment instruments for a specific fiscal code.
It has two operations :

- [POST] _searchPaymentInstrumentsUsingPOST_ : this operation search payment instruments for a specific fiscal code, it returns a complete list or a _request-id_
- [GET] _searchPaymentInstrumentsUsingGET_ : this operations retrieve a search results by its _request-id_

for North API, see documentation [here](north-api/pagopa_swagger_SPI.json)

for South API, see documentation _TBD_
