Knowage step-by-step tutorials
=======

The following tutorial is aimed at describing the steps to follow in order to produce your data visualizations with Knowage cockpits, that is the most used Knowage dashboarding component.


Step 1: Set up the environment - Knowage installation
-----------

We are going to exploit the Knowage Installer, that is delivering a Knowage instance with a demo database ("Foodmart" database), many datasets and a comprehensive set of predefined analyses. We will go throught the steps to create similar analyses from scratch; you will have opportunity to play with the predefined demo analyses plus to create your own, being able to make comparisons and to explore possibilities.

More into technical details, the Installer will configure the Foodmart database as a Knowage datasource as an example; refer to the [online Knowage documentation (Configure data sources)](https://knowage-suite.readthedocs.io/en/6.4/administrator-guide/configure-data-sources.html) to learn how to connect Knowage to your databases.

Knowage installer is available for downloading at [link](https://www.knowage-suite.com/site/knowage-download/) [1]. The following video tutorials explain how to install Knowage in Windows and Linux operating systems:

* Knowage installer for Windows at [link](https://www.youtube.com/watch?v=gqBBLOTi07Y&list=PL8aPCaNaefVS7CRSI0cbk9dkGgpS1nyXO&index=3) [2]

[![Watch the video](https://img.youtube.com/vi/gqBBLOTi07Y/mqdefault.jpg)](https://www.youtube.com/watch?v=gqBBLOTi07Y&list=PL8aPCaNaefVS7CRSI0cbk9dkGgpS1nyXO&index=3)

* Knowage installer for Linux at [link](https://www.youtube.com/watch?v=uK_C_bQSAaU&list=PL8aPCaNaefVS7CRSI0cbk9dkGgpS1nyXO&index=2) [3]

[![Watch the video](https://img.youtube.com/vi/uK_C_bQSAaU/mqdefault.jpg)](https://www.youtube.com/watch?v=uK_C_bQSAaU&list=PL8aPCaNaefVS7CRSI0cbk9dkGgpS1nyXO&index=2)

A complete guide to installation is available  in the [online Knowage documentation (Installation guide)](https://knowage-suite.readthedocs.io/en/6.4/installation-guide/index.html).

In order to be able to replicate exactly the steps done in this tutorial, you have to select Highcharts JS charting library option plus to install demo materials. Please read Highcharts JS usage terms carefully before installing it. Be aware that Knowage supplies Chart.js as an alternative charting library.


Step 2: Create your data
-----------

Data are the central point for visualization. After Knowage installation, the next step is to define data access.

Knowage provides different ways to access to data and make them available for visualization. The dataset is the basic object in Knowage that permits that. A dataset is a way to read data from a source and represents the portion of data to be used by one or more analyses.

Knowage users can be divided in technical and final users; those 2 groups have different modalities to create datasets. In the following paragraphs some video tutorials explain how to access data from thecnical user and end user perspectives.

For more detailed explaination please refer to Knowage online documentation linked in the following paragraphs.

### Create your query and file dataset as technical user

Watch the [video tutorial](https://www.youtube.com/watch?v=od8dZHJF3oE&list=PL8aPCaNaefVS7CRSI0cbk9dkGgpS1nyXO&index=4&t=0s) [4] to know how to access data connecting to a database and querying it via SQL or uploading a file.

*KNOWAGE dataset creation (file and query types) by the admin* tutorial on Knowage YouTube channel:

[![Watch the video](https://img.youtube.com/vi/od8dZHJF3oE/mqdefault.jpg)](https://www.youtube.com/watch?v=od8dZHJF3oE&list=PL8aPCaNaefVS7CRSI0cbk9dkGgpS1nyXO&index=4&t=0s)



Due to technical skills needed to write SQL code, the query dataset type is available only for technical users. In the first part of the video tutorial the general dataset configuration are showed with a list of the different dataset types availables in Knowage. For the complete list of datasets that a technical user can create refer to the [online documentation (Advanced Data Access)](https://knowage-suite.readthedocs.io/en/6.4/functionalities-guide/advanced-data-access/index.html).

### Create a metamodel as technical user

A metamodel is the high-level representation of a datamart, it is designed by technical users but the main goal is to allow final users to query the enterprise database using a web drag-&-drop user interface (the Knowage Query by Examples - QbE engine), without the need of SQL expertise.
Whatch the [video tutorial](https://www.youtube.com/watch?v=ueUfgYHT_CA&list=PL8aPCaNaefVS7CRSI0cbk9dkGgpS1nyXO&index=5&t=0s) [5] to see how to create a metamodel.

*Knowage metamodel creation by the admin* tutorial on Knowage YouTube channel:

[![Watch the video](https://img.youtube.com/vi/ueUfgYHT_CA/mqdefault.jpg)](https://www.youtube.com/watch?v=ueUfgYHT_CA&list=PL8aPCaNaefVS7CRSI0cbk9dkGgpS1nyXO&index=5&t=0s)

For further information, please consult the dedicated section in the [online documentation (Meta Web)](https://knowage-suite.readthedocs.io/en/6.4/functionalities-guide/meta-web/index.html).


### Create your file and QbE dataset as end user

The end user can access data in different ways. He can exploit datasets shared by technical users (those datasets are tipically querying enterprise datasources) or CKAN resources, upload his own data or query the metamodels (also created and shared by the technical users) using QbE. The full description of the ways the end user can access data is described in the [online documentation (Basic Data Access)](https://knowage-suite.readthedocs.io/en/6.4/functionalities-guide/basic-data-access/index.html).

Watch the [video tutorial](https://www.youtube.com/watch?v=nQmuRfQaa50&list=PL8aPCaNaefVS7CRSI0cbk9dkGgpS1nyXO&index=5) [6] to have a brief overview on where end user can find data and learn how to:

* create file dataset uploading csv/xls files
* create QbE dataset querying a metamodel

*KNOWAGE dataset creation (file and qbe types) by the user* tutorial on Knowage YouTube channel:

[![Watch the video](https://img.youtube.com/vi/nQmuRfQaa50/mqdefault.jpg)](https://www.youtube.com/watch?v=nQmuRfQaa50&list=PL8aPCaNaefVS7CRSI0cbk9dkGgpS1nyXO&index=5)


Step 3: Create your dashboard
-----------

Once data are linked into Knowage and dataset are created it is time to create the data visualizations. The Knowage tool for easily reaching this goal and create dashboards is the Cockpit engine: it is providing a user-friendly designer where the user selects one or more datasets and uses them to create interactive visualizations, that we call "cockpits". A key aspect is that cockpit and its graphical elements, called widgets, can rely on different datasets of different types at the same time with no differences from the user perspective: this means that it doesn't matter where the datasets are coming from, if the final user created them by his own or if they were created and shared by technical people. Another key aspect is that data coming from different sources can be used simultaneously in the same cockpit.

Create a cockpit as end user or technical user is pretty the same except for some properties that are specific for technical users. The [video tutorial](https://www.youtube.com/watch?v=KtqMyn8fsg8&list=PL8aPCaNaefVS7CRSI0cbk9dkGgpS1nyXO&index=6) [7] shows how to create a cockpit step by step.

*Cockpit creation - Knowage 6.4* tutorial on Knowage YouTube channel:

[![Watch the video](https://img.youtube.com/vi/KtqMyn8fsg8/mqdefault.jpg)](https://www.youtube.com/watch?v=KtqMyn8fsg8&list=PL8aPCaNaefVS7CRSI0cbk9dkGgpS1nyXO&index=6)

For further details concerning single widgets refer to the [online documentation (Cockpit)](https://knowage-suite.readthedocs.io/en/6.4/functionalities-guide/cockpit/index.html).

Notes
-----------
[1]: *KNOWAGE DOWNLOAD - COMMUNITY EDITION* Knowage download page.

[2]: *KNOWAGE How To - Full Knowage installation on Windows* tutorial on Knowage YouTube channel.

[3]: *KNOWAGE How To - Installation on Linux* tutorial on Knowage YouTube channel.

[4]: *KNOWAGE dataset creation (file and query types) by the admin* tutorial on Knowage YouTube channel.

[5]: *Knowage metamodel creation by the admin* tutorial on Knowage YouTube channel.

[6]: *KNOWAGE dataset creation (file and qbe types) by the user* tutorial on Knowage YouTube channel.

[7]: *Cockpit creation - Knowage 6.4* tutorial on Knowage YouTube channel.

How to contribute
-----------
Before start to contribute, please read and sign the [Contributor License Agreement](https://www.clahub.com/agreements/KnowageLabs/Knowage-Tutorials).
The contribution process is based on GitHub pull requests (https://help.github.com/articles/about-pull-requests/).