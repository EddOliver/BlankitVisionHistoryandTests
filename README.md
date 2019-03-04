# Blankit Vision History and Tests

This repository has been created to showcase the history of development of Blankit's computer vision module, iteration and tests.

Created to provide a demo (or several) for Hax accelerator.

This repository has been created to showcase the history of development of Blankit's computer vision module, iteration and tests.

Created to provide a demo for Hax accelerator.

The first iteration of this module was born during AngelHack Mexico City: https://angelhack.com/portfolio-posts/angelhack-mexico-city-hackathon-2018-june-23-24-2018/. Which we won in the end with practically the same idea that would be refined at later dates.
That win gave us access to the entrepreneurial ecosystem in San Francisco, exposure an Incubation program and further acceleration down the line. http://blog.angelhack.com/meet-the-hackcelerators-2018-startups

That fist version was built on a Raspberry Pi 3, the programming logic was also simple, we saved every certain time a picture and sent it to a Vision recognition service provided by IBM (Visual Recognition). We fiddled with a model created by us in order to recognize the presence or absence of human faces. At this point it didn't matter if we didn't recognize anything else as we were just solving for the use case of absence.  

See: https://www.verywellhealth.com/choosing-to-leave-the-hospital-against-medical-advice-2614871
And: https://www.cms.gov/medicare/medicare-fee-for-service-payment/acuteinpatientpps/readmissions-reduction-program.html

This is quite a big problem is hospitals, it happens a lot (almost 40% in Mexico), patients abandoning their rooms and leaving, and patients with severe symptoms leaving their rooms. And it is quite difficult sometimes to detect this. That's why computer vision was an excellent choice. Reducing readmissions because of abandonement is a huge ROI for hospitals.

In addition to that once the model detects there are no faces it sends an alarm to our platform at which time was quite lean, it used MQTT to communicate that message, and once the information was on the webpage we could trigger any alarm we wanted to, on that step we just refreined to an email and a notification.

We actually don't have any photos of that working as most of the pictures of the hackathon and the pith were lost but it looked like this:
<img src= "https://www.raspberrypi.org/app/uploads/2017/05/Pi-Camera-attached-1-1390x1080.jpg">

And the camera was literally taped to a tripod, but for a hackathon it was an awesome PoC.

After that we improved much more the design and produced a demo as we were going thriough technical due diligence by AngelHack. Here it is (just click on the image): 

[![Vision Demo - MIA - Blankit](https://i.ibb.co/QQ985bK/1.png)](https://youtu.be/OX0gO1C_PAA)


Then we advanced through the two Incubators that we were on during that time, (AngelHack's Hackcelerator and Tec Lean Launch of our University: http://tecleanlaunchcdmx.strikingly.com/portafolio).

With that pressure we had to iterate into a much better design, and we improved on the algorithm.
Still a PoC but we went to a Retirement home to run a pilot on it, we cannot share much because we signed an NDA with the retirement home but here is a small demo of the whole system working (its quite bad I know but that is what we were allowed to share):

https://www.youtube.com/watch?v=WM3jetAzUF4  ------Victor .Ponlo para que des click en imagen

We learned quite a lot from this pilot including:
- The voice assistant works quite well, but not for patients who have hearing impairments, and in that population that is a huge percentage.
- The other devices worked quite well and were praised by both patients and providers alike. It seems that there is quite an opportunity market in that sector as they seldom have communication systems. Even in some hospitals.
- The vision module performed quite well whenever there was an incident but during the whole pilot that only happened three times. (Remember that the intent was to solve for hospitals mainly).
- There are several use cases that we can solve for in this instance and we might but for now it was a good first pilot overall as we tested several hypothesis we had and with every interview and test, it seemed as those hypothesis were being strengthened.

The next step was to finish those Incubators with two demo days, one in Mexico City and one in San Francisco during the: https://globaldemoday.io/

For that we streamlined everything and improved on our UX and UI:

-------Victor sube imagen del modulo de imagen y una de todos los modulos las buenas negras de san fran

And we produced this more professional video of the system:

-------------victor pon el video Bueno el mamado que hizo snapfilms como imagen aqui

With this came a period of going around several cities in the US and Mexico, participating in pitches and contests and we actually obtained victories in most of them.

Went to Johns Hopkins University to Medhacks, which is the world's premier Medical Hackathon and won the prize for Best IoT solution which was a spinoff on our voice assistant with a different use case:

https://devpost.com/software/amy-the-voice-of-medicine?utm_campaign=winner_email&utm_content=submission_won&utm_medium=tweet&utm_source=twitter

Participated in GlobalDemoDay with an excellent result (click on the image please):

[![Blankit at AngelHack’s Global Demo Day 2018](https://res-5.cloudinary.com/crunchbase-production/image/upload/c_lpad,h_256,w_256,f_auto,q_auto:eco/v1397750238/263f7da43e4360c0912997e3950e938e.jpg)](https://youtu.be/cTsb9BTLCpY)

And later we went to Monterrey Mexico to participate in INCmty Prize for health Entrepreneurship IBM - TecSalud, and yes we also won that one:
http://www.tecsalud.mx/es/listado-de-noticias/premian-lo-mejor-del-emprendimiento-en-salud-2018.aspx

And that is our biggest selling point, that last one gives us unlimited access to two of the biggest hospitals in Mexico, to run any test or pilot we want to make. In our case we are about to begin the first pilot in Monterrey at the end of March and first days of April to continue iterating and improving the product as we find many more use cases..

## Other use cases and further development

Since then we developed an aditional use case that is just being an IP camera able to send alerts to the central systems to use in Radiology.

1.- After patients have received contrast (which contains a radioactive isotope and is analog to glucose), they sometimes have very agressive reactions. The problem is that in that time the patient has to be secluded from everyone for a period of 2 to 3 hours before being scanned. And that is where our camera module comes in just as an IP camera capable of sending notifications. This use case was actually recommended by the main Biomedical Engineer of Ángeles Acoxpa which is one of the biggest hospital chains in Mexico city.

<img src= https://prd-medweb-cdn.s3.amazonaws.com/documents/radiology/images/PET-scanner.jpg>

2.- We have been improving on the algorithm and exploring several other technologies that use vision, and in the meantime generated several other demos:

We have been very busy with the maker and tech community so we were able to gain access to top of the line development boards and hardware. And for vision we developed in three fronts:

- Android Development using the OpenCV SDK and the Thundercom AI kit:
With this we developed a Two factor authentication to control access to maternity rooms. 
Demo:https://www.youtube.com/watch?v=bJGoDKyP2c4

More information on:https://www.hackster.io/126496/techcare-baby-safe-ad1936

And evidence that we have the AI kit: 
<img src="https://s3.amazonaws.com/stratupbootcampbucket/thunder.jpg">


- Python SDK libraries to use with drones:
Demo:  ------------victor tu video del dron

More information on: -----link de hackster victor

- FPGA development on the Ultra 96.
For this we deployed a solution for Industrial IoT, and we are exploring its capabilities for image recognition.
More info: https://www.hackster.io/114197/bbm-bridge-baby-monitor-for-predictive-maintainence-959fc6

In the meanwhile we have been experimenting with CV with the FPGA but we have yet to produce a Prototype.

Here is evidence of ownership:

-------------Pon las imagenes victor



And that's pretty much it, we have several prototypes that we will be willing to try at the hospital pilots this next month. We are eager to reduce our stack to a single refined Production candidate as we check on production costs, and the effectiveness of these options. And of course your input would be invaluable as most of the other parts of the design are mostly finished.

Thank you for reading, I know that this may be quite a lot but we are quite enthusiastic about the prospects of joining Hax and taking our technology and Statup to the next level.






