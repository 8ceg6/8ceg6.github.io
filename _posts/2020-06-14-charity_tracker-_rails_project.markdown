---
layout: post
title:      "Charity Tracker- Rails Project"
date:       2020-06-14 23:11:59 +0000
permalink:  charity_tracker-_rails_project
---


For my rails project I chose to make a simple app that tracks the donations of a donor to charities. It consisted of three tables. To meet one of the requirements of the project I used the ` donations ` table as the join table to make the connection between the ` donors ` and ` charities ` tables. Applying the has_many_through Macro a donor(user) is able to select or create a charity to donate to. This was implemented by using a nested route. The format of the route is ` donors/:id/donations/new ` this approach made use of the join table through donations. After submitting a donation, the donor is ` redirected to ` the ` donors/:id/donations ` show page. On this page a view displays the charities of which they donated to and the amount. With the use of a ` scope query ` this view page also displays the total amount of money they have donated to charities. 
A particular portion of this project gave me a lot of problems and that was the ` omniauth ` login. My particular issue was that when a new donor would try to ` Sign up ` using this approach it would not save to the database. After (several hours)10 of trying different approaches on how I could find out why t would not save. I used a technique I saw in a study video. It is called ` raise (class name).errors.full_messages.inspect ` . Using this method gave me the information needed to figure out how to set up my variables. I was missing one of the ` params ` needed to make a successful callback and create the user. This method going to be a very essential tool, along with others, going forward when debugging is needed. I must add that nothing beats that satisfying feeling you get when overcome something that is very challenging. I still have a long walk on short path but I will make it successfully 

