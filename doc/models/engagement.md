
# Engagement

The engagements associated with the account.

## Structure

`Engagement`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `EngagementId` | `string` | Optional | The engagement ID. |
| `ChargingGroup` | `string` | Optional | The charging group name. |
| `Services` | [`List<AccountService>`](../../doc/models/account-service.md) | Optional | The services associated with the account. |

## Example (as JSON)

```json
{
  "engagementId": "1234",
  "chargingGroup": "Engagement1234",
  "services": [
    {
      "name": "Svc1",
      "description": "Usage Segmentation - Main Line.",
      "states": [
        {
          "name": "Svc1 Activate",
          "workflowSequenceNumber": 1.0,
          "servicePlans": [
            "4523aef7250f67205fd5",
            "4d4090c0f2d48814c94d"
          ]
        },
        {
          "name": "Svc1 No Telematics",
          "workflowSequenceNumber": 3.0,
          "servicePlans": [
            "4523aef7250f67205fd5",
            "4d4090c0f2d48814c94d"
          ]
        },
        {
          "name": "Svc1 Deactivate",
          "workflowSequenceNumber": 2.0,
          "servicePlans": [
            "4523aef7250f67205fd5",
            "4d4090c0f2d48814c94d"
          ]
        }
      ]
    },
    {
      "name": "WIFI",
      "description": "Usage Segmentation - WiFi.",
      "states": [
        {
          "name": "WIFI Redirect",
          "workflowSequenceNumber": 2.0,
          "servicePlans": [
            "4d4090c0f2d48814c94d"
          ]
        },
        {
          "name": "WIFI Trial",
          "workflowSequenceNumber": 4.0,
          "servicePlans": [
            "4d4090c0f2d48814c94d"
          ]
        },
        {
          "name": "WIFI Goodwill",
          "workflowSequenceNumber": 6.0,
          "servicePlans": [
            "4d4090c0f2d48814c94d"
          ]
        },
        {
          "name": "WIFI Disable",
          "workflowSequenceNumber": 3.0,
          "servicePlans": [
            "4d4090c0f2d48814c94d"
          ]
        }
      ]
    }
  ]
}
```

