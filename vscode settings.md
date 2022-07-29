# How to use settings.json file under .vscode directory 

Basically you saw how to use restclient to execute API requests in the file test_api.http
Now there you need to do following thing:

@APIKEY={{APIKEY_DUMMY}}
  you can replace this APIKEY with either of the DUMMY,DEV or QA API keys as per your requirement
@HOST={{HOST_LOCAL}}
  similarly you can also replace HOST_LOCAL with HOST_DEV or HOST_QA as per your requirement

you were manually copy pasting the APIKEY and HOST values based on DEV QA environment...-> how you can avoid this also.

so all you need to do is:
1. in your vscode project (in the ROOT or top most location) - create a folder .vscode folder
2. inside this .vscode folder create a file settings.json

![image](https://user-images.githubusercontent.com/109071677/181795719-f0fef8d2-a0fe-49e8-9754-3006070dc4ca.png)

3. and inside this json file you can put all the HOSTS and APIKEYS as environment variables
4. after this you also need to adjust test_api.http with some basic changes
   (refer to settings.json file and test_api_after_making_settings.http file for more details)


# References:
1. https://code.visualstudio.com/docs/getstarted/settings#_settingsjson
