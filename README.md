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

> Folder structure options and naming conventions for software projects

### A typical top-level directory layout

    .
    ├── src                   # files for the main code
    ├── log                   # folder for placing log files 
    ├── data                  # Dataset for recommendation
    ├── .env                  # env file for environment variables
    ├── .gitignore            # ignoring files with certain extensions
    ├── config.py             # configuration variables for the code
    ├── DockerFile            # DockerFile to dockerize the code
    ├── README.md             # README.md
    ├── requirements.txt      # requirements file
    ├── setup.sh              # building the docker
    ├── start.sh              # running the docker
    └── test.sh               # testing the docker with sample request


#### Running docker file

After cloning the code, go the base path ./ (where DockerFile is located)

```sh
# Run the setup.sh, which builds the image
$ bash setup.sh

# Run the start.sh, which runs the image
$ bash start.sh

# Run the test.sh, which runs a sample curl request
$ bash test.sh




