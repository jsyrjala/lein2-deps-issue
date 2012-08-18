= Case 1 =

* Disable midje in dev dependencies
* run `lein classpath` and notice clojure version

```clojure
$ lein deps :tree
 [compojure "1.1.1"]
   [clout "1.0.1"]
   [org.clojure/core.incubator "0.1.0"]
   [org.clojure/tools.macro "0.1.0"]
   [ring/ring-core "1.1.1"]
     [clj-time "0.3.7"]
       [joda-time "2.0"]
     [commons-codec "1.6"]
     [commons-fileupload "1.2.1"]
     [commons-io "2.1"]
     [javax.servlet/servlet-api "2.5"]
 [org.clojure/clojure "1.4.0"]
 [ring-mock "0.1.3"]
```

= Case 2 =

* Enable midje in dev dependencies
* run `lein classpath` and notice clojure version

```clojure
$ lein deps :tree
 [compojure "1.1.1"]
   [clout "1.0.1"]
   [org.clojure/core.incubator "0.1.0"]
   [ring/ring-core "1.1.1"]
     [clj-time "0.3.7"]
     [commons-codec "1.6"]
     [commons-fileupload "1.2.1"]
     [commons-io "2.1"]
     [javax.servlet/servlet-api "2.5"]
 [midje "1.3.1"]
   [colorize "0.1.1"]
   [ordered "1.0.0"]
   [org.clojure/algo.monads "0.1.0"]
   [org.clojure/core.unify "0.5.1"]
   [org.clojure/math.combinatorics "0.0.1"]
   [org.clojure/tools.macro "0.1.1"]
   [utilize "0.1.3"]
     [joda-time "2.0"]
 [ring-mock "0.1.3"]
   [org.clojure/clojure "1.2.1"]
```