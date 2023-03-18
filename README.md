# CS4249 Logging Prototype

The application in its current state is tied to an existing Google Forms document; its responses can be found in the Google Sheets document [here](https://docs.google.com/spreadsheets/d/1DhLaS2c8utK9C8VvhQma5H18NzBLq1Pd7sjwe62z8VE/edit?usp=sharing). To customise the setup to your own Google Forms document, follow the instructions as provided in `googlesender.py`.

## Development

Host the web application on your local network using the [HTTP servers Python module](https://docs.python.org/3/library/http.server.html). The steps for setting up your development environment are as follows:

```bash
# clone repository
git clone https://github.com/petermonky/cs4249-logging-prototype.git

# navigate inside project folder
cd cs4249-logging-prototype

# get host device's IP address
ipconfig getifaddr en0

# host web application on local network
python3 -m http.server 8000
```

The application can then be accessed by any other devices on the same local network by navigating to `http://<host device IP>:8080`.

## Production

To host the application online, one may look into free hosting providers like [Netlify](https://www.netlify.com/).
