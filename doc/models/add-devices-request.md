
# Add Devices Request

Request to add the devices.

## Structure

`AddDevicesRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `State` | `string` | Required | The initial service state for the devices. The only valid state is “Preactive.” |
| `DevicesToAdd` | [`List<AccountDeviceList>`](../../doc/models/account-device-list.md) | Required | The devices that you want to add. |
| `AccountName` | `string` | Optional | The billing account to which the devices are added. |
| `CustomFields` | [`List<CustomFields>`](../../doc/models/custom-fields.md) | Optional | The names and values for any custom fields that you want set for the devices as they are added to the account. |
| `GroupName` | `string` | Optional | The name of a device group to add the devices to. They are added to the default device group if you don't include this parameter. |
| `SkuNumber` | `string` | Optional | The Stock Keeping Unit (SKU) number of a 4G device type with an embedded SIM. |
| `SmsrOid` | `string` | Optional | **Constraints**: *Minimum Length*: `3`, *Maximum Length*: `32`, *Pattern*: `^[A-Za-z0-9]{3,32}$` |

## Example (as JSON)

```json
{
  "accountName": "0868924207-00001",
  "customFields": [
    {
      "key": "CustomField2",
      "value": "SuperVend"
    }
  ],
  "devicesToAdd": [
    {
      "deviceIds": [
        {
          "kind": "imei",
          "id": "990013907835573"
        },
        {
          "kind": "iccid",
          "id": "89141390780800784259"
        }
      ],
      "ipAddress": "ipAddress2"
    },
    {
      "deviceIds": [
        {
          "kind": "imei",
          "id": "990013907884259"
        },
        {
          "kind": "iccid",
          "id": "89141390780800735573"
        }
      ],
      "ipAddress": "ipAddress2"
    }
  ],
  "groupName": "West Region",
  "state": "preactive",
  "skuNumber": "skuNumber2",
  "smsrOid": "smsrOid6"
}
```
