# camera microservice

provides out-of-the-box functionality for robotics and ai in the form of a simple and robust rest api

## requirements

* python3
* flask
* time
* json
* sys
* cv2

## usage

`python app.py <port (optional), default 6000>`

Endpoint | Function | Description | Example
--- | --- | --- | ---
/ | GET | Returns default dictionary | `{time: unix epoch, img0: serialized ndarray}`
/stereo | GET | Returns stereo dictionary | `{time: unix epoch, img0: serialized ndarray, img1: serialized ndarray}`
