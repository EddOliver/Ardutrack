# Ardutrack
Biometrics Monitoring platform for pre and post COVID-19 patients based on the Arduino MRK 1010.

DISCLAIMER: This application is used for demonstrative and illustrative purposes only and does not constitute an offering that has gone through regulatory review. It is not intended to serve as a medical application. There is no representation as to the accuracy of the output of this application and it is presented without warranty.

Introduction, inspiration and Problem
Let me show you two images. The first image is a car from the mid-1800. This other one is a tesla roadster 2020. You can see huge differences between those two. The mechanical and technological prowess that took place.

Now here are two other images separated by almost the same amount of time...

The first one is from the Spanish flu pandemic from 1918 and the other one is from last month during our current COVID19 pandemic.

And thus lies the main problem...

We are treating the COVID19 pandemic like all the other pandemics in the past, with social isolation and PPE. With all the advances in Biotech, nanotech, AI and other scientific disciplines this is quite a shame. The solutions we are employing are insufficient, in an age where we can get information about almost anything due to technology.

Digitalization in healthcare in Latin America (our region) and even in the developed world has fallen behind and we need to find solutions that can help both doctors and patients with their needs and a great tool to aid us in the fight against COVID19. IF we are going to erradicate or control COVID-19, social distancing and PPE is NOT enough, we need to acurately employ contact tracing.

Most of our focus will be on this aspect of the contest:

Flatten the curve in communities with preventive solutions
And for that we will develop a couple IoT devices to do Contact Tracing. A little on Contact Tracing: From Wikipedia: "In public health, contact tracing is the process of identification of persons who may have come into contact with an infected person ("contacts") and subsequent collection of further information about these contacts. By tracing the contacts of infected individuals, testing them for infection, treating the infected and tracing their contacts in turn, public health aims to reduce infections in the population. Diseases for which contact tracing is commonly performed for include tuberculosis, vaccine-preventable infections like measles, sexually transmitted infections (including HIV), blood-borne infections, some serious bacterial infections, and novel infections (e.g. SARS-CoV, H1N1, and COVID-19). The goals of contact tracing are:

To interrupt ongoing transmission and reduce the spread of an infection
To alert contacts to the possibility of infection and offer preventive counseling or prophylactic care
To offer diagnosis, counseling and treatment to already infected individuals
If the infection is treatable, to help prevent reinfection of the originally infected patient
To learn about the epidemiology of a disease in a particular population
Contact tracing has been a pillar of communicable disease control in public health for decades. The eradication of smallpox, for example, was achieved not by universal immunization, but by exhaustive contact tracing to find all infected persons."

And again, IF we are going to erradicate or control COVID-19, social distancing and PPE is NOT enough, we need to acurately employ contact tracing.

This Solution will try and give that a shot with existing technology.

Reading the SDGs profile on the UNDP page was quite discouraging:

Hopefully I wholeheartedly think that low cost solutions that can provide contact tracing like this one can be later adapted to other chronic and degenerative diseases like the ones related to CVD or Cardiovascular diseases which are the ones with the highest mortality among any cause. If we start with our current focus and then adapt these low-cost solutions we might be able to finally use our technological tools to aid many more peope than just the ones that can pay for healthcare and in time maybe promote the concept of preventive medicine that has been the rage all these years, but has never really taken off.

Solution
Our solution is a smart platform with patient centric risk-assessing IoT devices that will keep track of several variables such as temperature, steps, and heart rate, among others through a web application.

It includes a wearable band that we integrated with a set of sensors that can be embedded easily into clothing. It can be worn on the wrist, chest or as an armband.



Whenever the system detects an anomaly via heart rate temperature, movement or other it will send an alarm, notification and recommendations both to the user and the Doctor linked to the app. Here are some screenshots of the solution in our new webapp: iot.covital.com.mx

Check it out with the login: DrGregoryHouse@gmail.com and the PW: toor

If a Doctor logs in:

All this data will be shared with the user’s doctor or Medical carer in real time and provide invaluable insights in order to analyze and possibly stop the spread of COVID19 and will also serve as a basis after the pandemic to focus on other diseases such as Metabolic or chronic ones. If the patient logs in you'll see:

These kinds of measures have shown to decrease considerably the risk of contagion during the pandemic as shown by other smart health applications in countries like South Korea.

Viability
As we are using existing technology its scalability has already been proven as we just need to share the go to market strategy and business model of previous wearable companies.

From: https://3dinsider.com/wearable-statistics/#:~:text=According%20to%20a%20survey%20conducted,bands%20to%2025%20million%20units "From $29 million in sales in 2014, the sales of wearable devices have gone up to $172 million by 2018. By the end of 2018, an estimated 350 million wearable devices will have been in use worldwide. By the end of 2019, the global retail revenue from smart devices has reached $53.2 billion."

And this is perfect for a developing country such as the one we are from, which is Mexico. The country lacks the infrastructure to do high level contact tracing, but the low cost of these devices and the fact that most of the population is already using a wearable band and a phone makes it a good choice. And yes for the moment we are one of the most-at-risk regions:

Also, whenever countries go ahead and raise lockdowns their numbers will most likely go up as is the problem that we are having in Mexico. So a low cost, easy to use contact tracing solution like this one is probably one of the most viable solutions as you can detect quite a lot with just the heart rate and temperature.

Step by Step instructions
This will focus heavily on the Arduino MKR 1010 WiFi development.

The two most important variables in tracking symptoms are without a doubt Heart rate and temperature. And this will be the focus of the product.

As usual if you are new to Arduino go to the official resource:https://www.arduino.cc/en/Guide/MKRWiFi1010

Step 1: Heart Rate Monitor
For this one I'm going to improve on one of the modules of my past projects (just a single module) and link it to the Arduino MKR 1010. It is a heart rate and SpO2 monitor based on the MAX30100. These are two variables that are always important to know in a biomedical setting, and are quite useful.

First build the circuit:

This is quite easy once you get a hang of the MAX30100 module.

If you have the green RCWL-0530, MAX30100 module, I know your pain. But here is the best solution in the whole internet. Instead of desoldering the SMD resistors like some sources say, just set some 4.7k Ohm pull-up resistors for the SDA and SCL pins. Always use 5V for VCC and you are set.

For this project you will need these libraries installed in Arduino IDE:

PubSubClient: https://github.com/knolleary/pubsubclient
ArduinoJSON: https://github.com/bblanchon/ArduinoJson
Any MAX30100 library: not needed really but it has several examples.
Just go to the library manager at Programs->Include Library->Manager.

I have to say this, this was a considerable improvement over my other MCU's as the Arduino MKR WiFi 1010 adopted the MAX30100 library natively as it was written without me having to change any line.

If you need help setting up the Arduino MKR 1010 go to the official resource:

https://www.arduino.cc/en/Guide/MKRWiFi1010

If you have any more questions with this, I probably solved them in my other project: https://www.hackster.io/Edoliver/health-and-fitness-tracker-753695

The Arduino MRK 1010 code and some examples are as always in the project's Github and at the bottom. You can upload that sketch at this moment.

Here is my initial test:


Step 2: Temperature monitor
Now that we have shown that the heart rate sensor is compatible, lets add a Temperature Sensor:

Ill be using the DHT11 humidity and temperature sensor because that's what I had at hand, but i would recommend the BME280 which is much precise.

foto del DHT11

For this one you'll need the DHT11 sensor library by Adafruit, as usual go to the Library manager and download it.

https://github.com/adafruit/DHT-sensor-library

Now for this one you'll have to follow this circuit:

Now its time to upload the example provided at the bottom of this tutorial and run a test:


Step 3: Joining the sensors and MQTT setup
Now we will have to join both sensors and also use the Pubsub library to send the data to IBM cloud.

Let's integrate the sensors first, here is the circuit diagram you should follow. You can now download the last example code to have both sensors working.

What I'll be doing for the two sensors to work properly is adding a counter:

int x=20; // counter, the intention is to take 20 Heart beats for every 1 temp reading
With that incorporated into a loop with it becoming smaller I'll take 19 Heart rate reading per 1 of temperature. There are very small temperature variances in a person/ambient so it does not need to be performed at all times.

Let's do a test of it:


And add a battery!

This makes use of the full potential of the Arduino MRK 1010 and makes it a complete product:


Now for the last part, which is integration to IBM IoT. for that we have previously developed and amazing tutorial on how to connect any device to that platform and showcase everything into Node-RED, from there it is very simple to just call the API and upload it to your web application! (ours was shown at the start of the article):

https://www.hackster.io/Altaga/the-ultimate-ibm-watson-iot-platform-guide-eb6bfc

As usual the final code with everything provided is at the end of this documentation.

Step 4: 3D printed parts
For this particular device a proper case is in order. For this I tried to make it as small as possible, but also attractive to some degree. What I intend for this device is to be able to wear it whether it is on the wrist, arm of chest. So, I leave to the final user to implement the cord at own discretion.



Here are some money shots and how it fits with the solution:







With the straps and from the back:

Showcase:


Final Video Demo:

Final Commentary
We envision a future in which Healthcare is invisible and seamless, where you are getting the attention of experts but only engage if necessary. Using Machine learning and IoT to monitor symptoms to a condition with every process improving so it becomes error-free. With emphasis on the preventive side and with the patient as the point of care, YOU become the point of care.

We don't have to repeat and do the same actions we used to do 200 years ago. We have a lot of new technology and in this case COVID-19 is becoming the exception.

With our solution we will be creating big data with previously wasted information in order to provide better healthcare services and improve on the patient-doctor relation. With this MPs can attend many more patients simultaneously and with better and improved care.

References:

https://www.who.int/csr/disease/ebola/training/contact-tracing/en/

https://www.theverge.com/2020/3/5/21166088/coronavirus-covid-19-protection-doctors-nurses-health-workers-risk

https://weather.com/health/cold-flu/news/2020-01-09-17-things-you-probably-didnt-know-about-the-flu

Elert, E. 2013. FYI: Why is There a Winter Flu Season? Popular Science. http://www.popsci.com/science/article/2013-01/fyi-why-winter-flu-season [2 November, 2014]

https://www.nih.gov/news-events/nih-research-matters/flu-virus-fortified-colder-weather

http://sitn.hms.harvard.edu/flash/2014/the-reason-for-the-season-why-flu-strikes-in-winter/

https://medicalfuturist.com/ten-ways-technology-changing-healthcare/?utm_source=The%20Medical%20Futurist%20Newsletter&utm_campaign=ee5854702c-EMAIL_CAMPAIGN_2019_10_29_diabetes_companies_COPY_&utm_medium=email&utm_term=0_efd6a3cd08-ee5854702c-420575081


