# API endpoints

These endpoints allow you to recommend price .

## POST
 [/v1/price]<br/>
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

