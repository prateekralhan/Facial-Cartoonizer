# 👻👽 Facial Cartoonizer 👾🤖

A minimalistic Web application that makes use of a simple facial image cartoonization network to generate cartoon like sketch like output for any image fed as input ( based on CVPR2020 White-box cartoonizaiton paper ).

<kbd>
<img src="https://user-images.githubusercontent.com/29462447/118412485-e4461280-b6b7-11eb-8d83-21047103f15a.png" data-canonical-src="https://user-images.githubusercontent.com/29462447/118412485-e4461280-b6b7-11eb-8d83-21047103f15a.png"/> 
</kbd>

&nbsp;


## Installation:
* Simply execute the command 8**pip install -r requirements.txt*** to install the necessary dependencies.

## Usage:
1. Clone this Repository to a directory and navigate to that directory.
2. Run the command: ***python app.py***
3. This will run the web-app on localhost. Upload your desired Image and it will automatically download the cartoonized version of the same in your system.
4. Feel free to play around with the codes, add more features, beautify it. :wink:

<kbd>
<img src="https://user-images.githubusercontent.com/29462447/118412754-67b43380-b6b9-11eb-8e10-b2096515a995.png" data-canonical-src="https://user-images.githubusercontent.com/29462447/118412754-67b43380-b6b9-11eb-8e10-b2096515a995.png"/> 
</kbd>

&nbsp;
<kbd>
<img src="https://user-images.githubusercontent.com/29462447/118412813-b366dd00-b6b9-11eb-97fe-6bb48de92aa3.png" data-canonical-src="https://user-images.githubusercontent.com/29462447/118412813-b366dd00-b6b9-11eb-97fe-6bb48de92aa3.png"/> 
</kbd>

&nbsp;
<kbd>
<img src="https://user-images.githubusercontent.com/29462447/118412815-b5c93700-b6b9-11eb-857c-53edfec80140.png" data-canonical-src="https://user-images.githubusercontent.com/29462447/118412815-b5c93700-b6b9-11eb-857c-53edfec80140.png"/> 
</kbd>

&nbsp;
<hr>
<b>NOTE:</b>
 1.  Ensure your entire web app folder structure is maintained in the same format as you see here ( as in case of Flask ).
<hr>

### Running the Dockerized App
1. Ensure you have Docker Installed and Setup in your OS (Windows/Mac/Linux). For detailed Instructions, please refer [this.](https://docs.docker.com/engine/install/)
2. Navigate to the folder where you have cloned this repository ( where the ***Dockerfile*** is present ).
3. Build the Docker Image (don't forget the dot!! :smile: ): 
```
docker build --tag sketch_app .
```
4. Run the docker:
```
docker run --publish 8000:8080 --detach --name bb sketch_app
```

This will launch the dockerized app. Navigate to ***localhost:8000*** in your browser to have a look at your application. You can check the status of your all available running dockers by:
```
docker ps
```
