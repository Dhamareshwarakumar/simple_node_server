# <center>Simple NodeJS Server</center>

<br>

# Environment Setup (Debian Linux)

-   `sudo apt install npm`

<br>
<br>

# Download & Run Application

-   `git clone https://github.com/Dhamareshwarakumar/simple_node_server.git`
-   `cd simple_node_server`
-   `npm install`
-   `npm start`

<br>
<br>

# Design

-   `npm init`
-   `npm install express`

## server.js

```javascript
const express = require("express");
const app = express();

const PORT = process.env.PORT || 3000;

app.get("/", (req, res) => res.send(`<h1>Welcome to Node Dev Server</h1>`));

app.listen(PORT, () => console.log(`Server started on port ${PORT}`));
```
