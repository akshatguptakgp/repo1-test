# API endpoints

These endpoints allow you to recommend price .

## POST
`official client only` [/1/billing/start-trial.json](#post-1billingstart-trialjson) <br/>
`official client only` [/1/billing/cancel-trial.json](#post-1billingcancel-trialjson) <br/>
`official client only` [/1/billing/start-or-update-subscription.json](#post-1billingstart-or-update-subscriptionjson) <br/>
`official client only` [/1/billing/cancel-subscription.json](#post-1billingcancel-subscriptionjson) <br/>
___

**Parameters**

|          Name | Required |  Type   | Description                                                                                                                                                           |
| -------------:|:--------:|:-------:| --------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|     `name` | required | string  | The product name. <br/><br/> Supported values: `string` |
|     `item_condition_id` | required | int  | The condition id for the product. <br/><br/>  Supported values: `int`        |
|     `category_name` | required | string  | The category name for the product. <br/><br/>  Supported values: `string`        |

**Response**

```
// Customer has no subscription
{
    "price": 0
}


```
___

