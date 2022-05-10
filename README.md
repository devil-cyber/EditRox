<<<<<<< HEAD
# EditRox (In Development) 
## Abstract
**EditRox is a pair coding platform, that provides feature to intract with  peers and code at the same time with high quality video and audio calling feature and real time code update feature. You get a feature to compile & run the program. The video calling is supported by WebRTC that provides low latency and also a industry standered. The video call is end to end encrypted, so no need to worry about the security. This app can handle upto 20 participant in a single room and can be scaled upto 100 participant depending upon the business needs. Its infrastructure is equiped with load balancer and reverse proxy that take care of the app at the time of peak load and load scarcity. This web application is lossely coupled and communicate via aws SQS(Simple Queue Service). The most exciting features of this web aplication are listed below:**
- The project is open source and anybody can make changes according to their requirments.
- There is not any rate limit and time limit over time.
- After end of metting this application does not store your data.
- This application is end to end encrypted.
- It provides HD video + audio calling.
- A compiler to run your code.
- Various Language and editor theme support.

## Introduction
After the spread of covid most of the it industry are going for remote work, the metting and code discussion are handled over online metting, but problem with most of these platform does not provide a way to share and edit their code in real time and the application that contains these feature are either paid or need high bandwitdh. These problem lead to the devlopment of EditRox, A realtime code editing web app that is equiped with video + audio calling feature.

## Design
`The architecture of Application:`

![](/asset/arch.png)

The application is divided into three parts:
- Client Side / Frontend
- Video + Audio  Server
- Compiler Server
- These three parts communicate to each other via SQS (Amazon Simple Queue Service).
- The compiler API and video server is equiped with nginx that act as load balancer and reverse proxy.
- The realtime commication is handled by WebRTC (peer to peer connection)

## Tech Stack Used
- Backend
    - `Node.js`
    - `Socket.io (WebRTC for real time communication)`
    - `SQS ( Simple Queue Service) ( For communication with other component of application)`
    - `AWS + Heroku (Cloud Provider for hosting Application)`
    - `Nginx (As load balancer & reverse proxy)`
    - `Docker container`

- Frontend
    - `React.js`
    - `Javascript`
    - `CSS`
    - `Socket.io (For handling client side communication )`
    - `Netlify (For Deployment)`
## Glimpse of WebApp

![](/asset/01.png)

![](/asset/02.png)

![](/asset/03.png)

![](/asset/04.png)

## Unique Feature:
- Project is open source anybody can change according to their business need.
- This application is free of cost.
- There is not any rate limit and time limit.
- It provide support for different programing language.
- It also provide diffrent editor theme and fontsize for coding.
- It contains a compiler to run the program.
- It also provides video calling feature.
- It contains feature to mute, unmute and close thier video.
- Yours peers can also edit your code and help in debuging in realtime.

## Future Work:
- We are working on a better UI.
- We will add an authentication system, if you want to create a room of people <= 10 then there is no need of authentication but after >10 authentication will be needed.
- Authentication system will also caontins a Admin prevliged feature.
- We will also provide a feature to save your code and sync yours previous code.
- We will also add a screen share feature.

## Conclusion:
After testing this application with various people, we got some posetive feedback and the application profrmace was also great durin the testing phase. There are some smaller bugs and we are yet woring on that. But overall we think that its a great start and in near feature we also launc a better version of this application with better UI and more features. We will also require some expert feedback and thier support along the way.

[Click For Demo](https://editrox.netlify.app/#/f1b78005-79db-4d09-80c5-d80e87be1ff9)


