# SkyWay video chat example

## Getting started

1. Clone sample apps

   ``` shell
   $ git clone https://github.com/cloud-hackathon/skyway-apps.git
   ```

2. Move to `sfu-videochat` directory
3. Once you’ve given it a try, sign up for the free[Community Edition](https://console-webrtc-free.ecl.ntt.com/users/registration) and get an API Ke
4. Run application with the API key you got in step 3

   ``` shell
   $ export DOCKER_HOST=tcp://hack0[1-9].hiconyan.com:2375
   $ docker build -t sfu-videochat:[your_team_name] .
   $ docker run -it -p 808[0-9]:80 -e SKYWAY_KEY=<YOUR_API_KEY> sfu-videochat:[your_team_name]
   ```
   
5. Access `https://hack0[1-9].hiconyan.com/808[0-9]/` on browser

## Reference

* [SkyWay - Enterprise Cloud WebRTC Platform](https://webrtc.ecl.ntt.com/)
* [skyway/skyway-js-sdk: JavaScript SDK for SkyWay](https://github.com/skyway/skyway-js-sdk)
