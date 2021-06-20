I just wrapped a [project](https://jkclem.github.io/nhl-api-vignette/) ([github repo](https://github.com/jkclem/nhl-api-vignette)) that gives an example of how to write functions to intearct with an API. I used the NHL's API to write the vignette. 

## The Project

In addition to writing a few functions to interact with a few of the API's endpoints, I explored some of the data available. I found some things that would surprise no one, like shooting percentage and shots per game are positive correlated with win percentage. I found some surprising things, like penalty minutes per game appears to have a quadratic relationship with win percentage.

## Reflections

Working on this project, I went through the normal development process. I coded up functions, tested them against known edge cases, and verified the output looked as expected. Then I went through the data exploration process to find and visualize relationships in the data. Overall, it was a pretty comfortable endeavor, except for one thing.

I've interacted with APIs before, but one problem that I hadn't encountered was different Ids for an entity depending on the endpoint. The NHL has a [records](https://gitlab.com/dword4/nhlapi/-/blob/master/records-api.md) and a [stats](https://gitlab.com/dword4/nhlapi/-/blob/master/stats-api.md) API. Depending on which API is being called, the correct Id to use changes. 

I wasn't sure to design the functions to expect a **franchise Id** or a **team Id** because I could not decide what a user would want as a default. My workaround was letting a user supply a full team name (e.g. `"New York Rangers"`) to a function and let the function map it to the appropriate Id number. If a user wanted to pass an Id, I expect them to provide the proper Id given the API whose endpoint the function is querying. I'm still not sure that this was the right choice. Were I to build a production-ready API interaction package, I would want to poll likely users to know their preference. I don't know the feasibility of that, but I feel like it is a huge design decision to make without outside input.

I'm interested to dig into some code for widely used API interfacing packages to see how other people have approached this issue. 
