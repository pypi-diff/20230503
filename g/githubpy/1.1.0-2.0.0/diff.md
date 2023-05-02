# Comparing `tmp/githubpy-1.1.0.tar.gz` & `tmp/githubpy-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/githubpy-1.1.0.tar", last modified: Fri Feb 14 05:26:07 2014, max compression
+gzip compressed data, was "githubpy-2.0.0.tar", last modified: Tue May  2 23:48:35 2023, max compression
```

## Comparing `githubpy-1.1.0.tar` & `githubpy-2.0.0.tar`

### file list

```diff
@@ -1,5 +1,12 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2014-02-14 05:26:06.000000 githubpy-1.1.0/
--rw-r--r--   0 michael    (501) staff       (20)     9768 2014-02-14 05:24:33.000000 githubpy-1.1.0/github.py
--rw-r--r--   0 michael    (501) staff       (20)     1156 2014-02-14 05:26:06.000000 githubpy-1.1.0/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      373 2013-06-24 04:01:45.000000 githubpy-1.1.0/README
--rw-r--r--   0 michael    (501) staff       (20)      872 2014-02-14 05:24:33.000000 githubpy-1.1.0/setup.py
+drwxr-xr-x   0 liaoxuefeng   (501) staff       (20)        0 2023-05-02 23:48:35.412239 githubpy-2.0.0/
+-rw-r--r--   0 liaoxuefeng   (501) staff       (20)    35149 2023-05-02 23:26:11.000000 githubpy-2.0.0/LICENSE
+-rw-r--r--   0 liaoxuefeng   (501) staff       (20)      757 2023-05-02 23:48:35.411955 githubpy-2.0.0/PKG-INFO
+-rw-r--r--   0 liaoxuefeng   (501) staff       (20)      373 2023-05-02 23:26:11.000000 githubpy-2.0.0/README
+-rwxr-xr-x   0 liaoxuefeng   (501) staff       (20)    12398 2023-05-02 23:34:05.000000 githubpy-2.0.0/github.py
+drwxr-xr-x   0 liaoxuefeng   (501) staff       (20)        0 2023-05-02 23:48:35.411490 githubpy-2.0.0/githubpy.egg-info/
+-rw-r--r--   0 liaoxuefeng   (501) staff       (20)      757 2023-05-02 23:48:35.000000 githubpy-2.0.0/githubpy.egg-info/PKG-INFO
+-rw-r--r--   0 liaoxuefeng   (501) staff       (20)      161 2023-05-02 23:48:35.000000 githubpy-2.0.0/githubpy.egg-info/SOURCES.txt
+-rw-r--r--   0 liaoxuefeng   (501) staff       (20)        1 2023-05-02 23:48:35.000000 githubpy-2.0.0/githubpy.egg-info/dependency_links.txt
+-rw-r--r--   0 liaoxuefeng   (501) staff       (20)        7 2023-05-02 23:48:35.000000 githubpy-2.0.0/githubpy.egg-info/top_level.txt
+-rw-r--r--   0 liaoxuefeng   (501) staff       (20)       38 2023-05-02 23:48:35.412328 githubpy-2.0.0/setup.cfg
+-rw-r--r--   0 liaoxuefeng   (501) staff       (20)      939 2023-05-02 23:47:20.000000 githubpy-2.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `githubpy-1.1.0/github.py` & `githubpy-2.0.0/github.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,307 +1,378 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3
 # -*-coding: utf8 -*-
 
 '''
-GitHub API Python SDK. (Python >= 2.5)
+GitHub API Python3 SDK.
 
-Apache License
+GPLv3 License
 
 Michael Liao (askxuefeng@gmail.com)
 
+https://github.com/michaelliao/githubpy
+
 Usage:
 
->>> gh = GitHub(username='githubpy', password='test-githubpy-1234')
->>> L = gh.users('githubpy').followers.get()
->>> L[0].id
-470058
->>> L[0].login == u'michaelliao'
-True
->>> x_ratelimit_remaining = gh.x_ratelimit_remaining
+>>> token = os.getenv('GITHUB_TOKEN') # token from env or other source
+>>> proxy = os.getenv('HTTPS_PROXY') # proxy for access https, default to None
+>>> gh = GitHub(token, proxy=proxy)
+>>> L = gh.users('michaelliao').followers.get()
+>>> L[0].login # doctest: +ELLIPSIS
+'...'
+>>> print('rate limit remaining: ', gh.x_ratelimit_remaining) # doctest: +ELLIPSIS
+rate limit remaining: ...
 >>> x_ratelimit_limit = gh.x_ratelimit_limit
 >>> x_ratelimit_reset = gh.x_ratelimit_reset
->>> L = gh.users('githubpy').following.get()
->>> L[0].url == u'https://api.github.com/users/michaelliao'
-True
->>> L = gh.repos('githubpy')('testgithubpy').issues.get(state='closed', sort='created')
->>> L[0].title == u'sample issue for test'
-True
+>>> L = gh.users('michaelliao').following.get()
+>>> L[0].url # doctest: +ELLIPSIS
+'https://api.github.com/users/...'
+>>> L = gh.repos('michaelliao')('githubpy').issues.get(state='closed', sort='created', direction='asc')
+>>> L[0].title
+'No license'
 >>> L[0].number
 1
->>> I = gh.repos('githubpy')('testgithubpy').issues(1).get()
->>> I.url == u'https://api.github.com/repos/githubpy/testgithubpy/issues/1'
-True
->>> gh = GitHub(username='githubpy', password='test-githubpy-1234')
->>> r = gh.repos('githubpy')('testgithubpy').issues.post(title='test create issue', body='just a test')
->>> r.title == u'test create issue'
-True
->>> r.state == u'open'
-True
+>>> I = gh.repos('michaelliao')('githubpy').issues(1).get()
+>>> I.url
+'https://api.github.com/repos/michaelliao/githubpy/issues/1'
+>>> new_issue = { 'title': 'New issue test', 'body': 'Test create issue with githubpy', 'assignees': ['michaelliao']}
+>>> r = gh.repos('michaelliao')('githubpy').issues.post(new_issue)
+>>> r.title
+'New issue test'
+>>> r.state
+'open'
+>>> exist = gh.repos('michaelliao')('githubpy').contents('test/café.txt').get() # doctest: +ELLIPSIS
+{...}
+>>> # update exist file:
+>>> import base64, datetime
+>>> dt = datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
+>>> file_content = bytes('Hello world! ' + dt, 'utf-8')
+>>> update = { 'message': 'Update file at ' + dt, 'committer': { 'name': 'Michael', 'email': 'askxuefeng@gmail.com' }, 'content': base64.b64encode(file_content).decode('utf-8'), 'sha': exist.sha }
+>>> commit = gh.repos('michaelliao')('githubpy').contents('test/café.txt').put(update)
+>>> commit.content.url
+'https://api.github.com/repos/michaelliao/githubpy/contents/test/caf%C3%A9.txt?ref=master'
 >>> gh.repos.thisisabadurl.get()
 Traceback (most recent call last):
     ...
 ApiNotFoundError: https://api.github.com/repos/thisisabadurl
 >>> gh.users('github-not-exist-user').followers.get()
 Traceback (most recent call last):
     ...
 ApiNotFoundError: https://api.github.com/users/github-not-exist-user/followers
 '''
 
-import re, os, time, hmac, base64, hashlib, urllib, mimetypes, json
+__version__ = '2.0.0'
 
-try:
-    # Python 2
-    from urllib2 import build_opener, HTTPSHandler, Request, HTTPError
-    from urllib import quote as urlquote
-    from StringIO import StringIO
-    def bytes(string, encoding=None):
-        return str(string)
-except:
-    # Python 3
-    from urllib.request import build_opener, HTTPSHandler, HTTPError, Request
-    from urllib.parse import quote as urlquote
-    from io import StringIO
+from urllib.request import build_opener, HTTPSHandler, HTTPError, Request
+from urllib.parse import quote
+from io import StringIO
 
-from collections import Iterable
+import re, os, time, hmac, base64, hashlib, urllib, mimetypes, json
+from collections import namedtuple
+from collections.abc import Iterable
 from datetime import datetime, timedelta, tzinfo
 
-TIMEOUT=60
+TIMEOUT = 60
 
-__version__ = '1.1.0'
+_API_VERSION = '2022-11-28'
 
 _URL = 'https://api.github.com'
+
 _METHOD_MAP = dict(
         GET=lambda: 'GET',
         PUT=lambda: 'PUT',
         POST=lambda: 'POST',
         PATCH=lambda: 'PATCH',
         DELETE=lambda: 'DELETE')
 
 DEFAULT_SCOPE = None
+
 RW_SCOPE = 'user,public_repo,repo,repo:status,gist'
 
+AccessToken = namedtuple('AccessToken', ['access_token', 'scope', 'token_type'])
+
+
+def _encode_path(path):
+    '''
+    Encode url path.
+    '''
+    return quote(path, encoding='utf-8')
+
+def _encode_params(kw):
+    '''
+    Encode parameters.
+
+    >>> kw = { 'a': 'K&R', 'lang': 'Ελληνικά,Français,中文,日本語', 'page': 1 }
+    >>> _encode_params(kw)
+    'a=K%26R&lang=%CE%95%CE%BB%CE%BB%CE%B7%CE%BD%CE%B9%CE%BA%CE%AC%2CFran%C3%A7ais%2C%E4%B8%AD%E6%96%87%2C%E6%97%A5%E6%9C%AC%E8%AA%9E&page=1'
+    '''
+    args = []
+    for k, v in kw.items():
+        q = quote(str(v), encoding='utf-8')
+        args.append(f'{k}={q}')
+    return '&'.join(args)
+
+def _encode_json(obj):
+    '''
+    Encode object as json str.
+    '''
+    def _dump_obj(obj):
+        if isinstance(obj, dict):
+            return obj
+        d = dict()
+        for k in dir(obj):
+            if not k.startswith('_'):
+                d[k] = getattr(obj, k)
+        return d
+    return json.dumps(obj)
+
+def _parse_json(jsonstr):
+    def _obj_hook(pairs):
+        o = JsonObject()
+        for k, v in pairs.items():
+            o[str(k)] = v
+        return o
+    return json.loads(jsonstr, object_hook=_obj_hook)
+
+class _Get(object):
+
+    def __init__(self, _gh, _path):
+        self._gh = _gh
+        self._path = _path
+
+    def __call__(self, **kw):
+        return self._gh._http('GET', self._path, None, **kw)
+
+    def __str__(self):
+        return f'GET {self._path}'
+
+    __repr__ = __str__
+
+class _Executable(object):
+
+    def __init__(self, _gh, _method, _path):
+        self._gh = _gh
+        self._method = _method
+        self._path = _path
+
+    def __call__(self, data=None):
+        return self._gh._http(self._method, self._path, data)
+
+    def __str__(self):
+        return '_Executable (%s %s)' % (self._method, self._path)
+
+    __repr__ = __str__
+
+class _Callable(object):
+
+    def __init__(self, _gh, _name):
+        self._gh = _gh
+        self._name = _name
+
+    def __call__(self, *args):
+        n = len(args)
+        if n == 0:
+            return self
+        if n == 1:
+            return _Callable(self._gh, self._name + '/' + _encode_path(str(args[0])))
+        return _Callable(self._gh, self._name + '/' + '/'.join([_encode_path(str(arg)) for arg in args]))
+
+    def __getattr__(self, attr):
+        if attr == 'get':
+            return _Get(self._gh, self._name)
+        if attr == 'put':
+            return _Executable(self._gh, 'PUT', self._name)
+        if attr == 'post':
+            return _Executable(self._gh, 'POST', self._name)
+        if attr == 'patch':
+            return _Executable(self._gh, 'PATCH', self._name)
+        if attr == 'delete':
+            return _Executable(self._gh, 'DELETE', self._name)
+        return _Callable(self._gh, f'{self._name}/{attr}')
+
+    def __str__(self):
+        return '_Callable (%s)' % self._name
+
+    __repr__ = __str__
+
 class GitHub(object):
 
     '''
     GitHub client.
     '''
 
-    def __init__(self, username=None, password=None, access_token=None, client_id=None, client_secret=None, redirect_uri=None, scope=None):
-        self.x_ratelimit_remaining = (-1)
-        self.x_ratelimit_limit = (-1)
-        self.x_ratelimit_reset = (-1)
-        self._authorization = None
-        if username and password:
-            # roundabout hack for Python 3
-            userandpass = base64.b64encode(bytes('%s:%s' % (username, password), 'utf-8'))
-            userandpass = userandpass.decode('ascii')
-            self._authorization = 'Basic %s' % userandpass
-        elif access_token:
-            self._authorization = 'token %s' % access_token
-        self._client_id = client_id
-        self._client_secret = client_secret
-        self._redirect_uri = redirect_uri
-        self._scope = scope
+    def __init__(self, token=None, proxy=None, debug=False):
+        self.x_ratelimit_remaining = -1
+        self.x_ratelimit_limit = -1
+        self.x_ratelimit_reset = -1
+        self._authorization = f'Bearer {token}' if token else None
+        self._debug = debug
 
-    def authorize_url(self, state=None):
+    @classmethod
+    def authorize_url(cls, client_id, redirect_uri, scope=None, state=None, **kw):
         '''
         Generate authorize_url.
 
-        >>> GitHub(client_id='3ebf94c5776d565bcf75').authorize_url()
-        'https://github.com/login/oauth/authorize?client_id=3ebf94c5776d565bcf75'
+        scope: A space-delimited list of scopes. Default to None (no scope, read-only access to public information). See https://docs.github.com/en/developers/apps/building-oauth-apps/scopes-for-oauth-apps
+        state: An unguessable random string. It is used to protect against cross-site request forgery attacks. Default to None (do not use state).
+
+        >>> GitHub.authorize_url(client_id='3ebf94c5776d565bcf75', redirect_uri='https://example.com/callback', scope='public_repo, user', allow_signup='false')
+        'https://github.com/login/oauth/authorize?allow_signup=false&client_id=3ebf94c5776d565bcf75&redirect_uri=https%3A//example.com/callback&scope=public_repo%2C%20user'
         '''
-        if not self._client_id:
-            raise ApiAuthError('No client id.')
-        kw = dict(client_id=self._client_id)
-        if self._redirect_uri:
-            kw['redirect_uri'] = self._redirect_uri
-        if self._scope:
-            kw['scope'] = self._scope
+        if not client_id:
+            raise ValueError('Bad argument of client_id.')
+        if not redirect_uri:
+            raise ValueError('Bad argument of redirect_uri.')
+        kw['client_id'] = client_id
+        kw['redirect_uri'] = redirect_uri
+        if scope:
+            kw['scope'] = scope
         if state:
             kw['state'] = state
-        return 'https://github.com/login/oauth/authorize?%s' % _encode_params(kw)
+        params = _encode_params(kw)
+        return f'https://github.com/login/oauth/authorize?{params}'
 
-    def get_access_token(self, code, state=None):
+    @classmethod
+    def get_access_token(cls, client_id, client_secret, code, redirect_uri=None, state=None):
         '''
         In callback url: http://host/callback?code=123&state=xyz
 
-        use code and state to get an access token.        
+        use code and state to get an access token.
         '''
-        kw = dict(client_id=self._client_id, client_secret=self._client_secret, code=code)
-        if self._redirect_uri:
-            kw['redirect_uri'] = self._redirect_uri
+        kw = dict(client_id=client_id, client_secret=client_secret, code=code)
+        if redirect_uri:
+            kw['redirect_uri'] = redirect_uri
         if state:
             kw['state'] = state
+        url = 'https://github.com/login/oauth/access_token'
         opener = build_opener(HTTPSHandler)
-        request = Request('https://github.com/login/oauth/access_token', data=_encode_params(kw))
+        request = Request(url, data=_encode_params(kw))
         request.get_method = _METHOD_MAP['POST']
         request.add_header('Accept', 'application/json')
         try:
             response = opener.open(request, timeout=TIMEOUT)
             r = _parse_json(response.read())
             if 'error' in r:
-                raise ApiAuthError(str(r.error))
-            return str(r.access_token)
+                raise ApiAuthError(400, url, r.error)
+            return AccessToken(r.access_token, r.scope, r.token_type)
         except HTTPError as e:
-            raise ApiAuthError('HTTPError when get access token')
+            raise ApiAuthError(e.code, url, 'HTTPError when get access token')
 
     def __getattr__(self, attr):
-        return _Callable(self, '/%s' % attr)
+        path = _encode_path(attr)
+        return _Callable(self, f'/{path}')
 
-    def _http(self, method, path, **kw):
+    def _http(self, _method, _path, _data=None, **kw):
         data = None
         params = None
-        if method=='GET' and kw:
-            path = '%s?%s' % (path, _encode_params(kw))
-        if method in ['POST', 'PATCH', 'PUT']:
-            data = bytes(_encode_json(kw), 'utf-8')
-        url = '%s%s' % (_URL, path)
+        if _method=='GET' and kw:
+            _path = '%s?%s' % (_path, _encode_params(kw))
+        if _method in ['POST', 'PATCH', 'PUT', 'DELETE']:
+            data = bytes(_encode_json(_data), 'utf-8')
+        url = f'{_URL}{_path}'
+        headers = {
+            'Accept': 'application/vnd.github+json',
+            'X-GitHub-Api-Version': _API_VERSION
+        }
+        if self._authorization:
+            headers['Authorization'] = self._authorization
+        if _method in ['POST', 'PATCH', 'PUT']:
+            headers['Content-Type'] = 'application/json'
         opener = build_opener(HTTPSHandler)
         request = Request(url, data=data)
-        request.get_method = _METHOD_MAP[method]
-        if self._authorization:
-            request.add_header('Authorization', self._authorization)
-        if method in ['POST', 'PATCH', 'PUT']:
-            request.add_header('Content-Type', 'application/x-www-form-urlencoded')
+        request.get_method = _METHOD_MAP[_method]
+        for k, v in headers.items():
+            request.add_header(k, v)
+        if self._debug:
+            curl = ['curl -v', f'  -X {_method}']
+            for k, v in headers.items():
+                curl.append(f'  -H "{k}: {v}"')
+            curl.append(f'  "{url}"')
+            if data:
+                curl.append(f'  -d \'{_encode_json(_data)}\'')
+            print(' \\\n'.join(curl))
         try:
             response = opener.open(request, timeout=TIMEOUT)
             is_json = self._process_resp(response.headers)
             if is_json:
                 return _parse_json(response.read().decode('utf-8'))
         except HTTPError as e:
             is_json = self._process_resp(e.headers)
             if is_json:
                 json = _parse_json(e.read().decode('utf-8'))
-            req = JsonObject(method=method, url=url)
-            resp = JsonObject(code=e.code, json=json)
-            if resp.code==404:
-                raise ApiNotFoundError(url, req, resp)
-            raise ApiError(url, req, resp)
+            else:
+                json = e.read().decode('utf-8')
+            if e.code == 404:
+                raise ApiNotFoundError(url)
+            if e.code == 403:
+                raise ApiForbiddenError(url)
+            if e.code == 409:
+                raise ApiConflictError(url)
+            raise ApiError(e.code, url)
 
     def _process_resp(self, headers):
         is_json = False
         if headers:
-            for k in headers:
-                h = k.lower()
-                if h=='x-ratelimit-remaining':
-                    self.x_ratelimit_remaining = int(headers[k])
-                elif h=='x-ratelimit-limit':
-                    self.x_ratelimit_limit = int(headers[k])
-                elif h=='x-ratelimit-reset':
-                    self.x_ratelimit_reset = int(headers[k])
-                elif h=='content-type':
-                    is_json = headers[k].startswith('application/json')
+            for h in headers:
+                hl = h.lower()
+                if hl == 'x-ratelimit-remaining':
+                    self.x_ratelimit_remaining = int(headers[h])
+                elif hl == 'x-ratelimit-limit':
+                    self.x_ratelimit_limit = int(headers[h])
+                elif hl == 'x-ratelimit-reset':
+                    self.x_ratelimit_reset = int(headers[h])
+                elif hl == 'content-type':
+                    is_json = headers[h].startswith('application/json')
         return is_json
 
-class _Executable(object):
-
-    def __init__(self, gh, method, path):
-        self._gh = gh
-        self._method = method
-        self._path = path
 
-    def __call__(self, **kw):
-        return self._gh._http(self._method, self._path, **kw)
-
-    def __str__(self):
-        return '_Executable (%s %s)' % (self._method, self._path)
+class JsonObject(dict):
+    '''
+    general json object that can bind any fields but also act as a dict.
+    '''
+    def __getattr__(self, key):
+        try:
+            return self[key]
+        except KeyError:
+            raise AttributeError(f'\'Dict\' object has no attribute \'{key}\'')
 
-    __repr__ = __str__
+    def __setattr__(self, attr, value):
+        self[attr] = value
 
-class _Callable(object):
 
-    def __init__(self, gh, name):
-        self._gh = gh
-        self._name = name
+class ApiError(Exception):
 
-    def __call__(self, *args):
-        if len(args)==0:
-            return self
-        name = '%s/%s' % (self._name, '/'.join([str(arg) for arg in args]))
-        return _Callable(self._gh, name)
+    def __init__(self, code, url, message=None):
+        super(ApiError, self).__init__(message if message else f'{code}: {url}')
+        self.code = code
+        self.url = url
 
-    def __getattr__(self, attr):
-        if attr=='get':
-            return _Executable(self._gh, 'GET', self._name)
-        if attr=='put':
-            return _Executable(self._gh, 'PUT', self._name)
-        if attr=='post':
-            return _Executable(self._gh, 'POST', self._name)
-        if attr=='patch':
-            return _Executable(self._gh, 'PATCH', self._name)
-        if attr=='delete':
-            return _Executable(self._gh, 'DELETE', self._name)
-        name = '%s/%s' % (self._name, attr)
-        return _Callable(self._gh, name)
 
-    def __str__(self):
-        return '_Callable (%s)' % self._name
+class ApiAuthError(ApiError):
 
-    __repr__ = __str__
+    def __init__(self, code, url, message=None):
+        super(ApiAuthError, self).__init__(code, url, message)
 
-def _encode_params(kw):
-    '''
-    Encode parameters.
-    '''
-    args = []
-    for k, v in kw.items():
-        try:
-            # Python 2
-            qv = v.encode('utf-8') if isinstance(v, unicode) else str(v)
-        except:
-            qv = v
-        args.append('%s=%s' % (k, urlquote(qv)))
-    return '&'.join(args)
 
-def _encode_json(obj):
-    '''
-    Encode object as json str.
-    '''
-    def _dump_obj(obj):
-        if isinstance(obj, dict):
-            return obj
-        d = dict()
-        for k in dir(obj):
-            if not k.startswith('_'):
-                d[k] = getattr(obj, k)
-        return d
-    return json.dumps(obj, default=_dump_obj)
+class ApiForbiddenError(ApiError):
+    ' 403 Error '
 
-def _parse_json(jsonstr):
-    def _obj_hook(pairs):
-        o = JsonObject()
-        for k, v in pairs.items():
-            o[str(k)] = v
-        return o
-    return json.loads(jsonstr, object_hook=_obj_hook)
+    def __init__(self, url):
+        super(ApiForbiddenError, self).__init__(403, url)
 
-class ApiError(Exception):
 
-    def __init__(self, url, request, response):
-        super(ApiError, self).__init__(url)
-        self.request = request
-        self.response = response
+class ApiNotFoundError(ApiError):
+    ' 404 Error '
 
-class ApiAuthError(ApiError):
+    def __init__(self, url):
+        super(ApiNotFoundError, self).__init__(404, url)
 
-    def __init__(self, msg):
-        super(ApiAuthError, self).__init__(msg, None, None)
 
-class ApiNotFoundError(ApiError):
-    pass
+class ApiConflictError(ApiError):
+    ' 409 Error '
 
-class JsonObject(dict):
-    '''
-    general json object that can bind any fields but also act as a dict.
-    '''
-    def __getattr__(self, key):
-        try:
-            return self[key]
-        except KeyError:
-            raise AttributeError(r"'Dict' object has no attribute '%s'" % key)
+    def __init__(self, url):
+        super(ApiConflictError, self).__init__(409, url)
 
-    def __setattr__(self, attr, value):
-        self[attr] = value
 
 if __name__ == '__main__':
     import doctest
     doctest.testmod()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `githubpy-1.1.0/setup.py` & `githubpy-2.0.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from distutils.core import setup
-import sys
+import setuptools
 
 import github
 
-kw = dict(
+setuptools.setup(
     name = 'githubpy',
     version = github.__version__,
-    description = 'Github v3 API Python SDK',
-    long_description = open('README', 'r').read(),
+    description = 'Github REST API Python3 SDK',
+    long_description = 'githubpy is a simple Python3 client for GitHub REST API.',
     author = 'Michael Liao',
     author_email = 'askxuefeng@gmail.com',
     url = 'https://github.com/michaelliao/githubpy',
     download_url = 'https://github.com/michaelliao/githubpy',
     py_modules = ['github'],
+    python_requires = '>=3.5',
+    install_requires = [],
     classifiers = [
         'Development Status :: 5 - Production/Stable',
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
-        'Programming Language :: Python',
+        'Programming Language :: Python :: 3',
         'Topic :: Internet',
         'Topic :: Software Development :: Libraries :: Python Modules',
-    ])
-
-setup(**kw)
+    ]
+)
```

