# nearest-pantone

JavaScript library to find the nearest Pantone color name for a given hex color. It uses CIEDE2000 color difference algorithm


### Prerequisites

```
node
```

### Installing

This module is also available as a NPM module, just install and start using in your project

You can view it at (NPM Link)[https://www.npmjs.com/package/nearest-pantone]

Install the NPM module using the following command 

```
npm install nearest-pantone
```

And then require the module in your code by adding this:

```
const pant = require("nearest-pantone")
```

The input color needs to in HEX format eg. "#b37256"

Pass the input color as an argument in the following function

```
pant.getClosestColor(inputColor)
```

It'll return an object like this 

```
{
	pantone : "16-1429", 
	name: "sunburn", 
	hex: "#b37256"
}
```

Here is a complete example to print the pantone name of the nearest color

```
const pant = require("nearest-pantone")

const inputColor = "#b37256"
const pantoneColor = pant.getClosestColor(inputColor)

console.log(pantoneColor.name)

// prints : sunburn
```

## Built With

* [Color Diff](https://github.com/markusn/color-diff)


## Versioning

We use [SemVer](http://semver.org/) for versioning

## Authors

* **Saurabh Suman** - *Founder, Total Internal Reflection*

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details
