https://docs.djangoproject.com/ko/3.1/intro/tutorial01/

```
$ django-admin startproject mysite
$ python manage.py startapp polls
```

- The outer mysite/ root directory is a container for your project. Its name doesn't matter to Django; you can rename it to anything you like.
- manage.py: Django 프로젝트와 다양한 방법으로 상호작용 하는 커맨드라인의 유틸리티 입니다. manage.py 에 대한 자세한 정보는 [django-admin and manage.py](https://docs.djangoproject.com/ko/3.1/ref/django-admin/) 에서 확인할 수 있습니다.
- mysite/ 디렉토리 내부에는 프로젝트를 위한 실제 Python 패키지들이 저장됩니다. 이 디렉토리 내의 이름을 이용하여, (mysite.urls 와 같은 식으로) 프로젝트의 어디서나 Python 패키지들을 임포트할 수 있습니다.
- mysite/**init**.py: Python으로 하여금 이 디렉토리를 패키지처럼 다루라고 알려주는 용도의 단순한 빈 파일입니다. Python 초심자라면, Python 공식 홈페이지의 [패키지](https://docs.python.org/3/tutorial/modules.html#tut-packages)를 읽어보세요.
- mysite/settings.py: 현재 Django 프로젝트의 환경 및 구성을 저장합니다. [Django settings](https://docs.djangoproject.com/ko/3.1/topics/settings/)에서 환경 설정이 어떻게 동작하는지 확인할 수 있습니다.
- mysite/urls.py: 현재 Django project 의 URL 선언을 저장합니다. Django 로 작성된 사이트의 "목차" 라고 할 수 있습니다. [URL dispatcher](https://docs.djangoproject.com/ko/3.1/topics/http/urls/) 에서 URL 에 대한 자세한 내용을 읽어보세요.
- mysite/asgi.py: An entry-point for ASGI-compatible web servers to serve your project. See [How to deploy with ASGI](https://docs.djangoproject.com/ko/3.1/howto/deployment/asgi/) for more details.
- mysite/wsgi.py: 현재 프로젝트를 서비스하기 위한 WSGI 호환 웹 서버의 진입점입니다. [How to deploy with WSGI](https://docs.djangoproject.com/ko/3.1/howto/deployment/wsgi/)를 읽어보세요.
