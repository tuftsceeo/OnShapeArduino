# Arduino OnShape API Client

An API client that allows Arduino Nano to interact with OnShape's API

## Setup/Installation

### API Key

To start, you'll want to create an API Key/Secret Key pair [here](https://dev-portal.onshape.com/keys)

### Installing Libraries

This client is made up of four libraries:

- TimeLib: Built-in library used to get dates for [request signature](https://dev-portal.onshape.com/keys)
- SHA256: Creates the HMAC digest for authorization
- [Base64](https://github.com/Densaugeo/base64_arduino): Encodes the HMAC in base 64
- OnShape: The actual client interface

TimeLib and [Base64](https://github.com/Densaugeo/base64_arduino) can be installed through the Arduino IDE's Library Manager. SHA256 and OnShape must be installed from this repository. To do so, zip the contents of each folder. Then, in the Arduino IDE, you can install these two libraries through `Sketch>Include Library>Add .ZIP Library`.

## Usage

This API client can make the same API requests that are available in OnShape's API Explorer. You can find example code through the IDE in `File>Examples>OnShape` or in this repo under `OnShape/examples'.