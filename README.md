# :bird: Tweeply (Powered by IBM Watson) ![](https://github.com/IpshitaC/tweeply/blob/master/assets/watson.gif)

### Table of Contents
1. [About](#about)
2. [How does it work?](#how-does-it-work)
3. [Technologies Used](technologies-used)
4. [Demo](#demo)
5. [Installation](#installation)
6. [Contributing](#contributing)
7. [License](#license)

## About
Tweeply is a cognitive Bluemix-based Web application that sends custom replies to all public tweets sent to a particular Twitter handle. This application is most suited for automated Twitter-based customer care services, election campaigns and almost anything interactive! In this version, Tweeply handles customer care queries and sends out suitable replies for the same.

This application was built during the #IBM include< geek.tech > Cognitive Computing Hack Camp held in New Delhi.

## How Does it Work?
Tweeply takes all public tweets made to a particular Twitter handle and analyzes them using the [IBM Watson Natural Language Classifier](https://www.ibm.com/watson/developercloud/nl-classifier.html) service. The service can be trained by the developer, according to the requirements of the application. The service yields confidence scores of various classes, out of which the class with the highest confidence score is said to be the classification of the text.

The application then chooses the predefined replies, as per the classification and tweets it to the handle, from which the request tweet was made, within a matter of seconds.

To read more about the IBM Watson Natural Language Classifier Service and its usage, please refer to the [documentation](https://www.ibm.com/watson/developercloud/doc/nl-classifier/).

## Technologies Used
* Node-RED
* JavaScript
* CSS3/HTML5
* IBM Watson Natural Language Classifier Service
* Twitter API
* Cloudant NoSQL DB

## Demo
Here's a demo of the query tweet and the reply tweet sent by the application.
@ipshi_chattons is the Twitter account for the bot and @ipshitachatterjee8 is the sample user account.
![Request Tweet](https://github.com/IpshitaC/tweeply/blob/master/assets/request_tweet.png)

![Reply Tweet](https://github.com/IpshitaC/tweeply/blob/master/assets/reply_tweet.png)

##Installation
1. [Clone or download](https://github.com/IpshitaC/tweeply.git) the repository
2. Update the credentials in [bluemix-settings.js](https://github.com/IpshitaC/tweeply/blob/master/bluemix-settings.js).
3. Run public/[index.html](https://github.com/IpshitaC/tweeply/blob/master/public/index.html)

## Contributing
See [CONTRIBUTING.md](https://github.com/IpshitaC/tweeply/blob/master/CONTRIBUTING.md) for more details. Or feel free to reach out to me via [mail](mailto:chatterjeei08@gmail.com).

##License
Tweeply is licensed under Apache 2.0 license. See [LICENSE](https://github.com/IpshitaC/tweeply/blob/master/LICENSE) for more details.
