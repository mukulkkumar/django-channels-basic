### This is a very basic setup of channels in django

#### *In this repository, I have just installed django and channels packages.*

#### channels config for django

```
pip install channels
```

#### Once that’s done, you should add channels to your INSTALLED_APPS setting:
```
INSTALLED_APPS = (
    'django.contrib.auth',
    'django.contrib.contenttypes',
    'django.contrib.sessions',
    'django.contrib.sites',
    ...
    'channels',
)
```

#### And finally, set your ASGI_APPLICATION setting to point to that routing object as your root application:

```
ASGI_APPLICATION = "myproject.asgi.application"
```

Then, Just did a very simple programming for django channels, so that we can see random numbers on our web page without refreshing it.
