# citrix-capstone

## Resources
Issue tracker: https://waffle.io/peterwerner/citrix-capstone

Firebase Database: https://console.firebase.google.com/project/citrix-capstone-2016/database/data


## client-app/
Contains: style sheets, images, components, layouts, and utilities.

### public/
Contains css files and images used by the app.

### src/components
These are the building blocks of the app that render the ui.
Contains some logic to interact with the front and back end.

### src/layouts
Contains: base layout for the app and layouts for each page.
Layouts are composed of multiple React components.

### src/utilities
Contains the bulk of the logic.

- firebase.js & firebase2.js: Interacts with firebase database, including writers/readers, and listeners. Also contains firebase authentication.

- firechat.js: Contains logic implementing firechat, our text chat and session rooms that are used by the app.

- peerVideo.js: Contains logic for setting up peer to peer connections. Communicates with the server to do so.

- filecache.js:  Caches files in memory and listens to changes, updates components accordingly.

- googlePicker.js & googleapi.js & metadata.js:  Interacts with GoogleAPIs used by the application.

- search.js: Implements logic behind searching for files. 

### src/index.js
Entry point to the application, routes to specific pages.

## server-app/

### server.js
Server side of peer to peer connections.
