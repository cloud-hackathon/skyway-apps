# SkyWay video chat example

## Getting started

1. Clone sample apps

   ``` shell
   $ git clone https://github.com/cloud-hackathon/skyway-apps.git
   ```

2. Move to `sfu-videochat` directory
3. Once you’ve given it a try, sign up for the free[Community Edition](https://console-webrtc-free.ecl.ntt.com/users/registration) and get an API Key.
4. Replace the API key in the sample code with the one you got in step 3.

   ``` shell
   $ echo "window.__SKYWAY_KEY__ = '<YOUR_KEY_HERE>';" > key.js
   ```

5. Run application

   ``` shell
   $ export DOCKER_HOST=tcp://hack0[1-9].hiconyan.com:2375
   $ docker build -t sfu-videochat:[your_team_name] .
   $ docker run -it -p 808[0-9]:80 sfu-videochat:[your_team_name]
   ```
   
6. Access `https://hack0[1-9].hiconyan.com/808[0-9]/` on browser

## Reference

* [SkyWay - Enterprise Cloud WebRTC Platform](https://webrtc.ecl.ntt.com/)
* [skyway/skyway-js-sdk: JavaScript SDK for SkyWay](https://github.com/skyway/skyway-js-sdk)
