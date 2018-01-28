# Volley
Hello my friend!
This is my first repository and I just wanted to post thing that was my problem recently. Let's see what we got here :
1. A Singleton Class which helps you with handling your volley requests and I'm telling you guys it's too simple and needs to be worked on commensurate with your project functionality.
2. An Interface which ofc you know that you need to have a listener btw.

And this is how to use it down here...
```java
   VolleySingleton.getInstance(this).addStringRequest(new VolleyCallback<String>() {
       @Override
       public void getResult(boolean state, String response) {
           Toast.makeText(SplashActivity.this, response + state, Toast.LENGTH_SHORT).show();
       }
   });
```
