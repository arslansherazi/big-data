# Big Data Analytics

### Setup env (Python 3.13)
~~~
brew install uv
~~~

~~~
uv venv venv-bigdata
~~~

~~~
source venv-bigdata/bin/activate
~~~

~~~
uv pip install -r requirements.txt
~~~

~~~
uv pip freeze > requirements.txt
~~~

### Add jupyter kernel (Run this command inside the venv)
Pre-requisite
~~~
uv pip install ipykernel
~~~
~~~
python -m ipykernel install --user --name=venv --display-name "bigdata-venv"
~~~

### IoT Explorer (IoT Hub Client)
~~~
git clone https://github.com/Azure/azure-iot-explorer.git
~~~
~~~
cd azure-iot-explorer
~~~
~~~
npm install
~~~
~~~
npm start
~~~
### Raspberry Pi Azure IoT Online Simulator
~~~
https://azure-samples.github.io/raspberry-pi-web-simulator/
~~~
## IoT Commands
~~~
brew install azure-cli
~~~
~~~
az extension add --name azure-iot
~~~
~~~
az extension list
~~~
### Change Consumer Group for IoT device receiving messages
~~~
az iot hub monitor-events --hub-name F3-IT --consumer-group arslan-haider-consumer-group --device-id arslan-haider-device
~~~