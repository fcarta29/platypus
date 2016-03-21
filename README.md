## Project Platypus

Platypus is an initiative to improve documentation across a number of VMware's products (see [Supported Products](#supported-products)) as described using [Open API](https://openapis.org/) and [Swagger UI](http://swagger.io/swagger-ui/). This allows everyone to easily consume, and enhance VMware's REST API's & their usage.

## Just Run it

`docker run --rm --name platypus -p 80:8080 vmware/platypus`

## Specify PRODUCT & VERSION

`docker run --name platypus --rm -p 80:8080 -e PRODUCT="vra" -e VERSION="7" vmware/platypus`

> replace vRA and version with product of your choice

## Supported Products

| Product       | Version       | Build   |
| ------------- | :---:         | :---:   |
| vRA           | 7             | 3311738 |
| vROPs         | 6.2           | 3445568 |
| vRO           | 7             | 3310032 |
| NSX			| 6.2			| 		  |


_**or**_

#### Get it

clone this repo, and then:

`git submodule update --init --recursive` to make sure you obtain the Swagger-UI code-base

#### Build it

Replace `[vmware/platypus]` with your choice of a

`docker build -t vmware/platypus .`


## Contribution

Have an idea to improve Platypus ?

1. Fork the Platypus
2. Make modifications
3. Open a PR