# bs-utils
A collective list of APIs for PSP Added Value Services search payment instruments

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

The platform provides the following services  :

- CheckIban
- Payment Instruments

### Check-Iban
This service lets the client retrieve the account holder validation for a specific fiscal code.

_TBD_

### Payment Instruments

This service lets the client retrieve the payment instruments for a specific fiscal code.

Banking Services platform ( named BS ) provides the search payment instruments service.
BS is connected to many `card services` in order to enquiring , each service search 
The Services inq


This endpoint lets the user retrieve the payment instruments for a specific fiscal code.
