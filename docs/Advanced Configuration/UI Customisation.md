---
sidebar_position: 1
---
# UI Customisation

Stirling PDF allows straightforward customisation of the application name to make Stirling-PDF your own using environment variables `APP_HOME_NAME`, `APP_HOME_DESCRIPTION`, and `APP_NAVBAR_NAME` with Docker or Java. 


### Local 
If running Java directly, you can also pass these as properties using `-D` arguments such as:
```
java -jar Stirling-PDF.jar -DAPP_HOME_NAME="New Application Name"
```

Alternatively you can set these via environment variables to be read by running 
```
export APP_HOME_NAME="Stirling PDF"
```

### Docker
If in docker you can do it via docker run or compose whichever you are using are part of installation.
Simply add these to the end of your script/file
#### Docker run
```
-e APP_HOME_NAME=Stirling PDF \
-e APP_HOME_DESCRIPTION=Your locally hosted one-stop-shop for all your PDF needs. \
-e APP_NAVBAR_NAME=Stirling PDF \
```
#### Docker Compose

```
    environment:
      APP_HOME_NAME: Stirling PDF
      APP_HOME_DESCRIPTION: Your locally hosted one-stop-shop for all your PDF needs.
      APP_NAVBAR_NAME: Stirling PDF
```
