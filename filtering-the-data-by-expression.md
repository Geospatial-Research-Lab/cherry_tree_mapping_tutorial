# Filtering the Data By Expression

To see what data we've brought in, right click on Urban\_Forestry\_Street\_Trees in the layer panel on the right had side of the screen and select Open Attribute Table from the pop-up menu. This will open up the layer's attribute table.&#x20;

<figure><img src=".gitbook/assets/Screenshot 2023-03-06 at 4.26.01 PM.png" alt=""><figcaption><p>Right-clicking on a layer will open up a menu where you can select Open Attribute Table.</p></figcaption></figure>

Even if you opted to filter the street tree dataset prior to downloading it from the Open Data DC portal, you'll find that the dataset still includes non-cherry trees. In the image of the attribute table below you can see that the dataset still includes plum trees, also members of the Prunus genus, as well as chokecherries.&#x20;

<figure><img src=".gitbook/assets/Screenshot 2023-03-06 at 4.30.14 PM.png" alt=""><figcaption></figcaption></figure>

Note: The exact rows that you'll have will be different if you're using the complete dataset versus the pre-filtered dataset, but you should have the same column headings as seen above.

We can filter out these unwanted tree types from our dataset by using an expression to select only those rows of data that contain the tree types we want to map. To do this, click on the Select Features Using an Expression icon located in the tool bar of the Attribute Table. This will open the Select by Expression tool window. You can either type in or use the selection list in the center of the window to enter the expression: 'CMMN\_NM' LIKE '% cherry'

<figure><img src=".gitbook/assets/Screenshot 2023-03-06 at 4.35.41 PM.png" alt=""><figcaption><p>Select By Expression tool window with an expression.</p></figcaption></figure>

This expression should return every row where the CMMN\_NM column contains data in the pattern of "any character(s), space, cherry" such as "Yoshino cherry" or "Kwanzan cherry".

Note: You can find out more about building expressions by reviewing the documentation on the righthand side of the Select by Expression tool window when you click on any of the information in the middle column of the tool window, or by reviewing the section on [Interacting with features in the attribute table](https://docs.qgis.org/3.22/en/docs/user\_manual/working\_with\_vector/attribute\_table.html?highlight=select%20expression#id31) in the QGIS user manual.

Once you've entered the expression, click Select features at the bottom right of the window and then Close. You should see your selected rows highlighted in the attribute table as well as a count of selected items listed at the top of the attribute table window.

<figure><img src=".gitbook/assets/Screenshot 2023-03-06 at 4.39.13 PM.png" alt=""><figcaption><p>Example of attribute table after selection by expression.</p></figcaption></figure>

If you look at the attribute table above, you'll notice that some cherry trees that we want, specifically Yoshino and Snowgoose trees, didn't get captured by our expression. We can try again to expand our results. Click on the Deselect All Features From The Layer icon to clear the previous selection before clicking on the Select Features Using an Expression icon to reopen the Select by Expression tool window.

