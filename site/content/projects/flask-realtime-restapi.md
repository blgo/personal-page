---
title: Flask Realtime RESTapi
image: img/screenshotfrom20180109141814.png
weight: 1
date: 2018-01-09T00:07:14.000Z
external_link: ''
---
Try the <a href="http://82.38.27.16:5000">Live Demo</a>, _which in fact is my experimental hydroponic greenhouse_, or run it yourself from the <a href="https://hub.docker.com/r/blgo/flask-realtime-restapi/">Docker image</a>

> The hydroponic automation mentioned above consists of a Raspberry Pi and a humidity/temperature sensor connected. A Python script and Adafruit libraries, take care of controlling the sensor and sending the reading to the REST API.
>
> \
>
>
>
>
> \
>
>
> The REST API, the MongoDB instance and the web application and the Websockets server, are running in the same Raspberry Pi. 
>
> \
>
>
>
>
> \
>
>
> I am still implementing and researching which PH and EC sensors are best for continous reading.

Github <a href="https://github.com/blgo/flask-realtime-restapi">repository and documentation</a>.

For quite a while, I wanted to start writting my own IoT hub from scratch, with realtime charts (using Websockets) and REST endpoints.

I didn't know it was such a vast universe! It makes me think about this quote "the more you know the less you know".

This application displays temperature and humidity readings in a timeline, received on the REST endpoint /sensor1. Also, it shows latency and server events log.

1. <b>Realtime updates:</b> Uses Flask-SocketIO and Eventlet.</br>
2. <b>RESTful:</b> Flask-RESTful api provides function wrappers and predefined methods (GET, POST, PUT, DELETE).</br>
3. <b>Charts:</b> Charts.js: Fast and lightweight.</br>
4. <b>Database: Mongoengine is a simple declarative API, similar to the Django ORM. MongoDB offers flexibility and low maintenance  permanent storage.</br>
   </br>
