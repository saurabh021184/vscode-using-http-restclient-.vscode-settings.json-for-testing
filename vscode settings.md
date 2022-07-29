# How to use settings.json file under .vscode directory 

Basically you saw how to use restclient to execute API requests in the file test_api.http
Now there you need to do following thing:

@APIKEY={{APIKEY_DUMMY}}
@HOST={{HOST_LOCAL}}

you were manually copy pasting the APIKEY and HOST values based on DEV QA environment...-> how you can avoid this also.

so all you need to do is:
1. in your vscode project (in the ROOT or top most location) - create a folder .vscode folder
2. inside this .vscode folder create a file settings.json

![image](https://user-images.githubusercontent.com/109071677/181795719-f0fef8d2-a0fe-49e8-9754-3006070dc4ca.png)

3. and inside this json file you can put all the HOSTS and APIKEYS as environment variables
4. after this you also need to adjust test_api.http with some basic changes
   (refer to settings.json file and test_api_after_making_settings.http file for more details)

# After you did the above changes how to use these environment variables
1. In the bottom right of Vscode you will get the option to change your Rest Client Environment
    ![image](https://user-images.githubusercontent.com/109071677/181798682-49f0ccd9-4895-48b4-8976-0c6c7e551633.png)

2. The you will see the options to change your environment based on evironment variables you created in settings.json file
    ![image](https://user-images.githubusercontent.com/109071677/181798897-dc722d82-f9e8-45d0-a9b0-3a8a4176cc71.png)

3. That's it Just use your test_api_xxx.http file without any manual copy pasting to change the environment variable
4. One thing -> you can change your vscode colors etc. with the property 
    "workbench.colorCustomizations": {
        "titleBar.activeBackground": "#45a1ac",
        "statusBar.background": "#45a1ac"
        
   """just hover your around it you will see color pallete to change it
   ![image](https://user-images.githubusercontent.com/109071677/181799496-85e4c43c-27f1-4321-b0e4-9f01fc9c9102.png)

# THANK YOU!!!!!
# References:
1. https://code.visualstudio.com/docs/getstarted/settings#_settingsjson
2. https://courses.codewithandrea.com/courses/783023/lectures/14364306
