
# Usage

The daily network data usage of a single device during a specified time period.

## Structure

`Usage`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `BytesUsed` | `long?` | Optional | The number of bytes that the device sent or received on the report date. |
| `ExtendedAttributes` | [`List<CustomFields>`](../../doc/models/custom-fields.md) | Optional | The number of mobile-originated and mobile-terminated SMS messages on the report date. |
| `ServicePlan` | `string` | Optional | The list of service plans associated with the device/account. |
| `SmsUsed` | `int?` | Optional | The number of SMS messages that were sent or received on the report date. |
| `Source` | `string` | Optional | The source of the information for the reported usage. |
| `Timestamp` | `string` | Optional | The date of the recorded usage. |

## Example (as JSON)

```json
{
  "bytesUsed": 4096,
  "extendedAttributes": [
    {
      "key": "MoSms",
      "value": "0"
    }
  ],
  "smsUsed": 0,
  "source": "Raw Usage",
  "timestamp": "2020-12-01T00:00:00Z",
  "servicePlan": "servicePlan6"
}
```

