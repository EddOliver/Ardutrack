# Ardutrack
Biometrics Monitoring platform for pre and post COVID-19 patients based on the Arduino MRK 1010.

<img src="https://hackster.imgix.net/uploads/attachments/1184794/_7hdoZbz8iH.blob?auto=compress%2Cformat&w=900&h=675&fit=min">

DISCLAIMER: This application is used for demonstrative and illustrative purposes only and does not constitute an offering that has gone through regulatory review. It is not intended to serve as a medical application. There is no representation as to the accuracy of the output of this application and it is presented without warranty.

Introduction, inspiration and Problem
Let me show you two images. The first image is a car from the mid-1800. This other one is a tesla roadster 2020. You can see huge differences between those two. The mechanical and technological prowess that took place.

<img src="https://hackster.imgix.net/uploads/attachments/1174859/image_JhGNDWJAP3.png?auto=compress%2Cformat&w=740&h=555&fit=max">

Now here are two other images separated by almost the same amount of time...

The first one is from the Spanish flu pandemic from 1918 and the other one is from last month during our current COVID19 pandemic.

<img src="https://i.ibb.co/ZXJJ2xF/covid.png">

And thus lies the main problem...

We are treating the COVID19 pandemic like all the other pandemics in the past, with social isolation and PPE. With all the advances in Biotech, nanotech, AI and other scientific disciplines this is quite a shame. The solutions we are employing are insufficient, in an age where we can get information about almost anything due to technology.

Digitalization in healthcare in Latin America (our region) and even in the developed world has fallen behind and we need to find solutions that can help both doctors and patients with their needs and a great tool to aid us in the fight against COVID19. IF we are going to erradicate or control COVID-19, social distancing and PPE is NOT enough, we need to acurately employ contact tracing.

Most of our focus will be on this aspect of the contest:

####Flatten the curve in communities with preventive solutions

And for that we will develop a couple IoT devices to do Contact Tracing. A little on Contact Tracing: From Wikipedia: "In public health, contact tracing is the process of identification of persons who may have come into contact with an infected person ("contacts") and subsequent collection of further information about these contacts. By tracing the contacts of infected individuals, testing them for infection, treating the infected and tracing their contacts in turn, public health aims to reduce infections in the population. Diseases for which contact tracing is commonly performed for include tuberculosis, vaccine-preventable infections like measles, sexually transmitted infections (including HIV), blood-borne infections, some serious bacterial infections, and novel infections (e.g. SARS-CoV, H1N1, and COVID-19). The goals of contact tracing are:

- To interrupt ongoing transmission and reduce the spread of an infection
- To alert contacts to the possibility of infection and offer preventive counseling or prophylactic care
- To offer diagnosis, counseling and treatment to already infected individuals
- If the infection is treatable, to help prevent reinfection of the originally infected patient
- To learn about the epidemiology of a disease in a particular population

<img src="https://hackster.imgix.net/uploads/attachments/1174860/image_Bj3hJCxKWd.png?auto=compress%2Cformat&w=740&h=555&fit=max">

Contact tracing has been a pillar of communicable disease control in public health for decades. The eradication of smallpox, for example, was achieved not by universal immunization, but by exhaustive contact tracing to find all infected persons."

And again, IF we are going to erradicate or control COVID-19, social distancing and PPE is NOT enough, we need to acurately employ contact tracing.

This Solution will try and give that a shot with existing technology.

Reading the SDGs profile on the UNDP page was quite discouraging:

<img src="https://hackster.imgix.net/uploads/attachments/1174861/_pddnT2ntMl.blob?auto=compress%2Cformat&w=740&h=555&fit=max">

Hopefully I wholeheartedly think that low cost solutions that can provide contact tracing like this one can be later adapted to other chronic and degenerative diseases like the ones related to CVD or Cardiovascular diseases which are the ones with the highest mortality among any cause. If we start with our current focus and then adapt these low-cost solutions we might be able to finally use our technological tools to aid many more peope than just the ones that can pay for healthcare and in time maybe promote the concept of preventive medicine that has been the rage all these years, but has never really taken off.

# Solution
Our solution is a smart platform with patient centric risk-assessing IoT devices that will keep track of several variables such as temperature, steps, and heart rate, among others through a web application.

<img src="">

It includes a wearable band that we integrated with a set of sensors that can be embedded easily into clothing. It can be worn on the wrist, chest or as an armband.

<img src="">
<img src="">

Whenever the system detects an anomaly via heart rate temperature, movement or other it will send an alarm, notification and recommendations both to the user and the Doctor linked to the app. Here are some screenshots of the solution in our new webapp: iot.covital.com.mx

Check it out with the login: DrGregoryHouse@gmail.com and the PW: toor

These kinds of measures have shown to decrease considerably the risk of contagion during the pandemic as shown by other smart health applications in countries like South Korea.

## Viability

As we are using existing technology its scalability has already been proven as we just need to share the go to market strategy and business model of previous wearable companies.

From: https://3dinsider.com/wearable-statistics/#:~:text=According%20to%20a%20survey%20conducted,bands%20to%2025%20million%20units "From $29 million in sales in 2014, the sales of wearable devices have gone up to $172 million by 2018. By the end of 2018, an estimated 350 million wearable devices will have been in use worldwide. By the end of 2019, the global retail revenue from smart devices has reached $53.2 billion."

<img src="">

And this is perfect for a developing country such as the one we are from, which is Mexico. The country lacks the infrastructure to do high level contact tracing, but the low cost of these devices and the fact that most of the population is already using a wearable band and a phone makes it a good choice. And yes for the moment we are one of the most-at-risk regions:

<img src="">

Also, whenever countries go ahead and raise lockdowns their numbers will most likely go up as is the problem that we are having in Mexico. So a low cost, easy to use contact tracing solution like this one is probably one of the most viable solutions as you can detect quite a lot with just the heart rate and temperature.

# Step by Step instructions

You can find them at the pryect hosted on Hackster: https://www.hackster.io/Edoliver/ardutrack-9a684f

# Final Commentary
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


