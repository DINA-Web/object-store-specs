# object-store-specs
Specifications for the Object Store Module (aka multimedia)

This repository aim is to collect and document the different requirements (what the module should do) and the specifications (how the module should do it). The scope is limited to what the module should do to be DINA compliant and should not target a specific institution. 

Requirements/Specifications are recorded as [Issues](https://github.com/DINA-Web/object-store-specs/issues).

# API Specifications

* Rendered version: https://dina-web.github.io/object-store-specs/
* Open API 3 Schema: https://github.com/DINA-Web/object-store-specs/blob/master/schema/metadata.yaml

# Mock Server
A mock API can be created based on the OpenAPI specifications with [Prism](https://github.com/stoplightio/prism).

`docker run --init --rm -it -p 4010:4010 -P stoplight/prism:4 mock -h 0.0.0.0 https://raw.githubusercontent.com/DINA-Web/object-store-specs/master/schema/metadata.yaml`

A mock server will now be accessible on `http://127.0.0.1:4010/v1/metadata`
