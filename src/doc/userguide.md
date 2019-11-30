## Introduction

The NGSI Registration Browser widgets allows you to browse the registrations
managed by a given
[Orion Context Broker](https://www.fiware.org/developers/catalogue/)
server in a easy and paginated way. This is accomplished using GET querys to the
v2 of the Context Broker API, so updates made into the context broker are not
reflected immediately when using this widget.

## Settings

- **NGSI server URL:** URL of the Orion Context Broker to use for retrieving
  entity information.
- **Use the FIWARE credentials of the user:** Use the FIWARE credentials of the
  user logged into WireCloud. Take into account this option cannot be enabled if
  you want to use this widget in a public workspace as anonoymous users doesn't
  have a valid FIWARE auth token. As an alternative, you can make use of the
  "Use the FIWARE credentials of the workspace owner" preference.
- **Use the FIWARE credentials of the dashboard owner**: Use the FIWARE
  credentials of the owner of the workspace. This preference takes preference
  over "Use the FIWARE credentials of the user". This feature is available on
  WireCloud 0.7.0+ in a experimental basis, future versions of WireCloud can
  change the way to use it making this option not funcional and requiring you to
  upgrade this widget.
- **NGSI tenant/service**: Tenant/service to use when connecting to the context
  broker. Must be a string of alphanumeric characters (lowercase) and the `_`
  symbol. Maximum length is 50 characters. If empty, the default tenant will be
  used
- **NGSI scope**: Scope/path to use when connecting to the context broker. Must
  be a string of alphanumeric characters (lowercase) and the `_` symbol
  separated by `/` slashes. Maximum length is 50 characters. If empty, the
  default service path will be used: `/`
- **Edit button**: Display a edit button for editing a registration information
- **Delete button**: Display a delete button for deleting a registration

## Wiring


##### Input Endpoints

-  **Reload:** This widget reloads all the information and the table when
   something arrives at this endpoint


##### Output Endpoints

- This widget has no output endpoint
