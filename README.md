# Deploy API using Flask

We created a Flask server for communication with clients.
Response values to be sent to the client were generated from the YOLOv5 learning model and AWS S3.
<br>
<br>
### How to generate response data
On Raspberry Pi, we store photos, temperature, and humidity values of current Artechne in AWS S3 in jpg and json format.

Flask reads the json value stored in S3 and extracts the current temperature and humidity values of Artechne.

In Flask, the jpg stored in S3 extracts the current seat status information of the Artechne through the YOLOv5 learning model.

As a result, the Flask responds in json form with the temperature, humidity, the number of seats remaining, and the number of seats currently unavailable.
<br>
<br>
### This is a picture that was tested with a Postman.
---
![API_포스트맨](https://github.com/SmArtechne/smartechne-flask/assets/70840463/b07c0f55-37f5-40f3-857d-3cbac663a116)
<br>
<br>
### It is generating real-time seat status information through the YOLOv5 learning model.
---
![플라스크_욜로분석](https://github.com/SmArtechne/smartechne-flask/assets/70840463/a9471548-6156-4cf9-a96b-22cb03569cb6)


