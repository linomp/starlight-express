# Developing APIs with Python

Stripped down path to teach you what are APIs, how to build one quick with FastAPI (that also follows modern best practices), and how to build an interesting project at the end.

## Git & Github

To upload your project to github correctly you NEED to know this. Please watch  (in order): 

1. **[Learn Git in 15 minutes](https://www.youtube.com/watch?v=USjZcfj8yxE)** 

2. **[Learn Github in 20 minutes](https://www.youtube.com/watch?v=nhNq2kIvi9s)**

Checklist after watching those videos:

- [ ] have a github account
- [ ] know how to create a repository on github
- [ ] know how to push your git repo to github
- [ ] know the benefit of working on branches separate from the main branch
- [ ] know how to create & delete secondary branches in your git repo
- [ ] know how to merge secondary branches into the main one


## The Path

**1. [Tutorial about APIs & FastAPI framework (58 min.)](https://www.youtube.com/watch?v=-ykeT6kk4bk&t=731s)** - TechWithTim makes the best python videos.
  
   <img src="https://user-images.githubusercontent.com/40581019/175874893-8332d135-3306-490c-b6bd-671876d33d13.png" width="45%" />

**2. [Build amazon price tracking app (19 min.)](https://www.youtube.com/watch?v=Bg9r_yLk7VY)**  - you don't build a web app, but contains all the steps for scraping AND sending you an email when the price is below a chosen threshold. 
  
   <img src="https://user-images.githubusercontent.com/40581019/175885423-704dfb3f-8d79-4704-bc1a-ccbb6cbcbcdb.PNG" width="45%" />

**3. Project Idea:** Use the knowledge from steps 1 & 2 to build an API with these endpoints:
  - POST `/tracking`: here I can send the url of a new product that I want to track and a price "threshold" for sending me an alert.
  - GET `/tracking`: returns me a list with the currently tracked product urls, along with product name, price threshold and best price so far.
  - GET `/config`: show me the email to which the alerts will be sent
    
    Notes: 
    - First focus only the API (the backend). Later you can investigate how to add an actual UI / web page (the frontend).
    - also, the script created in step 2 runs only once. For monitoring the price automatically you will need to run it as a **Scheduled Task**, but it's easy. This [answered stack overflow question](https://stackoverflow.com/questions/70104983/how-to-use-apscheduler-correctly-in-fastapi) shows how to do that (within FastAPI).

## Further resources

#### More about Web Scraping
- [TechWithTim: Web scraping with BeautifulSoup](https://www.youtube.com/playlist?list=PLzMcBGfZo4-lSq2IDrA6vpZEV92AmQfJK). 4 videos, from 11 to 27 mins. each.

  <img src="https://user-images.githubusercontent.com/40581019/175874933-a4f6a3d8-bfbb-4a15-ad80-394c039f57fb.PNG" width="35%" />
  
- Web scraping Memes from Reddit with FastAPI: [part 1 (48 min)](https://www.youtube.com/watch?v=di13K2xTedo&list=PLhH3UpV2flryU3DDc47zAbiyDdbIFnnNB&index=4) | [part 2 (30 min)](https://www.youtube.com/watch?v=0cVybZ_loWw&list=PLhH3UpV2flryU3DDc47zAbiyDdbIFnnNB&index=5). 

  <img src="https://user-images.githubusercontent.com/40581019/175878832-ea9dab71-e0d8-4b08-b6d4-0d1c68b8ac66.PNG" width="35%"/>


#### More about Web Applications
- [Fullstack development tutorial (1h)](https://www.youtube.com/watch?v=OzUzrs8uJl8). Learn to connect FastAPI (backend), ReactJS (frontend) and MongoDB (database) by building a To-Do list app.
  
- [Learn HTML & CSS building a portfolio website (2h)](https://youtu.be/r_hYR53r61M). Responsive layout, browser local storage (chosen theme persists after page refresh).
 
  <img src="https://user-images.githubusercontent.com/40581019/133420469-aa1fb07e-2ff7-4eed-8047-e3702c3dc316.PNG" width="35%" />
