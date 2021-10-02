
# TryHackMe OhSint Walkthrough
---------------------------------------------------------------
First of all, we need to download the task file

So What information can you possible get with just one photo?..
We have many tools to get informations from a picture, i'll use [exiftool](https://www.poftut.com/how-to-install-and-use-exiftool-in-linux-windows-kali-ubuntu-mint-with-examples/) command line tool in kali.

![2exiftool](https://user-images.githubusercontent.com/90579213/135710471-c54aba83-b39c-481f-bbc5-882a43879f22.JPG)

mmm that copyright name interests me!
lets make some google DORKING !

![dorking](https://user-images.githubusercontent.com/90579213/135710632-cdda408e-e795-4c10-a43e-bf38b9be27d4.JPG)

As we see OWoodflint has a **twitter,github** accounts and a **wordpress** blog.
All flags will be found using these 3 search results.


soo let's dive in to the questions :

  ### 1)What is this users avatar of?
  
  ![q1](https://user-images.githubusercontent.com/90579213/135710800-07d15c4e-c60b-4204-bee9-fa64c5548f12.JPG)

  #### Answer(twitter): cat
  
  ### 2)What city is this person in?
  
  see this tweet 
  
  ![q2bssid](https://user-images.githubusercontent.com/90579213/135711010-38eb2ce1-7a49-4d5d-bf39-477e2ff46a2d.JPG)
  
  from the BSSID(found on the tweet) and a simple search using www.wigle.net we can answer this question:

  ![wigle1](https://user-images.githubusercontent.com/90579213/135711109-340a50e7-0a5b-4286-b93d-825bb78223b3.JPG)
  ![wigle2](https://user-images.githubusercontent.com/90579213/135711161-64ec935c-0f51-424f-bb8c-28a2322356aa.JPG)

  If you zoom out in the map you’ll be able to see a purple point on London, and Yay, thats the answer !
  
  #### Answer:London

  ### 3)Whats the SSID of the WAP he connected to?
  we need to zoom on to this location and we'll find the ssid
  
  ![ssid](https://user-images.githubusercontent.com/90579213/135711428-6b3c0120-7da1-4149-aa6a-64cf65d6cce5.JPG)
  
  #### Answer:unileverwifi
  
  ### 4)What is his personal email address?
  
  #### Answer:OWoodflint@gmail.com
  
  ### 5)What site did you find his email address on?
  
  #### Answer:github.com
  
  ### 6)Where has he gone on holiday?
  let's visit his wp blog:
  
  ![s2](https://user-images.githubusercontent.com/90579213/135711558-649a4e8a-e887-4646-8239-7af61fd4558f.JPG)

  #### Answer: New York
  
  ### 7)What is this persons password?
  Omg that was the hardest one in this room,
  let's view the page source
  
  ![password](https://user-images.githubusercontent.com/90579213/135711826-cbe8e472-4eb7-40b5-a7d8-661d6d4e99b6.JPG)
  
  and finally we found it "pennYDr0pper.!"
  
  #### Answer:pennYDr0pper.!
  
  
  After completing this room u'll gett a badge

![image](https://user-images.githubusercontent.com/90579213/135711926-58e59907-ea87-41f3-b39a-2357c3a0014c.png)

  
  

