
# Sauce Control

Trying out Jasonette with the goal of building an app for managing github/gitlab.

### Steps followed

- Create repo 
- add `./src/main.json`
- `npm run dev`

Jasonette:

- Downloaded: https://github.com/Jasonette/JASONETTE-iOS/archive/master.zip
- Extracted it to `./ios`
- cd into folder, run `./Setup` and point it to `localhost:8080/main.json` (Raw github file in production)
- After XCode opens hit play to open Simulator


### Development

Make any changes you want to the json in `./src`, then on the simulator close and reopen the app to see changes.

Problem so far is that the JSON doesn't seem to refresh. I don't even think the app is requesting it again, it seems to be cached (because I don't see a logged request on the http-server). This may be just because of Simulator?