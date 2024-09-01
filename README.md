# FluentBit

## Build the Docker Image
docker build -t fluent-bit-image .

## Run the Container for listnening UDP packets on a specified port and process the JSON data from those packets
docker run -d --name fluent-bit -p 5140:5140 fluent-bit-image

## Verify Logs
docker logs fluent-bit
