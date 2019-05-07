# ![LOGO](logo.png) InstanceMetadataClient **flow**ground Connector

## Description

A generated **flow**ground connector for the InstanceMetadataClient API (version 2018-10-01).

Generated from: https://api.apis.guru/v2/specs/azure.com/imds/2018-10-01/swagger.json<br/>
Generated at: 2019-05-07T17:38:13+03:00

## API Description

The Azure Instance Metadata Client

## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Get Attested Data for the Virtual Machine.

#### Input Parameters
* `api-version` - _required_ - This is the API version to use.
    Possible values: 2018-10-01.
* `nonce` - _optional_ - This is a string of up to 32 random alphanumeric characters.
* `Metadata` - _required_ - This must be set to 'true'.
    Possible values: true.

### Get information about AAD Metadata

*Tags:* `Get metadata information`

#### Input Parameters
* `Metadata` - _required_ - This must be set to 'true'.
    Possible values: true.
* `api-version` - _required_ - This is the API version to use.
    Possible values: 2018-10-01.

### Get a Token from Azure AD

*Tags:* `Get token`

#### Input Parameters
* `Metadata` - _required_ - This must be set to 'true'.
    Possible values: true.
* `resource` - _required_ - This is the urlencoded identifier URI of the sink resource for the requested Azure AD token. The resulting token contains the corresponding aud for this resource.
* `api-version` - _required_ - This is the API version to use.
    Possible values: 2018-10-01.
* `client_id` - _optional_ - This identifies, by Azure AD client id, a specific explicit identity to use when authenticating to Azure AD. Mutually exclusive with object_id and msi_res_id.
* `object_id` - _optional_ - This identifies, by Azure AD object id, a specific explicit identity to use when authenticating to Azure AD. Mutually exclusive with client_id and msi_res_id.
* `msi_res_id` - _optional_ - This identifies, by urlencoded ARM resource id, a specific explicit identity to use when authenticating to Azure AD. Mutually exclusive with client_id and object_id.
* `authority` - _optional_ - This indicates the authority to request AAD tokens from. Defaults to the known authority of the identity to be used.
* `bypass_cache` - _optional_ - If provided, the value must be 'true'. This indicates to the server that the token must be retrieved from Azure AD and cannot be retrieved from an internal cache.
    Possible values: true.

### Get Instance Metadata for the Virtual Machine.

#### Input Parameters
* `api-version` - _required_ - This is the API version to use.
    Possible values: 2018-10-01.
* `Metadata` - _required_ - This must be set to 'true'.
    Possible values: true.

## License

**flow**ground :- Telekom iPaaS / azure-com-imds-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
