# About

noisehx is a teeny weeny library to generate Perlin noise.
The code is a port of [noisejs](https://github.com/josephg/noisejs) by [Joseph Gentle](https://github.com/josephg),
	which is based on Stefan Gustavson's implementation.

# Setting up

To install, use the command:
`haxelib git noisehx https://github.com/madhoe/noisehx.git`
	
# Example
```
// If no seed passed into constructor, a random one is used.
var perlin:Perlin = new Perlin();

for (x in 0...100)
{
	for (y in 0...100)
	{
		var value:Float = perlin.noise2d(x / 10.0, y / 10.0);
		// Do stuff with it...
	}
}
```