![alt text](https://raw.githubusercontent.com/dilentulcidas/mbmanager/master/githubimages/mbexplorerheader.png "MBExplorer header")

![alt text](https://raw.githubusercontent.com/dilentulcidas/mbmanager/master/githubimages/preview.png "MBExplorer screenshots")

# Description
This is the source code for a web app made with Spring Boot (Java) and also integrating a RESTful API. The goal of this app is for the user to store any bookmarks in a straightforward manner, all of which being saved in the database (MongoDB). The user can create folders to organize the respective bookmarks, and can add three types of bookmarks: location, text and url. 

Due to ``|`` being used as separator for the path of the folder/item, and it being incompatible with Tomcat 8, the ``VM OPTIONS`` of the running configuration for this app must have the following in order to not return page error:
```
-Dtomcat.util.buf.StringCache.byte.enabled=true -Dtomcat.util.http.parser.HttpParser.requestTargetAllow=|{}
```

**Last update:** 19th January 2018

[Web app access here](http://mybookmarkexplorer-springprojects.1d35.starter-us-east-1.openshiftapps.com/)
