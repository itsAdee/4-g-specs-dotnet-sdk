
# Change Pmec Device Profile Request

## Structure

`ChangePmecDeviceProfileRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `AccountName` | `string` | Required | - |
| `DeviceList` | [`List<MECDeviceList>`](../../doc/models/mec-device-list.md) | Required | - |
| `NewProfile` | `string` | Required | - |

## Example (as JSON)

```json
{
  "accountName": "0342351414-00001",
  "deviceList": [
    {
      "deviceIds": [
        {
          "id": "99948099913024600000",
          "kind": "iccid"
        }
      ]
    }
  ],
  "newProfile": "HSS EsmProfile Enterprise 5G internet"
}
```

