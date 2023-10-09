## Project 2 Vignette Response Post

`An explanation on what you did in the project and any interesting findigs?`

In this project, I created a document that was a vignette on the `CollegeFootballData.com` (CFBD) API. I created functions to query, parse, and return well-structured data on various components of college football such as team stats, game results, coaching history, venue information, team composite rankings, and team records. I then utilized the functions to query the CFBD API at different endpoints for basic exploratory data analysis. The most interseting finding was that `Alabama` dominated in all of the performance metrics I looked at over the past 10 seasons. This includes average composite talent rankings, average margin of victory, and average passing touchdowns. Further, they have agreat coach in `Nick Saban`, who has the most wins among active head coaches. One intersting finding focused on `Alabama`, is that their home game attenance seems to be steadily declining over the past few years. Lastly, `Bristol Motor Speedway` can hold the most fans.

`a reflection on the process you went through for this project. Are there things you learned programming wise? What would you do differently in approaching a similar project in the future?`

The general process I went through, which was the most challenging, was findng the right API that met the demands of the project, and figuring out how to connect to it. I then explored the API itself, which had a great interface, to see what kind of data was offered. Based on that, I narrowed down some of the more interesting topics and replicated the URLs in various functions in my r markdown file, that also cleaned the data and outputted into a usable format. I then started high level with the topics I wanted to explore and got more granular as each step revealed something new.
I learned a lot on how connect to APIs through R, especially regarding the `httr2` package, how to make a few new plots with `ggplot2`, and how to use different `apply` functions. 
In the future, I would approach a project similar to this by having a better idea of the type of API I want to pull data from. I would also spend more time upfront understanding the different components that go into an API request and what to look for that separates good documenation versus poor documenation. I would also spend more time brainstorming what kinds of questions I wanted answered from the data that could tell a story, as opposed to quickly jumping in and trying to create a bunch of data sets.

* [Link to the rendered github pages site](https://chandlerells.github.io/ST558Project2/)

* [Link to the regular repo](https://github.com/chandlerells/ST558Project2)
