# Here's the steps to starting up the nginx-docker reverse proxy
### Before starting - download Docker for your device from the official site
## Steps
1. Clone this repository
```sh 
git clone https://github.com/Rishi5154/CS3219AssignmentA.git
```
2. Build the repo as a docker image
```sh 
docker build -t webserver .
```
3. Run the container with following command
```sh 
docker run -it --rm -d -p 80:80 --name web webserver
```
4. Now go to [localhost](https://localhost) to access the static html file using **nginx** as reverse proxy server