Django Chat Async with Tornado Server
=====================================

This is chat asynchronous servers/frameworks together with Django/tornado.

Includes:

* Django application - simple chat for authenticated users - every user can write messages, every user can remove any message. 

* async servers Python Tornado + Socket.IO listen to connections from chat application.


Install and run
===============

1) Clone this repo:

```bash
git clone https://github.com/tgonzales/apolonius.git
```

2) I suppose that you are familiar with virtualenv. Let's run our Django application:

```bash
pip install -r apolonius/requirements.txt
python apolonius/manage.py syncdb
python apolonius/manage.py runserver	
python tornado-socketio/server.py
```

Go to `http://localhost:8000` and make sure that everything works.

```

By default every async server will run on port 8001, but you can easily change it in code. But do not forget to change `ASYNC_BACKEND_URL` in Django's `settings.py`

How it works.
-------------


