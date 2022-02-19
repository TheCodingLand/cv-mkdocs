# Some of the projects I worked on

=== "Professionnally"
    ## **Tina ML** 
    !!! quote "*A Complete machine learning platform used to build, track and serve AI models*"

    ???+ Note "Details"
        === "Context"

            ???+ info "Context"
                Ctg was looking for a tool to integrate machine learning to several business processes. <BR/>
                The platform anwsered all those requirements, and was based on some previous work I had done in AI. <BR/>
                I wrote the whole platform by myself including all Machine learning models code, frontend, backend and integrations.<BR/>
                The solution was deployed to Docker swarm then migrated to Kubernetes.
                

        === "Main Libraries Used"

            ???+ tip "Main libraries used" 
                * [X] `Django`
                * [X] `Pandas`
                * [X] `numpy`
                * [X] `pytorch`
                * [X] `tensorflow`
                * [X] `Huggingface transformers`
                * [X] `Catboost`
                * [X] `Xgboost`
                * [X] `redispy`

        === "Tech Stack"

            ???+ warning "Tech stack"
                * Docker
                * Kubernetes
                * Redis
                * mongodb
                * PostgreSql
                * ReactJs
    
    ## **Liquibase and Delphix Python** 

    !!! quote "*Database Migrations, Virtualization and Anonimization wrapper library for Delphix and Liquibase*"

    ???- tip "Main libraries used"
        * [X] `pydantic`
        * [X] `FastApi`
        * [X] `jpype0` - A way to run java components within python code

    ## **EIBS Move**

    !!! quote "*Release management system for banking software*"

    ???- tip "Main libraries used"
        * [X] `pydantic`
        * [X] `sqlalchemy`
        * [X] `SQLModel`
        * [X] `paramiko` - ssh library
        * [X] `pandas`

    ## **LBR File**

    !!! quote "*Self service - Free document optimization service and application for Luxembourg businesses document filling to the Luxembourg business register*"

    ???- Note "Details"

        === "Context"
            ???+ Info "Context"
                A lot of businesses had trouble filling documents for the administration. <br/>
                <br/>
                I wrote a service that opitimized documents and compressed them in compliance with the technical restrictions imposed by the CTIE, the IT department of Luxembourg.
                <br/><br/>
                Some algorithms were used to ensure that the compression did not render any of the character unreadable as this would be a serious liability issue.<br/><br/>
                This was provided for free for a few years until the LBR lowered the restrictions for document filing.
                An early version of the code is still on my github.<br/><br/>
                This was hosted on Google Cloud Engine.

        === "Main Libraries Used"
            ???+ tip "Main libraries used"
                * [X] `Imagemagick`
                * [X] `opencv`
                * [X] `tesseract-ocr`
                * [X] `redis-py`
                * [X] `asyncio`

        === "Tech stack"
            ???+ warning "Tech stack"
                * Docker
                * Kubernetes (Google cloud engine)
                * Redis
                * PostgreSql
                * ReactJs
                * Websockets


    ## **Call tracking**

    !!! quote "*application for IT helpdesk services call tracking and ticket efficient handliung of calls and statistics*"

    ???- Note "Details"


        === "Context"
            ???+ Info "Context"
                The tool used for tracking incoming was slow and a bit lacking in terms of usability. <br/>
                <br/>
                I first wrote an app with PHP and jquery, that was better in every way, from user interface to statistics output.
                <br/><br/>
                Then I wrote a complete log parser for the phone central to link my app to it, allowing complete interactivity with the web UI and incoming calls.
                I ended up rewriting it all in Python and React, using mobx for state management, and in a microservice architecture style, with an event queue management system.
                <BR/>
                This was my first experience with microservices, around 2016.

        === "Main libraries used"
            ???+ tip "Main libraries used"
                * [X] `Django`
                * [X] `redis-py`
                * [X] `React`
                * [X] `PHP`
                * [X] `jquery`

        === "Tech Stack"
            ???+ warning "Tech stack"
                * Docker / internal Docker swarm cluster
                * Redis
                * PostgreSql




=== "Personally"
   

    ## **SHAD Trading Bot**

    !!! quote "*Real time crypto portfolio management*"

    ???- Note "Details"

        === "Context"

            ???+ Info "Context"
                Noticing how market patterns  in crypto can be repeating and cascading, I had an idea to write a bot to detect such market tendencies and profit from them. <BR/>
                It uses a Sell Half At Double basic strategy for positions, in this stategy, there are no exits and no stop-loss.<BR/>
                <BR/>
                Entries are decided by a reinforcement learning model trained on a custom OpenAi Gym environment.<BR/>
                Training data and live trading data is extracted using several workers, from various Exchange APIs, at a 1m, and 1h time intervals. <BR/>
                I ended up using only 1h data for this strategy.
                <BR/>   
                The bot performed between +151% better than buy and hold strategies in 2020, and 208% better in 2021<BR/>
                I have also built a web platform that allows me to track each positions, taken by me or the bot, and monitor profits.<BR/>
                It is compatible with 3 different exchanges. (using a simple strategy design pattern) </BR>
                Everything is configurable from a django admin page.<BR>
                I will not release this code yet, as there is a chance that I release this as a paid service in the near future.

        === "Main libraries used"

            ???+ tip "Main libraries used"
                * [X] `OpenAI Gym`
                * [X] `Django`
                * [X] `pytorch`
                * [X] `backtester`
                * [X] `python-binance`
                * [X] `huobi_python`
                * [X] `coinbase`

        === "Tech Stack"
            ???+ warning "Tech stack"
                * Kubernetes
              



    ## **Rloop**

    !!! quote "*Hyperloop pod design competition for SpaceX*"

    ???- Note "Details"

        === "Context"

            ???+ Info "Context"
                I entered one of the first competition instances, we had built a team online from members of a reddit channel.
                My role was to implement a way to share Engineering results within the team.
                For this I've built a unified development environment where the results were automatically shared accros team members.
                This also helped with the technical setup, and experiment reproductibility.

        === "Tech Stack"
            ???+ warning "Tech stack"
                * Docker
                * AWS

    ## **AP-HP**

    !!! quote "*Volunteering for Paris hospitals During the Covid-19 pandemic*"

    ???- Note "Details"
        === "Context"
            ???+ Info "Context"
                During the pandemic, there was a call for machine learning engineers to help with some unprecented issues.<br/><br/>
                One of the issues I worked on with a team was arount medical supplies management using patient flow prediction.

        === "Main libraries used"
            ???+ tip "Main libraries used"
                * [X] `Django`
                * [X] `redis-py`
                * [X] `plotly`

    ## **Ctg Champions**

    !!! quote "*Friendly Internal Challenge betting on football matches, international competitions*"

    ???- Note "Details"


        === "Main libraries used"
            * [X] Application written in Dart/Flutter
            * [X] FastApi
            * [X] SqlAlchemy
        
        === "Flutter App preview"
            ![](https://github.com/TheCodingLand/Ctg-Champions/blob/master/mobile-app/champions/Q77WaGyYga.gif?raw=true)    
            


And more, just ask me, or have a look at the new [Automation](../automation.md) Project
