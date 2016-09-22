# HW_09-24
2) Write a short paragraph in response to each of the following questions:

a. What is an Activity?

    It can be an user interface, a single screen that a user can interact with or simply view. You can have many activities
    in an app and for it to be complete in it's functionality, it will require a compilation of activities. Activity will 
    need to be switched from one to another, screens need to be switched over for a better user experience and for an app to
    be responding to user input.
    
    You need an XML to define the look of the activity and a java file to program the functionality starting with activating
    it on the phone. It has to be declared in the manifest so that the system can invoke it.
    
b. What is the Manifest?

    It's an XML file where programmer defines what the requirements are in order for the app to run and what it contains:
    included app components, java package, permissions, minimum API level, libraries, and intent filters.
    
    Only <manifest> and <application> elements are required and can only occur once. Exceptions to order of elements:
      <activity-alias> is after <activity> that has the alias
      
      <application> must be the last element inside <manifest> element e.g. </application></manifest>
      
      Other than attributes of <manifest>, all other attributes begin with android:
      
      subclasses are defined through a name attribute and ti must include full package name
      
c. What is an Intent? Describe the difference between an implicit and explicit Intent.

    A java class to describe an operation to be performed used to start activities (from another activity or from launcher)
    or startService
    
    Explicit Intent: specify component to provide the exact class to be run and is simply a way to launch internal activities
    
    Implicit Intent: system determined which component is the best fit a s longa s enough information is included 
    - handled by intent resolution
        - matches intent gagains tall of the <intent-filter> (found in manifest.xml)
          using action, type, category to find the component that can handle them
