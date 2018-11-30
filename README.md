# Mobile-Apps---CMPS121

ASGN1:
  Create our first app consisting of three buttons. Each button has a new page/activity where we do certain things.
  What the buttons do:
  
    Enter Info - Enter info about photos with text and saves this information onto the device. 
    
    
      Done- Exit out of the current info page and move back to Main Menu
      
      
    View - View our typed in information after entering in our data
    
    
    Exit - Simply exits while keeping our data after the application has closed.
    
    
    
 The main difficulty with this assignment had to deal with keeping our data stored and having it persist across multiple activities(view screens). Not only that, but making it transition seamlessly and working flawlessly when moving between different view screens was also an uphill climb. A very fun and enjoyable first application using Android Studio!
 
 
 ASGN2:
  Create a mobile version of Connect Four board game. Main appeal of this assignment was to get the hang of fragments and having it   interact with an Activity. Fragments are like activities except more part of the UI and each fragment has its own life cycle. Very enjoyable if not challenging experience.
  
      Fragment - Represented the board and circles
    
      Main Activity- Where you can start a new game or continue off of the previous one
      
      
I had many difficulties getting the hang of fragments overall and it definitely was a nice learning experience. Getting the hang of Android studio and the complexities of the Java language is always a big plus!

ASGN3:
Create a background service to detect phone movement for Android.

Here are some notes taken at that time
Detecting phone movement

Plan to create:
1. When app first starts, create a background service running in its own thread
2. Create a variable called "first_accel_time" : this variables stores the time, T0, of when the background service first started
	2.5. Set "first_accel_time = null" initially
	2.6. Create variable T1, storing the time if the phone moved
	2.7. If T1 - T0 > 30 seconds , we set first_accel_time = T1
	2.8 
3. We measure movement from the accelerometer, measure significant acceleration in x and y directions 


---- 

Main Activity:

1. Start the service
2. Binds to it
3. Calls the method didItMove to service --> calls to ServiceTask
4. Update UI accordingly



---

Clear Button: Activity calls the service and the service
1. Set T0 to the current time
2. Set first_accel_time = null
