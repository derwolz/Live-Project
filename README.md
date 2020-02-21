# Live-Project
This was code used to help build Theatre Vertigo's website, that I had written.
The First part I worked on was creating a user friendly environment that displayed what plays are playing, their showing duration, the time of those showings, and the link to get a ticket.
![Bootstrapcode](https://user-images.githubusercontent.com/32439939/75077746-e2939c00-54c0-11ea-97b4-0dd553083e78.png)

My second task was to Pass a dropdown menu to the view, pass the result back to the controller, use that result in the process to create a database entry. Then in the index view, tie the User name to a castmember name and display it in the list of all cast members.

![UserstoView](https://user-images.githubusercontent.com/32439939/75077749-e3c4c900-54c0-11ea-97d9-d12a11439d1c.png)
First I passed the list of all usernames with their corresponding Id's to the view through Viewdata

![getFromView](https://user-images.githubusercontent.com/32439939/75079084-c265dc00-54c4-11ea-8776-2cf6d997149d.png)
Once I had created a procedure to pass information to the view I needed a way to get the response from the user. This method grabs the users input from the dropdown menu from "dbUsers" and passes that to userid, resets "dbUsers" data and using userid, finds the id of the user and replaces the empty database entry with its Id.

![ViewDropdown](https://user-images.githubusercontent.com/32439939/75077751-e3c4c900-54c0-11ea-83cc-579dae9e8c77.png)
All that was left was to implement the methods involved into the view.

![Dropdowntoview](https://user-images.githubusercontent.com/32439939/75077747-e32c3280-54c0-11ea-9031-049247e242a2.png)
The second part of this was to Have a method that passed Usernames for display, and their Id's that were assigned to the castmember database. I accomplished this through a Dictionary pairing passed to a Viewbag.

![ViewChange](https://user-images.githubusercontent.com/32439939/75077750-e3c4c900-54c0-11ea-93cf-48c5a015f952.png)
Using iteration, I find the id associated with each castmember and use that to display the Username through the value of the keyvalue pair.
