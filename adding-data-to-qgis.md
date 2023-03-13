# Adding Data to QGIS

Now we'll add our downloaded street tree data to QGIS. if you're a new QGIS user, it might be helpful to start with taking a quick tour of the graphical user interface (GUI). You'll find an [explanation of the parts of the GUI](https://docs.qgis.org/3.22/en/docs/user\_manual/introduction/qgis\_gui.html) on the QGIS Documentation site.

We'll use the ![](https://docs.qgis.org/3.22/en/\_images/mActionDataSourceManager.png) Data Source Manager to import the GeoJSON file you downloaded previously. You'll find the icon for the Data Source Manager in the tool bar.

1. Click the ![](https://docs.qgis.org/3.28/en/\_images/mActionAddOgrLayer.png) Vector icon to open the Vector dialog box.
2. Click the browse button to the right of the **Source** entry box to open your computer's file menu and locate the cherry\_trees.geojson file we downloaded previously.
3. Click the Add button to add the geojson to the map.&#x20;
4. Click the Close button to close the Data Source Manager window.

<figure><img src=".gitbook/assets/datasourcemanager.png" alt=""><figcaption></figcaption></figure>

The resulting map should look something like this:

<figure><img src=".gitbook/assets/Screenshot 2023-03-13 at 3.08.21 PM.png" alt=""><figcaption></figcaption></figure>

Note: QGIS randomly selects colors for visualizing data, so your data will likely be a different color.&#x20;
