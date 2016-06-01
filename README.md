AngularFire Course
========================

The course is out of date only in reference to the management console. A new version of the management console has been released. The UI is different, but it has all the same functionality. You should be easily able to find the same functionality in the new console that I show in the old console.

There are also a couple of problems/bugs with the new management console:

**The New Management Console**
Currently, there are known bugs with Firebases created in the new console in relation to authentication. For that reason I recommend that you create any new firebase using the classic management console here: https://www.firebase.com/account/#/ then if you wish you can upgrade it to the new management console.

**New Management Console Authentication**
The only problem currently is in your facebook authentication setup. The new firebase console documents are incorrect. 

If you click the "learn more" link when configuring facebook authentication in your application, and walk through the steps that firebase outlines, you will come to a step where you are directed to add a "OAuth redirect URI" to your facebook app with the format like this:

https://YOUR-APP-NAME.firebaseapp.com/__/auth/handler 

but in reality, you need to add a url like this:

https://auth.firebase.com/v2/YOUR-APP-NAME/auth/facebook/callback

You can find a walkthrough of the process that I made here: https://www.youtube.com/watch?v=8XnUs2xY5c4&feature=youtu.be



