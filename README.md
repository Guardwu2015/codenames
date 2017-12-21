# codenames

> Realtime webapp implementation of the classic social word game, Codenames, designed to be played on a TV and mobile devices. Based on a project by [sprek](https://github.com/sprek).

### Blog Series

To read more about how this project came to fruition and how to build an app using the same technologies, follow the links below!

* __Part 1__ - [Introduction and Planning](https://secdevops.ai/weekend-project-part-1-creating-a-real-time-web-based-application-using-flask-vue-and-socket-b71c73f37df7)
* __Part 2__ - [Enabling Websockets in Flask using Flask-SocketIO](https://secdevops.ai/weekend-project-part-2-turning-flask-into-a-real-time-websocket-server-using-flask-socketio-ab6b45f1d896)
* __Part 3__ (_In Progress_) - Using Websockets with Vue.js and Vuex

For content related to development, security, devops, AI, etc... check out [SecDevOps.AI](https://secdevops.ai)!

<p>
  <img src="screenshots/player-full.png" alt="Large Player View">
  <img src="screenshots/player-mobile.png" alt="Player - mobile" width="49%">
  <img src="screenshots/spymaster-mobile.png" alt="Spymaster - mobile" width="49%">
</p>

## Rules
Rules for codenames can be found [here](https://en.wikipedia.org/wiki/Codenames_(board_game)#Rules).

## Development
The app uses flask as its back-end and webpack as a front-end dev server.

### Flask Server
```bash
# optional: use a virtualenv
virtualenv venv
source venv/bin/activate

# install python dependencies
pip install -r requirements.txt

# run the flask server
npm run flask
```

### Webpack
```bash
# install dependencies
npm install

# run webpack dev server with hot reload at localhost:8080
npm run dev
```

## Production
### Build
``` bash
# install dependencies
npm install
pip install -r requirements.txt

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report

# start the flask server
npm run flask
```

## TODO

* Adjust colors for flipped cards on Spymaster view
* Add a turn timer/turn tracker
* Streamline install and build
