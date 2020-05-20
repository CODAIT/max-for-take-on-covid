# Use deep learning in your applications

You can use ready-to-use deep learning microservices that are running on the IBM Cloud
- Goto https://developer.ibm.com/exchanges/models/all/
- Pick a model that seems interesting to you (e.g. the [Object Detector](https://developer.ibm.com/exchanges/models/all/max-object-detector/)
- Click "Try the API" 


## Sample code pens

What you need:
 - web browser

## Sample web applications

Identify objects (people, animals, etc) in images! 
- Goto https://developer.ibm.com/exchanges/models/all/max-object-detector/
- Click "Try the web-app" to see the demo (no installation required)

You can write your own web app using these examples.

What you need:
 - Python (v3.x) or Node.js (v10+)

- [Python](https://github.com/IBM/max-tutorial-app-python/blob/solution/README.md)

  - Run these commands
   ```
   git clone https://github.com/IBM/max-tutorial-app-python.git
   cd max-tutorial-app-python
   pip install -r requirements.txt
   git checkout solution
   python app.py --ml-endpoint=http://max-object-detector.codait-prod-41208c73af8fca213512856c7a09db52-0000.us-east.containers.appdomain.cloud
   ```
  - Open http://localhost:8090 in your web browser

- [Node.js](https://github.com/IBM/max-tutorial-app-nodejs/blob/solution/README.md)
  ```
  git clone https://github.com/IBM/max-tutorial-app-nodejs.git
  cd max-tutorial-app-nodejs
  git checkout solution
  npm install
  node app.js --model=http://max-object-detector.codait-prod-41208c73af8fca213512856c7a09db52-0000.us-east.containers.appdomain.cloud
  ```
    - Open http://localhost:8090 in your web browser


## Internet of Things deep learning sample

What you need:
- Docker Desktop

https://github.com/CODAIT/max-node-red-docker-image
