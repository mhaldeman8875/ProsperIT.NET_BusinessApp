# Python Live Project - DataScrape

## Introduction
For the last three weeks of the C# course at The Tech Academy, I worked as a one-man-team developing an ASP .NET MVC Web Application. This web application allows for users to be registered to a database as 'employees' or 'admins'. Once a user is logged in, they are redirected to a clock in/clock out page. As an admin, the user can see details of all the users in the database, upload user images, etc.

Working on a legacy codebase was another great learning opportunity for adding/modifying features according to user stories, which I assisted in coming up with, as well as practicing the code-first approach to https://github.com/mhaldeman8875/ProsperIT.NET_BusinessApp.gitmodifying a pre-existing database. There were some particularly challenging tickets that were a large time sink, but with enough research I was able to overcome the obstacles and find ways to solve the issue. I worked primarily on [back end stories](#back-end-stories) however, I also worked on sever [front end stories](#front-end-stories) Over the two week sprint I also had the opportunity to share some of my knowledge regarding version control and virtual environments with the team project management and team programming [skills](#other-skills-learned) that I'm confident I will use again and again on future projects.
  
Below are descriptions of the stories I worked on, along with code snippets and navigation links. I also have some full code files in this repo for the larger functionalities I implemented.


## Back End Stories
* [763: Contact Form](#contact-form)
* [780: Email Template](#email-template)
* [750: User Details Partial](#user-details-partial)



### Contact Form
This ticket requested a way for any user to send an email to the admins using a form created in the Contact View. To do this I had to create a 'dummy' email account that would send emails populated with data from the users form.

To start, I created the form in the contact view:
  > ![login1](snippets/763-ContactForm/763-ContactView.png)

Then, I created a new model for the messages:
  > ![login1](snippets/763-ContactForm/763-EmailModel.png)

Finally, I added code to the HomeController so that the data can be passed to the model and then used by another method that creates the email and sends it:
  > ![login1](snippets/763-ContactForm/763-Homecontroller1.png)
  > ![login1](snippets/763-ContactForm/763-Homecontroller2.png)


### Email Template
I was tasked with improving the content of the emails sent from the program so that they include more information about the user, as well as a do-not-reply warning.

I modified the form in the ContactView:
  > ![](snippets/780-EmailTemplate/780-ContactView.png)


I had to update my EmailModel to reflect those changes:
  > ![](snippets/780-EmailTemplate/780-EmailModel.png)

In the HomeController, I added some string formatting to create the body of the email:
  > ![](snippets/780-EmailTemplate/780-HomeController.png)
    *note: I changed the email address back to the previous one after I confirmed that my changes were successful*

The final result: 
  > ![](snippets/780-EmailTemplate/780-EmailFormattingResult.png)


### User Details Partial
This user story required that in the Admin area, a partial be created that displays all of the users in the database, as well as their details.

The Partial View using the ApplicationUser Model to populate a table of all the users and their details:
  > ![](snippets/750-UserDetailsPartial/750-PartialView.png)

I also created a ViewModel for future functionality:
  > ![](snippets/750-UserDetailsPartial/750-ViewModel.png)
  > ![](snippets/750-UserDetailsPartial/750-ViewModel2.png)

The result:
  > ![](snippets/750-UserDetailsPartial/750-Result.png)

---
*Jump to: [Front End Stories](#front-end-stories), [Back End Stories](#back-end-stories), [Other Skills](#other-skills-learned), [Page Top](#live-project)*


## Front End Stories
* [720: Clock In/Clock out Modals](#modals)
* [738: Clock In Page Button](#clock-in-page-button)



### Modals
This ticket targets the Login View. My task was to add additional modals that display the current clock-in/clock-out time in red. 

  ![login1](snippets/720-ModalTime/720-LoginView1.png)

  ![login2](snippets/720-ModalTime/720-LoginView2.png)

  ![login3](snippets/720-ModalTime/720-LoginView3.png)

  ![login3](snippets/720-ModalTime/720-Javascript.png)

  
*Jump to: [Front End Stories](#front-end-stories), [Back End Stories](#back-end-stories), [Other Skills](#other-skills-learned), [Page Top](#live-project)*

## Other Skills Learned
* Working with a group of developers to identify front and back end bugs to the improve usability of an application
* Improving project flow by communicating about who needs to check out which files for their current story
* Learning new efficiencies from other developers by observing their workflow and asking questions  
* Practice with team programming/pair programming when one developer runs into a bug they cannot solve
  
*Jump to: [Front End Stories](#front-end-stories), [Back End Stories](#back-end-stories), [Other Skills](#other-skills-learned), [Page Top](#live-project)*