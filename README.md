QWsensor
========

Quick work - Making use of an environmental sensor


Project to access the Quirky-Wink-Spotter sensor data.  Hopefully to make quick work of using this data for monitoing and security uses for many.

First, praise for the responsive customer support team for this product.  I purchased this product in Fall 2013.  I liked the device and the idea, but was unable to get to the data to apply it.  Whether by coincidence or by amazing customer service based on feedback, they opened up a beta API and Steven Shaw sent me Oauth client IDs.


Phase 0
=======
If you are just getting started, trying to access your Spotter data, may I suggest the guidance of Marshall T. Rose: http://branch.com/b/wink-api#E4f6qUKBeKY


Phase 1
=======
Establish contact with the Quirky.com servers.  I found the quickest to be:


  curl --include --header "Content-Type: application/json"  --request POST  --data-binary "{ \"client_id\": \"YourClientID\",  \"client_secret\":\"YourCLientSecret\",  \"username\":\"YourQuirkyWinkEmail\",  \"password\": \"YourQuirkyWinkPassword\",  \"grant_type\":\"password\"}"  "https://winkapi.quirky.com/"
  

Phase 3
=======
The Wink API docs provide a starting place for several languages.  http://docs.wink.apiary.io/


Phase 4
=======
Others and I and perhaps yourself, will be writing code to make it easier to put the Spotter data to use.

Projects in my queue:

1) Python 3 code samples.  The Pythin in http://docs.wink.apiary.io/ was Python 2.

2) Android app for viewing sensor data

3) Try to keep a list of Spotter tools:
  https://play.google.com/store/apps/details?id=com.quirky.android.wink.wink&hl=en
  
