# gliders
The front page / home page for IOOS National Glider DAC

Please do not file issues here,  all GliderDAC related issues should be filed in the [IOOS National Glider Data Assembly Center (V2)](OOS National Glider Data Assembly Center (V2)) repository.


# Installation

1. Download and install nodeJS (should come with npm)
2. Install bower
   
   ```
   npm install -g bower
   ```

   _You may need to run as sudo_

3. Install grunt

   ```
   npm install -g grunt-cli
   ```

4. Use node to build the project dependencies

   ```
   npm install
   ```

5. Use bower to install the UI depencies

   ```
   bower install
   ```

6. Run the project

    ```
    bin/www
    ```
7. Accessing via localhost in browser:(Use data subdirectory)
  ```
    http://localhost:3003/data
  ```
Replace 3003 with your configured port.

# Developing

## Deployed files:
gliders.ioos.us is the wordpress site
gliders.ioos.us/data is this repo.

Most of this project are static files. The initial pages are loaded as jade
templates.  

# Update the .env file with config variables
For testing Google Analytics and things that use env variables.
Update the .env file in your root folder similar to this:
```
GOOGLE_ANALYTICS_ID=YOUR_ENV_VAR_HERE
```