# Use deep learning in your applications

You can use ready-to-use deep learning microservices from the Model Asset Exchange (MAX) that are running on the IBM Cloud to 
- detect objects in images,
- generate image captions,
- identify sounds,
- convert speech to text,
- and much more!

You can find a complete list at https://developer.ibm.com/exchanges/models/all/
- Pick a model that might be of interest to you (e.g. the [Object Detector](https://developer.ibm.com/exchanges/models/all/max-object-detector/))
- Click "Try the API" 

---
## Sample JavaScript code pens

You can consume these microservices in your web browser using JavaScript.

![web app example](doc/images/javascript_pens.png)

What you need:
 - Web browser
 
- Open https://codepen.io/collection/DzdpJM/#
- Try one of the examples

---
## Sample web applications

Identify objects (people, animals, etc) in images! 
- Goto https://developer.ibm.com/exchanges/models/all/max-object-detector/
- Click "Try the web-app" to see the demo (no installation required)

![web app example](doc/images/sample_web_app.png)

You can create a custom version of this web app using the Python and Node.js examples.

### What you need:
 - Python (v3.x) or Node.js (v10+)
 - git (optional)


### Steps:

- [Python instructions](https://github.com/IBM/max-tutorial-app-python/blob/solution/README.md)

  - If you have git installed, run these commands
    ```
    git clone https://github.com/IBM/max-tutorial-app-python.git
    cd max-tutorial-app-python
    pip install -r requirements.txt
    git checkout solution
    python app.py --ml-endpoint=http://max-object-detector.codait-prod-41208c73af8fca213512856c7a09db52-0000.us-east.containers.appdomain.cloud
    ```

  - If you don't have git installed, 
    - Open https://github.com/IBM/max-tutorial-app-python/tree/solution
    - Click "Clone or download"
    - Click "Download ZIP"
    - Run these commands in the extracted `max-tutorial-app-python-solution` directory
      ```
      pip install -r requirements.txt
      git checkout solution
      python app.py --ml-endpoint=http://max-object-detector.codait-prod-41208c73af8fca213512856c7a09db52-0000.us-east.containers.appdomain.cloud
      ```
      
  - Open http://localhost:8090 in your web browser

- [Node.js instructions](https://github.com/IBM/max-tutorial-app-nodejs/blob/solution/README.md)

  - If you have git installed, run these commands
    ```
    git clone https://github.com/IBM/max-tutorial-app-nodejs.git
    cd max-tutorial-app-nodejs
    git checkout solution
    npm install
    node app.js --model=http://max-object-detector.codait-prod-41208c73af8fca213512856c7a09db52-0000.us-east.containers.appdomain.cloud
    ```

  - If you don't have git installed, 
    - Open https://github.com/IBM/max-tutorial-app-nodejs/tree/solution
    - Click "Clone or download"
    - Click "Download ZIP"
    - Run these commands in the extracted `max-tutorial-app-nodejs-solution` directory
      ```
      npm install
      node app.js --model=http://max-object-detector.codait-prod-41208c73af8fca213512856c7a09db52-0000.us-east.containers.appdomain.cloud
      ```

  - Open http://localhost:8090 in your web browser

---
## Internet of Things deep learning sample

You can consume the microservices in an Internet of Things (IOT) application.

![IOT example](doc/images/iot.png)

What you need:
- [Docker Desktop](https://www.docker.com/products/docker-desktop)

### Steps

Follow the instructions in https://github.com/CODAIT/max-node-red-docker-image. Additional details can be found in https://github.com/CODAIT/node-red-contrib-model-asset-exchange.
