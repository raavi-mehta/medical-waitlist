# Heuristic Evaluation of Hi-Fi Prototype
Our application has three components. The first is a clinic client that shows
the waitlist on a screen within the clinic. The second is a mobile application
for patient use. The third is a receptionist client on a desktop that manages
information available to both the clinic and mobile clients. In document, we
will highlight how well our system adheres to the various heuristics.

## 1. Visibility of System Status 
The mobile application clearly uses headers on each page (sign up, find a
clinic, etc.) to show the user where they are. On the mobile application, when
the user checks in to a clinic, a message is displayed indicating that the user
successfully checked in to the clinic and the clinic is added to the user’s
Current Booking screen. In the settings for the receptionist’s client, each of
the section headers are highlighted based on which section is currently selected
so that the user can always know which section they are currently on.

Regarding negatives, the sandwich menu that the user uses to navigate most of
the application does not indicate to the user which page they are currently on
(though headers are provided on the pages themselves. No indicators are provided
anywhere in the app outside of the “Current Booking” screen to indicate that the
user is currently checked into a clinic.

## 2. Match Between System and the Real World 
Icons such as a gear and tool icon for settings or a bell icon for notifications
are used to help the user relate functionality of the application with the
applicable items. For the receptionist client features such as themes in the
settings menu actually show a color preview. In the mobile application the real
pictures of the clinics are shown further connecting the application to the real
world. On the mobile application, hearts and stars are used to indicate
favourite clinics and clinic ratings, respectively. This iconography is
intuitive because it matches real world concepts.

Some of the iconography in the mobile app is not intuitive (specifically, the
icons used in the sandwich menu, where a ‘home’ icon is used to represent the
“Find a Clinic” page). Few attempts are made in the mobile application to use
metaphor to make the interface more intuitive; the interface is presented in the
form of lists of text.

## 3. User Control and Freedom 
For the receptionist client the user can add new patients manually, delete
patients, move patients around on the waitlist (not implemented), edit patient
information (not implemented), and change various settings associated with
themes (not implemented), and text. Note a few buttons are dead/not working
since they were not implemented due to time constraints. On the mobile
application the user can easily move between states and edit things such as
their favorites lists. The applications do not allow full control such as
importing your own themes or changing the layout since we believe the tradeoffs
i.e. losing a recognizable interface is not worth the perceived benefits of
giving the users more control. Also deleting favorite clinics from the mobile
application or deleting patients on the waitlist for the desktop application can
not be undone. This is a major oversight since a user could accidently delete
this information and there is no way to quickly get it all back. An additional
problem is that the user can currently only have one clinic saved in “My
Clinics.” This lack of undo functionality is also an issue in the receptionist’s
client where the receptionist might accidently remove a patient from the list.

## 4. Consistency and Standards
The mobile application uses standard Android iconography for things such as
settings, and search functions. The theme for the mobile application is unified
under Android’s Material Design and no item has a duplicate meaning. The same
can be said for the receptionist application with the exception in style choices
to adhere more of a desktop environment instead of a mobile/touchscreen one. The
settings for the receptionist client also includes a menu bar to select various
settings section which is standard in many desktop applications.

Although consistency is preserved within applications, the same is not true
between applications. An example is a wrench icon being used to represent
settings in the mobile application compared to a gear icon being used to
represent the same thing in the receptionist desktop application. Going forward
we will try to bridge this divide and make the applications more consistent
across the various components. 

## 5. Error Prevention 
When signing up for a new account the application does not allow the user to
continue without filling out the required information. Moreover, when the user
is about to cancel their appointment, the app notifies them and asks them if
they are sure they want to cancel. Also the design of both the mobile and
desktop applications are simple, streamlined, and there is appropriate spacing
between buttons reducing accidental clicks. However in the desktop application,
there is currently no mechanism to prevent blank patient or doctors names for
the various data entry; this functionality may be useful since blank names are
almost never intentional.

## 6. Recognition Rather than Recall 
There are multiple parts of the different systems that allow users to quickly
recognize and access the information or settings that they need. On the mobile
application the pictures of clinics are added so a user can quickly recognize a
clinic they are familiar with. There is also a favorites list, and “my
appointment” for the mobile application. These elements allow the user to access
clinics easily without having to remember clinic-specific information, such as
name or address. 

The mobile client does not provide a list of most recently visited clinics. This
would have been a helpful addition that would allow users to recognize which
clinics they recently visited rather than remembering their names. The mobile
application also does not provide a map-like interface that allows users to find
clinics on a map. Again, this would reduce the amount of information that the
user has to remember.

## 7. Flexibility and Efficiency of Use
The mobile application has a lot of functionality. Always visible menus allow
users to quickly find different information such as which doctors are on, clinic
information, and/or appointment information. For the mobile application, certain
functionalities are flexible in the sense that users can access them from
multiple screens. Namely, this includes the favourite clinics functionality,
which can be accessed from both a clinic’s information page and the “Current
Booking” page. Users can navigate back and forward between pages for optimal
efficiency. The receptionist client has a more simplified layout, but again, the
interface was designed to make navigation quick and efficient.

The mobile app provides very few shortcuts for increased efficiency. That said,
the application is quite simple, and therefore most tasks only require two -
three clicks to accomplish. On the receptionist desktop client, it may have been
useful to include keyboard shortcuts for more advanced users to increase the
efficiency of their workflow. Again, we justified omitting this functionality
because of the simplicity of the overall app, but it may have been useful
nonetheless.

## 8. Aesthetic and Minimalist Design 
All features are designed to be simple and easy to access. With exception of the
news ticker on the clinic display, all the information in each application is
relevant. The news ticker adds more functionality to display client at the
expense of relevance, but it can be removed or customized by the receptionist to
be more relevant. Each component utilizes space well without being cluttered.
The mobile application provides sorting and searching functionality on the
clinic select page to help users manage the data available from that screen,
simplifying the experience. The mobile application makes use of material design
to ensure that it is aesthetically pleasing and minimalistic. Small touches such
as different colours for different wait times and the use of a heart icon that
becomes red when a clinic is in your favourites make the mobile application more
aesthetically pleasing.

While the mobile app’s select clinic page has a lot of information on it, it
provides the aforementioned sort and search tools. The “My Clinics” page
however, does not provide these tools, meaning the page could quickly get
cluttered with more clinics being added.

## 9. Help users Recognize, Diagnose, and Recover from Errors 
In the signup phase for the mobile application, if the user doesn’t enter the
required information into a field, a message will tell them the specific
information they are missing so that they can fill it out correctly. Also on the
mobile app, if you are not checked in and you view the “Current Booking”, it
will tell the user that they must check in first, thereby allowing them to
recover from this erroneous situation. Unfortunately, for the edit information
and sign up pages on the mobile app, every field requires that the user enter
information directly into a textbox. If the information is wrong, the app does
not alert the user that the information is wrong and will not be able to help
the user fix the erroneous information. 

## 10. Help and Documentation 
The receptionist’s desktop client currently includes a “Help” section within the
settings component which offers a centralized area for referencing help-related
information. This documentation also includes a link to our GitHub page to view
more documentation and to view and add to the issue tracker. Furthermore, the
mobile app includes a walkthrough for first-time users so that they can more
easily learn how to use the application.

In terms of negatives, the mobile client does have a placeholder section for
“Help”, but this is not currently populated due to time-constraints.
Furthermore, it would be helpful for the user if the documentation was a little
more spread out instead of just having a centralized section for documentation -
for example, having mini help links throughout the system to elaborate on
various workflow. Moreover, receptionists are unlikely to be familiar with
GitHub and are unlikely to derive much benefit from it.
