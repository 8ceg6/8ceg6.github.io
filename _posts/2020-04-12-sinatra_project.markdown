---
layout: post
title:      "Sinatra Project"
date:       2020-04-12 14:09:51 +0000
permalink:  sinatra_project
---


For my Sinatra MVC project I decided to create an application for a photography club. Where a user would be able to add 1 or multiple cameras. Users can have multiple cameras so a `has_many` and `belongs_to` relationship was established.  A User's list of cameras is displayed as `li` with links to the specific camera. Users through the camera show page can update or delete a camera in which they own. 
Another feature a `User` has is the ability to post a link via an `a` tag  `<h6><a href="<%=@user.photos%>"> <%=@user.username.capitalize%>'s Photos</a></h6>`   that wil direct you  to an outside source that contains photographs the user has taken.  Users through the camera show page can update or delete a camera in which they own. this information can reviewd before it is completely updated by `redirect to` action that returns them to the same `edit` page before submission.  All edits and or deletions are protected by the use of `Helper methods` that prevent someone else from altering the information that has been given. I envision an expansion of this application to include a listing of gear and accessories owned by the user. Happy shooting and enjoy 
