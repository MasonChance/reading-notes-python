# Django Settings: best practices


While there are several ways to configure the layout and pathing of your settings for any given Django project, one of the hurdles in development is that different setups can cause conflicts when working with other devs particularily because environment variables should never be made public through the Version Control System (VCS). 

Technologies and our understanding of them is constantly changing and we naturally start developing our own processes to manage and work within this rapidly changing environment; one model for managing these changes in a relatively "common process" way is by following the guidelines from the [12 factor app](https://12factor.net/). 

The factor I will touch on here is 'configuration', as it relates to settings, and the handling of environment variables. 

- use a third-party package such as `django-environ` to manage and handle environment variables so that they never become public to the VCS. 

- however you configure your settings, all custom settings should have descriptive variable names and comments regarding their purpose and relation to the codebase.

- seperate settings based on thier origin/scope of effect. ie. separate file for local_settings, third party settigns, environment settings, framework settings, custom settings etc

```
.venv
settings/
\_\_init\_\_.py
--> local_settings/
------> django_settings.py
------> env_settings.py
--> third_party_settings/
------> rst_frame_settings.py
------> whitenoise_settings.py
--> custom_settings/
------> production_settings.py

``` 

The above example is one way to configure settings files and makes tracing setting dependencies a lot clearer when tracing errors. when using this method, all settings files should be imported into the `__init__.py` file.

```
# settings/`__init__.py` :

from .local_settings.django_settings import *
from .local_settings.django_settings import *
from .third_party_settings.rst_frame_settings import *
from .third_party_settings.whitenoise_settings import *
from .custom_settigns.production_settings import *

``` 








#### [Return to Main index of Notes](./README.md)