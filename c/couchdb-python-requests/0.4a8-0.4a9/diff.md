# Comparing `tmp/couchdb_python_requests-0.4a8-py3-none-any.whl.zip` & `tmp/couchdb_python_requests-0.4a9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 20283 bytes, number of entries: 11
+Zip file size: 20299 bytes, number of entries: 11
 -rw-r--r--  2.0 unx      454 b- defN 13-Oct-02 07:22 couchdbrq/__init__.py
 -rw-r--r--  2.0 unx    45805 b- defN 21-Jan-14 15:36 couchdbrq/client.py
--rw-r--r--  2.0 unx     4453 b- defN 17-Mar-29 14:38 couchdbrq/pinger.py
+-rw-r--r--  2.0 unx     4473 b- defN 23-Feb-24 08:03 couchdbrq/pinger.py
 -rw-r--r--  2.0 unx     7046 b- defN 17-Mar-29 14:38 couchdbrq/view.py
 -rw-r--r--  2.0 unx      434 b- defN 13-Oct-02 07:25 couchdbrq/tests/__init__.py
 -rw-r--r--  2.0 unx     9773 b- defN 13-Oct-02 15:17 couchdbrq/tests/client.py
--rw-r--r--  2.0 unx      649 b- defN 23-Feb-23 15:35 couchdb_python_requests-0.4a8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-23 15:35 couchdb_python_requests-0.4a8.dist-info/WHEEL
--rw-r--r--  2.0 unx       59 b- defN 23-Feb-23 15:35 couchdb_python_requests-0.4a8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 23-Feb-23 15:35 couchdb_python_requests-0.4a8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      941 b- defN 23-Feb-23 15:35 couchdb_python_requests-0.4a8.dist-info/RECORD
-11 files, 69716 bytes uncompressed, 18673 bytes compressed:  73.2%
+-rw-r--r--  2.0 unx      649 b- defN 23-Feb-24 08:03 couchdb_python_requests-0.4a9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Feb-24 08:03 couchdb_python_requests-0.4a9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       59 b- defN 23-Feb-24 08:03 couchdb_python_requests-0.4a9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 23-Feb-24 08:03 couchdb_python_requests-0.4a9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      941 b- defN 23-Feb-24 08:03 couchdb_python_requests-0.4a9.dist-info/RECORD
+11 files, 69736 bytes uncompressed, 18689 bytes compressed:  73.2%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: couchdbrq/tests/__init__.py
 Comment: 
 
 Filename: couchdbrq/tests/client.py
 Comment: 
 
-Filename: couchdb_python_requests-0.4a8.dist-info/METADATA
+Filename: couchdb_python_requests-0.4a9.dist-info/METADATA
 Comment: 
 
-Filename: couchdb_python_requests-0.4a8.dist-info/WHEEL
+Filename: couchdb_python_requests-0.4a9.dist-info/WHEEL
 Comment: 
 
-Filename: couchdb_python_requests-0.4a8.dist-info/entry_points.txt
+Filename: couchdb_python_requests-0.4a9.dist-info/entry_points.txt
 Comment: 
 
-Filename: couchdb_python_requests-0.4a8.dist-info/top_level.txt
+Filename: couchdb_python_requests-0.4a9.dist-info/top_level.txt
 Comment: 
 
-Filename: couchdb_python_requests-0.4a8.dist-info/RECORD
+Filename: couchdb_python_requests-0.4a9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## couchdbrq/pinger.py

```diff
@@ -25,47 +25,47 @@
         }
 
         if not options.sync:
             params['stale'] = 'update_after'
 
         db.view('%s/%s' % (entry['design_doc'], entry['view_name']), **params).rows
     except:
-        print "Some errors occured:", sys.exc_info()[1]
+        print("Some errors occured: %s" % sys.exc_info()[1])
 
     return True
 
 def entries(args, options):
     for entry in args:
         if options.verbose:
-            print 'Parsing entry', entry
+            print('Parsing entry: %s' % entry)
 
         u = urlparse(entry)
         server = '%s://%s' % (u.scheme, u.netloc)
         _server = Server(server)
         path = [s for s in u.path.lstrip('/').split('/') if s]
 
 
         design_doc = None
 
         if len(path) == 2:
             database, design_doc = path
             if options.verbose:
-                print "  Single doc entry - %s:%s" % (database, design_doc)
+                print("  Single doc entry - %s:%s" % (database, design_doc))
             doc = _server[database]['_design/%s' % design_doc]
             yield {
                 'server': server,
                 'database': database,
                 'design_doc': design_doc,
                 'view_name': doc['views'].keys()[0],
             }, options
 
         elif len(path) == 1:
             database = path[0]
             if options.verbose:
-                print "  Whole database entry - %s" % (database)
+                print("  Whole database entry - %s" % (database))
 
             rows = [r for r in _server[database].view('_all_docs', startkey='_design/', endkey='_design0', include_docs=True).rows]
 
             for row in rows:
                 if 'views' in row.doc:
                     yield {
                         'server': server,
@@ -73,15 +73,15 @@
                         'design_doc': row.id.split('/')[1],
                         'view_name': row.doc['views'].keys()[0],
                     }, options
 
 
         elif len(path) == 0:
             if options.verbose:
-                print "  Whole server entry"
+                print("  Whole server entry")
 
             for db in _server:
                 rows = [r for r in _server[db].view('_all_docs', startkey='_design/', endkey='_design0', include_docs=True).rows]
 
                 for row in rows:
                     if 'views' in row.doc:
                         yield {
@@ -111,36 +111,36 @@
 
     if not args:
         parser.print_help()
         sys.exit(3)
 
 
     if options.verbose:
-        print 'Initiating pool of %d workers' % (options.threads)
+        print('Initiating pool of %d workers' % (options.threads))
 
     pool = multiprocessing.Pool(options.threads)
 
     result = pool.map_async(pinger, entries(args, options), 1)
 
     if options.verbose:
-        print 'Waiting %d seconds for all jobs done' % options.timeout
+        print('Waiting %d seconds for all jobs done' % options.timeout)
 
 
     result.wait(options.timeout)
 
     if not result.ready():
-        print "Timeout reached, terminating workers"
+        print("Timeout reached, terminating workers")
         pool.terminate()
-        print "Terminated"
+        print("Terminated")
         sys.exit(42)
     else:
         if result.successful():
             if options.verbose:
-                print 'All done'
+                print('All done')
             sys.exit(0)
         else:
-            print "Some errors occured"
+            print("Some errors occured")
             sys.exit(2)
 
 
 if __name__ == '__main__':
     main()
```

## Comparing `couchdb_python_requests-0.4a8.dist-info/METADATA` & `couchdb_python_requests-0.4a9.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: couchdb-python-requests
-Version: 0.4a8
+Version: 0.4a9
 Summary: CouchDB's Python wrapper (using requests library)
 Home-page: https://bitbucket.org/angry_elf/couchdb-python-requests
 Author: Alexey Elfman
 Author-email: elf2001@gmail.com
 License: GPL
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

## Comparing `couchdb_python_requests-0.4a8.dist-info/RECORD` & `couchdb_python_requests-0.4a9.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 couchdbrq/__init__.py,sha256=1av8tQ6a7bw9THOcxIZ4KQbAklB91PhK_JbMPTgnHTI,454
 couchdbrq/client.py,sha256=Shn5r9SdGoKloO6T75ZaBJz8Fy0LkdIRWmLS-LdPKUI,45805
-couchdbrq/pinger.py,sha256=iWysGWDqo1DbNH3tjysU2MOeVRYKjy4dPD9MCTXdrvY,4453
+couchdbrq/pinger.py,sha256=dtGeaUjXvibvehhZtn4Vm8uo1_ex2HMknGO1vVL3PzQ,4473
 couchdbrq/view.py,sha256=a3ZlHs67a8aKuwf4IUFJRbD0R9y0m471VtDDfki6EP4,7046
 couchdbrq/tests/__init__.py,sha256=olti1Y2c2bAbfh4Cm6UEaFdpiyR_NsSCH3Vfu8_Rt4g,434
 couchdbrq/tests/client.py,sha256=3ujZFksHeOBhEtBS3LfRnAxognwIvFwpDmF70q5qDUo,9773
-couchdb_python_requests-0.4a8.dist-info/METADATA,sha256=3rAgBYh11Cyjd7ZiLIG51GHsktEjNXYhjOqDYYXHLWc,649
-couchdb_python_requests-0.4a8.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-couchdb_python_requests-0.4a8.dist-info/entry_points.txt,sha256=tb9TcK_GGjzhclkETmvYOqWP8UwpZD7OnlHUiTSrkz8,59
-couchdb_python_requests-0.4a8.dist-info/top_level.txt,sha256=pjjDFly61na-FsdNUnyqVIzB4CO1xzRH1HN8mODFC2A,10
-couchdb_python_requests-0.4a8.dist-info/RECORD,,
+couchdb_python_requests-0.4a9.dist-info/METADATA,sha256=SjGjHjbLTRfQ6lHaV43azDgOzjMvW89Xic3ocUXQq6o,649
+couchdb_python_requests-0.4a9.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+couchdb_python_requests-0.4a9.dist-info/entry_points.txt,sha256=tb9TcK_GGjzhclkETmvYOqWP8UwpZD7OnlHUiTSrkz8,59
+couchdb_python_requests-0.4a9.dist-info/top_level.txt,sha256=pjjDFly61na-FsdNUnyqVIzB4CO1xzRH1HN8mODFC2A,10
+couchdb_python_requests-0.4a9.dist-info/RECORD,,
```

