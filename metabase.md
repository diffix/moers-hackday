# Accessing Moers traffic data through Metabase

The URL is [metabase.open-diffix.org](https://metabase.open-diffix.org/)

Login with:

Username: `participant@moershackday.de`

Password: `moershackday2022`

We have provided two ways to access the Moers traffic data. One is anonymized with Diffix, and the other provides direct access with no anonymization. In the metabase installation, they are:

| Database name | |
| --- | --- |
| __Moers Hackday__ | Anonymized with Diffix |
| __Non-anonymized Moers Hackday__ | Not anonymized |

All of the features of Metabase, including query building with the GUI, are available with the __Non-anonymized Moers Hackday__ data set. We make this dataset available to allow participants to compare Diffix data quality with non-anonymized.

The GUI query builder of Metabase does not work well with Diffix. Therefore queries need to be built with SQL. It is not obvious how to find the SQL query editor in Metabase, so the following shows you how.

## Visual guide to finding the SQL editor

After login, you should see a page like this. We have prepared a small number of example queries. You can find the list by selecting the `Beispielabfragen` link under `Sammlungen` (see red arrow):

<img src="images/seq10.png" width="600">

(Note that you can change the interface language by clicking on the gearbox on the lower left, clicking "Admin settings", and then "Localization".)

Select any of the listed example queries.

<img src="images/seq11.png" width="600">

Open the editor by clicking `ÖFFNE EDITOR`.

<img src="images/seq12.png" width="600">

It is handy to see the column names as you write queries. To do this, click on the icon shown here:

<img src="images/seq13.png" width="600">

Modify this query or one of the other examples.

<img src="images/seq14.png" width="600">

Alternatively, you can always start a new query from scratch by clicking `New` on the upper right corner:

<img src="images/seq1.png" width="600">

Click on 'New' in the upper right corner (see red arrow) to get this pulldown menu:

<img src="images/seq2.png" width="600">

After clicking "SQL Query" you'll see this:

<img src="images/seq3.png" width="600">

Select the dataset you want to work with ("Moers Hackday" or "Non-anonymized Moers Hackday"), and this will give you the SQL editor.  It is handy to see the column names as you write queries. To do this, click on the icon shown here:

<img src="images/seq4.png" width="600">

Write your query and execute:

<img src="images/seq5.png" width="600">

The "visualize" button at the bottom lets you visualize your result.

<img src="images/seq6.png" width="600">
