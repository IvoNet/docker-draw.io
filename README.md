# Draw.io contained :-)

This docker enables Draw.io
 
## usage

docker run -d --rm --name draw -p 4000:8080 -p 4443:8443 ivonet/draw.io

[localhost](http://localhost:4000?offline=1&libs=eip)
(the 'libs=eip' is optional but demonstrates the filtering of drawing tools)

## build

docker build -t ivonet/draw.io .


## Credits

The docker scripts I have here are adaptations based on [fjudith/docker-draw.io](https://github.com/fjudith/docker-draw.io)

I only tried to "improved" on it by making it a multi-stage build and eliminating some layers
my image is about 285Mb compared to the 677Mb of fjudith. Other than that fjudith deserves all the credit.
