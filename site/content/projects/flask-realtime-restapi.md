---
title: "Flask Realtime RESTapi"
date: 2018-01-09T00:07:14Z
image: "img/screenshotfrom20180109141814.png"
external_link: ""
weight: 1
draft: false
---
Try the <a href="http://82.38.27.16:5000">Live Demo</a> or run the <a href="https://hub.docker.com/r/blgo/flask-realtime-restapi/">Docker image</a>

I have a Raspberry Pi sending data to the REST endpoint every minute.

Github <a href="https://github.com/blgo/flask-realtime-restapi">repository and documentation</a>.

For quite a while, I wanted to start writting my own IoT hub from scratch, with realtime charts (using Websockets) and REST endpoints.

This little test project is my second attemp after a few months of learning about many web technologies, I didn't know it was such a vast universe! It makes me think about this quote "the more you know the less you know".

This application displays temperature and humidity readings in a timeline, received on the REST endpoint /sensor1. Also, it shows latency and server events log.

1. <b>Realtime updates:</b> Uses Flask-SocketIO and Eventlet.</br>
1. <b>RESTful:</b> Flask-RESTful api provides function wrappers and predefined methods (GET, POST, PUT, DELETE).</br>
1. <b>Charts:</b> Charts.js: Fast and lightweight.</br>
</br>

PD: Yes, it is a very naive implementation and easy to break, please don't :D . I hope I had all the time in world to make it bit more resiliant.
