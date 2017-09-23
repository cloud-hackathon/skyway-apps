# SkyWay video chat example

## Getting started

1. Clone sample apps

   ``` shell
   $ git clone https://github.com/cloud-hackathon/skyway-apps.git
   ```

2. Move to `sfu-videochat` directory
3. Once you've given it a try, sign up for the free [Community Edition](https://console-webrtc-free.ecl.ntt.com/users/registration) and get an API Key
    - Note that "権限(APIキー認証を利用する)" should be set to OFF. This parameter is for extra security.
4. Run application with the API key you got in step 3

### Run on localhost

1. Create `key.js` including the API key you got in step 3
  - `echo "window.__SKYWAY_KEY__ = '<Replace here the API key you got in step 3>';" > sfu-videochat/key.js`
2. Run web server
  - Mac:
    - `python3 -m http.server [ポート番号(デフォルトは8000)]`
    - `python -m SimpleHTTPServer [ポート番号(デフォルトは8000)]`
  - Win:
    - See: https://qiita.com/massie_g/items/2913066e596dae197539
3. Access `http://localhost:8000` on browser

### Run on Docker


   ``` shell
   $ export DOCKER_HOST=tcp://hack00[1-9].hiconyan.com:4750
   $ docker build -t sfu-videochat:[your_team_name] .
   $ docker run -it -p 808[0-9]:80 -e SKYWAY_KEY=<YOUR_API_KEY> sfu-videochat:[your_team_name]
   ```

1. Access `https://hack00[1-9].hiconyan.com/808[0-9]/` on browser

## Reference

* [SkyWay - Enterprise Cloud WebRTC Platform](https://webrtc.ecl.ntt.com/)
* [skyway/skyway-js-sdk: JavaScript SDK for SkyWay](https://github.com/skyway/skyway-js-sdk)
