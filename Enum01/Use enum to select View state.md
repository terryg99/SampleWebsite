# Use enum to select View state  

In Poker Copilot, for example, the view displayed on the right side of the app window depends on which button has been tapped on the left side of the window. In PC7, we might tap the “Recent hands” button to display one set of results, or the ‘Players” button to show a different view.  

One way to implement this is to define an @State boolean for each view. The buttons then make the state false for the hidden view and true for the view to be shown  
![Screenshot 2025-05-10 at 6.30.58 AM.png](Attachments/Screenshot%202025-05-10%20at%206.30.58%E2%80%AFAM.png)  
This works fine and may be the best approach for cases where there are only 2 or 3 views to select from. But as the number of cases increases, the code complexity increases exponentially because we have to “turn off” all but the desired boolean and turn on the desired one. For 2 views, it takes basically 4 lines of code for the buttons, but for 3 views it takes 9. There must be a better way. Could we use an enum instead?  
[MultiView01](Attachments/MultiView01)  
![Screenshot 2025-05-10 at 6.44.10 AM.png](Attachments/Screenshot%202025-05-10%20at%206.44.10%E2%80%AFAM.png)  
The code complexity grows arithmetically with number of views, rather than geometrically as in the previous case.  
