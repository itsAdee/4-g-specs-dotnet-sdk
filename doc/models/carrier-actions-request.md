
# Carrier Actions Request

Request for a carrier action.

## Structure

`CarrierActionsRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `AccountName` | `string` | Optional | The name of a billing account. |
| `CustomFields` | [`List<CustomFields>`](../../doc/models/custom-fields.md) | Optional | Custom field names and values, if you want to only include devices that have matching values. |
| `Devices` | [`List<AccountDeviceList>`](../../doc/models/account-device-list.md) | Optional | The devices for which you want to restore service, specified by device identifier. |
| `WithBilling` | `bool?` | Optional | set to "true" to suspend with billing, set to "false" to suspend without billing |
| `GroupName` | `string` | Optional | The name of a device group, if you want to restore service for all devices in that group. |
| `ServicePlan` | `string` | Optional | The name of a service plan, if you want to only include devices that have that service plan. |

## Example (as JSON)

```json
{
  "devices": [
    {
      "deviceIds": [
        {
          "id": "89148000000800139708",
          "kind": "iccid"
        }
      ],
      "ipAddress": "ipAddress4"
    }
  ],
  "accountName": "accountName0",
  "customFields": [
    {
      "key": "key0",
      "value": "value2"
    },
    {
      "key": "key0",
      "value": "value2"
    },
    {
      "key": "key0",
      "value": "value2"
    }
  ],
  "withBilling": false,
  "groupName": "groupName4"
}
```

