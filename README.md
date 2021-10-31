# Posture-Vision
## Inspiration

The Covid-19 pandemic has brought more people: students studying and professionals working from home.  Especially, children and teenagers are spending a lot of time seated at a desk or working with a computer because of excessive online learning. Spending hours in front of the computer is not only counter-productive for long hours of time, but it's extremely dangerous for one's health. Bad posture not only causes short-term discomfort but also has a long-term impact on the bones and muscles. It is the leading cause of Postural Dysfunction which is a long-term and painful disease, and Recently the number of students experiencing it has drastically increased. With the onset of the new semester the cases will rise up again that's why I came up with an idea to counter-tackle bad posture and avoid an unwanted disease before its too late

## What it does

PostureVision is an Open-CV/Machine learning-based app. PostureVision uses your webcam and monitors your posture in real-time in your browser, and sends notifications/alerts to you each time it detects poor posture. It also gives you real-time feedback about the quality of your posture and displays measurements for users that love detailed reports. PostureVision would be the best buddy to a student who is working a lot with computers/laptops and is careful about his health.

## How we built it

1. For the frontend I used HTML/CSS and React JS. I used the react-webcam package to send and show live webcam video feed to the ML model. I also used React Notifier package to make real-time notifications for browsers. I also used React JS in the backend and made a custom API to establish communication between the ML model and the backend which supports real-time image transfer

2. For building the Machine learning part I used Open CV and PoseNet A Tensorflow API. PoseNet allowed me to speed up the machine learning process. It provided a template on which I custom-coded some complex algorithms that enhance the detection power of the model. Then i exported it into TF js format after which I integrated the model into the backend. The Model has an accuracy of 94% and has comparably low latency and fast that makes it better than existing solutions

## Challenges we ran into

Initially, I was experimenting with a couple of models using TensorFlow (in Python), but it became too complicated (both on me as well as on the server) to handle and process data points in real-time between the frontend and the backend. I finally settled on using TensorFlow JS' PoseNet API to track data points in the browser, in real-time. I optimized it for maximum performance. Time limit was another problem. Going solo i had to do a lot of stuff by my own

## What I learned

I learned a ton of new stuff that we've never come across before. Things like tracking and calculating an object's position and orientation in 3D space with data inputs. I also learned about handling video streams with JavaScript in the browser. Perfected are React Skills and developed extensive knowledge of node packages. Working for the first time with PoseNet API was pretty hard, but learned a lot. 

## What's next for PostureVision

I'd like to have PostureVision deployed on a much larger scale. I'd initially have to work on more well-rounded features (such as real-time graphs) to monitor progress over a period of time and provide more comprehensive reports. Include a focus prediction by facial emotions and hosting the app online as a service
