## IoT Hub
#### Create an IoT Hub
~~~
Azure -> IoT Hub -> Create an IoT Hub
~~~

#### Retrieve the Device Connection String
~~~
IoT Hub -> IoT Hub Name -> Security settings -> Shared access policies -> iothubowner -> Primary connection string
~~~

#### Create new Consumer group (used to receive the messages on Device on IoT Explorer)
~~~
IoT Hub -> IoT Hub Name -> Hub settings -> Buit-in endpoints -> Create new consumer group
~~~

#### Register a New IoT Device
~~~
IoT Hub -> Iot Hub Name -> Device management -> Create a device
~~~

#### Retrieve the Device Connection String
~~~
IoT Hub ->  Device management -> Devices -> Device name -> Primary Connection String
~~~

## IoT Explorer (IoT Hub local client)
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

## Raspberry Pi Azure IoT Online Simulator
~~~
https://azure-samples.github.io/raspberry-pi-web-simulator/
~~~

## Important Commands
~~~
brew install azure-cli
~~~
~~~
az extension add --name azure-iot
~~~
~~~
az extension list
~~~
#### Change Consumer Group for IoT device receiving messages
~~~
az iot hub monitor-events --hub-name F3-IT --consumer-group arslan-haider-consumer-group --device-id arslan-haider-device
~~~