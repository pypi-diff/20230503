# Comparing `tmp/pendazz-0.0.1.tar.gz` & `tmp/pendazz-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pendazz-0.0.1.tar", last modified: Wed May  3 04:39:52 2023, max compression
+gzip compressed data, was "pendazz-0.0.2.tar", last modified: Wed May  3 05:15:33 2023, max compression
```

## Comparing `pendazz-0.0.1.tar` & `pendazz-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 04:39:52.865784 pendazz-0.0.1/
--rw-rw-rw-   0        0        0      269 2023-05-03 04:39:52.863783 pendazz-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-03 04:39:52.844255 pendazz-0.0.1/pendazz/
--rw-rw-rw-   0        0        0    12637 2023-05-03 04:34:42.000000 pendazz-0.0.1/pendazz/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 04:39:52.862802 pendazz-0.0.1/pendazz.egg-info/
--rw-rw-rw-   0        0        0      269 2023-05-03 04:39:52.000000 pendazz-0.0.1/pendazz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      152 2023-05-03 04:39:52.000000 pendazz-0.0.1/pendazz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 04:39:52.000000 pendazz-0.0.1/pendazz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-03 04:39:52.000000 pendazz-0.0.1/pendazz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 04:39:52.867783 pendazz-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      453 2023-05-03 04:39:43.000000 pendazz-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 05:15:33.741888 pendazz-0.0.2/
+-rw-rw-rw-   0        0        0      269 2023-05-03 05:15:33.741888 pendazz-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-03 05:15:33.732441 pendazz-0.0.2/pendazz/
+-rw-rw-rw-   0        0        0    16212 2023-05-03 05:15:07.000000 pendazz-0.0.2/pendazz/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 05:15:33.739884 pendazz-0.0.2/pendazz.egg-info/
+-rw-rw-rw-   0        0        0      269 2023-05-03 05:15:33.000000 pendazz-0.0.2/pendazz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      152 2023-05-03 05:15:33.000000 pendazz-0.0.2/pendazz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 05:15:33.000000 pendazz-0.0.2/pendazz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-03 05:15:33.000000 pendazz-0.0.2/pendazz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 05:15:33.743885 pendazz-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      453 2023-05-03 05:12:54.000000 pendazz-0.0.2/setup.py
```

### Comparing `pendazz-0.0.1/pendazz/__init__.py` & `pendazz-0.0.2/pendazz/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,14 +7,122 @@
     npuzzle_bfs()
     npuzzle_astar()
     factorial_prolog()
     boxsolver_prolog()
     list_prolog()
     sum_prolog()
     monkey_prolog()
+    classification_12()
+    regression_13()
+    '''
+
+def classification_12():
+    return '''
+    data=pd.read_csv("/content/drive/MyDrive/Re_Car_Purchasing_Data.csv",encoding="ISO-8859-1")
+    data.head()
+
+    X=data.drop(['Customer Name', 'Customer e-mail','Car Purchase Amount'],axis=1)
+    Y=data['Car Purchase Amount']
+
+    from sklearn.preprocessing import LabelEncoder
+    en=LabelEncoder()
+    X['Country'] = en.fit_transform(X['Country'])
+    X
+
+    from sklearn.preprocessing import StandardScaler
+    sc=StandardScaler()
+    X=sc.fit_transform(X)
+    X
+
+    from sklearn.model_selection import train_test_split
+    xtrain,xtest,ytrain,ytst=train_test_split(X, Y, random_state=0)
+
+    model = Sequential()
+    model.add(Dense(6,activation='relu',input_dim=6))
+    model.add(Dense(20,activation='relu'))
+    model.add(Dense(50, activation='relu'))
+    model.add(Dense(1,activation='linear'))
+    model.summary()
+    model.compile(optimizer=tf.keras.optimizers.Adam(learning_rate=0.01), 
+                metrics=[r2_score],
+                loss='mean_squared_error', run_eagerly=True)
+
+    from sklearn.metrics import r2_score
+
+    hist=model.fit(xtrain,ytrain,epochs=50, validation_split=0.2, batch_size=32)
+
+    hist.history.keys()
+
+    plt.plot(hist.history['loss'], label='Training Loss')
+    plt.plot(hist.history['val_loss'], label='Validation Loss')
+    plt.xlabel('epoches')
+    plt.ylabel('Loss')
+    plt.legend()
+
+    ypred=model.predict(xtest)
+
+    r2_score(ytst,ypred)
+    '''
+
+def regression_13():
+    return '''
+    from google.colab import drive
+    drive.mount('/content/drive')
+
+    import numpy as np
+    import pandas as pd
+    import seaborn as sns
+    import matplotlib.pyplot as plt
+    import tensorflow as tf
+    from keras.models import Sequential
+    from keras.layers import Dense
+
+    X=data.drop('target',axis=1)
+    Y=data['target']
+
+    from sklearn.model_selection import train_test_split
+    xtrain,xtest,ytrain,ytest = train_test_split(X,Y)
+
+    xnewtrain,xvalid,ynewtrain,yvalid = train_test_split(xtrain,ytrain)
+
+    model = Sequential()
+    model.add(Dense(13,activation='relu',input_dim=13))
+    model.add(Dense(20,activation='relu'))
+    model.add(Dense(50, activation='relu'))
+    model.add(Dense(1,activation='sigmoid'))
+    model.summary()
+
+    model.compile(optimizer=tf.keras.optimizers.Adam(learning_rate=0.002), 
+                metrics=[tf.keras.metrics.binary_accuracy], 
+                loss=tf.keras.losses.binary_crossentropy)
+
+    hist=model.fit(xnewtrain,ynewtrain,batch_size=32,epochs=100,validation_data=(xvalid,yvalid))
+
+    hist.history.keys()
+
+    plt.plot(hist.history['loss'], label='Training Loss')
+    plt.plot(hist.history['val_loss'], label='Validation Loss')
+    plt.xlabel('epoches')
+    plt.ylabel('Loss')
+
+    plt.plot(hist.history['binary_accuracy'], label='Training Loss')
+    plt.plot(hist.history['val_binary_accuracy'], label='Validation Loss')
+    plt.xlabel('epoches')
+    plt.ylabel('Loss')
+
+    ypred=model.predict(xtest)
+
+    newypred=np.round(ypred)
+    newypred
+
+    from sklearn.metrics import confusion_matrix, classification_report, accuracy_score
+    confusion_matrix(ytest,newypred)
+
+
+    print(classification_report(ytest,newypred))
     '''
 
 def monkey_prolog():
     return '''
     move(state(middle,onbox,middle,hasnot),
         grasp,
         state(middle,onbox,middle,has)).
@@ -29,25 +137,29 @@
         state(P1,onfloor,Z,H)).
 
     canget(state(_,_,_,has)).
     canget(State1):-
         move(State1,_,State2),
         canget(State2).
 
+    
+    query:- canget(state(atdoor, onfloor, atwindow, hasnot)).
+
     '''
 
 def sum_prolog():
     return '''
     sum(0,0).
     sum(N,S):-
         N>0,
         N1 is N-1,
         sum(N1,S1),
         S is N+S1.
 
+    query:- sum(5,S).
     '''
 
 def list_prolog():
     return '''
     len([],0).
     len([_|T],R):-
         len(T,R1),
@@ -55,14 +167,17 @@
 
 
     rev([],[]).
     rev([H|T],R):-
         rev(T,R1),
         append(R1,[H],R).
 
+
+    query:- len([1,2,3,4,5],N) & rev([a,b,c,d],A).
+
     '''
 
 def boxsolver_prolog():
     return '''
     getbox(1).
     getbox(2).
     getbox(3).
@@ -82,25 +197,30 @@
         C\=D,C\=E,
         D\=E,
     box(A,Acolor,_),box(B,Acolor,_),
     box(D,Dcolor,_),box(E,Dcolor,_),
     box(C,_,Csize),box(D,_,Csize),
     box(E,_,Esize),box(B,_,Bsize),
     Esize<Bsize.
+
+
+    query:- owners(E,B,A,C,D).
     '''
 
 def factorial_prolog():
     return '''
     factorial(0,1).
-factorial(N,S):-
-    N>0,
-    N1 is N-1,
-    factorial(N1,S1),
-    S is N*S1.
+    factorial(N,S):-
+        N>0,
+        N1 is N-1,
+        factorial(N1,S1),
+        S is N*S1.
 
+    
+    query:- factorial(5,N).
     '''
 
 def npuzzle_astar():
     return'''
     import numpy as np
 
     n = int(input("Enter the size of the matrix (nxn): "))
```

