# User Guide #

**A. Use the sample webapp application**

1) Open Sample webapp project

2) Edit dspace.cfg file and fill all the necessary information, that is:

> a) dspace.dir: the full path to the dspace.cfg file

> b) dspace.url

> c) dspace.name

> d) db.name

> e) db.url

> f) db.driver

> g) db.username and finally

> h) db.password

3) Edit file classes/classifier.beans and fill in the configFile property of the bean "dataLoader"

4) Place webapp in a servlet container (eg. Tomcat)

5) Use the well known ListRecords verb of OAI-PMH protocol to harvest data

............

**B. Develop new data loaders for legacy data sources**

1) Like DSpaceDataLoader, develop a new DataLoader by extending class "DataLoader" of the Biblio Transformation Engine library

2) Edit file classes/classifier.beans so as to include your own data loader in the spring context

3) Enjoy!