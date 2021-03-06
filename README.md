# microbit-webusb-serial-monitor
This project is an implementation of a simple serial monitor that utilises DAPjs to allow the use of the micro:bits WebUSB functionality.

## Feature Request and Issue Tracking
Please add an issue is you wish for any additional features or discover any issues using this project. Hopefully I'll learn from my mistakes!

## Local Server
This serial monitor was implemented with the intentions of understanding NodeJS and the WebUSB standard. That being said, running your own server will require an install of the latest version of NodeJS.

**Note: WebUSB is only available via a secure HTTPS connection or ``localhost`` for development.**

### Running
Once you have cloned this repo, head over to the ``bin`` folder where you will find a ``www`` file.

```
git clone https://github.com/Taylor-Woodcock/microbit-webusb-serial-monitor
cd microbit-webusb-serial-monitor\bin
node www
```

By default, this application is hosted on port 3000 at ``http://localhost:3000/``

### Node Modules (DAPjs)
At the moment, this repo has not been cleaned up and contains a load of potentially useless (for this project) node modules.
That being said, this project relies on the [DAPjs](https://github.com/ARMmbed/dapjs) JavaScript interface.

## Project Notes
As JavaScript isn't my goto language, and my knowledge of NodeJS was lacking, I decided to start with a simple, yet useful project to allow serial communication via the WebUSB standard.

I built this project using WebStorm's brilliant Node.JS Express App generator and utilised the features provided. With the division of business logic and views, modifying the look and feel of the page while maintaining the technical stuff was made very simple. The rendering is achieved via Jade and CSS located in the ``views`` and ``public\stylesheets`` folders, while the logic uses JavaScript found throughout the repo.

This project will later be expanded to work as a bridge between the BBC micro:bit and the internet; enabling internet connectivity to micro:bits via the onboard 2.4GHz radio.

## Repos
[DAPjs](https://github.com/ARMmbed/dapjs) JavaScript interface to CMSIS-DAP

## Code of Conduct
Not sure if I'm allowed/should put this... But I see it on a lot of micro:bit projects.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
