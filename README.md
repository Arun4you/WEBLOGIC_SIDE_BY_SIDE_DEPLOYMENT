# WEBLOGIC_SIDE_BY_SIDE_DEPLOYMENT

Side-by-side deployment is used to deploy a new version of an application while the older version is still actively serving clients. 

Because side-by-side application deployment is intended to have two different versions of an application deployed simultaneously, it is necessary to distinguish between the two versions of the application.

In this case, we have to specify the "WebLogic-Application-Version" for the web app to distinguish the old version from the new one.

You need to have META-INF/MANIFEST.MF file for your EARs as well.

MANIFEST.MF Content in EAR1 and EAR2:

EAR 1:

Manifest-Version: 1.0
Class-Path:
WebLogic-Application-Version: v1

EAR 2:

Manifest-Version: 1.0
Class-Path:
WebLogic-Application-Version: v2
