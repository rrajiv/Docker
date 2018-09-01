# Instructions

Build the image
````
docker build -t akamaidev .
````

Run the image
````
docker run -it -v $HOME/.edgerc:/root/.edgerc -v $HOME/<repo>/:/src/ akamaidev
````