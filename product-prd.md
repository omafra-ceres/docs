# Intro and Goal
The aim of this product is to provide an end-to-end data management solution for OMAFRA specialists. The goal of this solution is to reduce the amount of time specialists use in generating insights for their clients from as long as a few months to a few days.


# Northstar
How do we know this solution has succeeded? When users report drastically reduced time from data collection to insights generation. The greater the delta in time spent, the more successful this product is. Ideal situation is that insights are generated and transmitted in real time to clients.


# Who is it for?
1. **Specialists** - specialists are the primary users of this application. The will be provided access to enter, upload, export and analyse data using this application
2. **Other potential users (tentative)**
    1. Research partners - might be able to submit data to the platform and view results
    2. Clients (growers, industry etc) - might be able to view visualizations and analyses from a portal


# Why build it?
1. It will create a centralized data store - allowing all specialists access to all the data generated across the department, and thus increasing their data analysis capabilities
2. It will speed up data management and analysis 
3. It will standardize data storage 
4. It will provide the foundation for more advanced data analysis techniques – including machine learning 



# What is it?
## Storage 
A database solution that has the following features
1. Users can create a data structure - detailing the names of the data fields and the type of data they can contain
2. Users can create field types (data objects) from primitives that can be used as field types in creating data structures
3. Users can search within the database for data based on specific parameters. Data searches are not limited to single datasets, or to data they themselves have uploaded
4. Users can manage data within the database with a graphic user interface
5. Users can export data based on specific parameters in formats interoperable by most analysis programs. Data exports are not limited to single datasets, or to data they themselves have uploaded. Data can be exported in two ways:
    1. As a file export e.g. .csv file format
    2. Via authenticated API API
6. Data can be saved on the database in alignment with pre-selected/pre-created data structures either by:
    3. A data entry tool 
    4. A data importation tool
    5. An API


## For Partner and Historical Data
![alt_text](images/image1.jpg "image_tooltip")

A conversion tool that takes historical data and converts it to a data structure as outlined above
1. The user should be able to upload a simple spreadsheet exports (e.g. CSV files) to the database with this tool
2. The user should be able to use the software to identify which columns on the spreadsheet/table contain data for specific fields of the pre-set data structure
3. The tool should be able to import the data and make simple conversions where necessary e.g. date format conversions, address enrichment or degradation etc
4. The tool should be able to identify duplicate data, data that is incompatible with the predetermined data structure, as well as gaps with the data, and flag them for action by the user


## For Novel Data
![alt_text](images/image2.jpg "image_tooltip")

A data entry tool that will allow users submit novel data in line with preset data structures at the point of observation or soon after
1. The tool should be able to provide simple data validation at the point of entry, aiming to eliminate errors in the data stored and used for analysis
2. The tool should be able to download updated data structures from the storage application and present them to users
3. Users should be able to use the tool via
    1. **Mobile** - with a scouting app. This app should have an offline mode for no-bandwidth or low-bandwidth situations
    2. **Web (responsive for mobile)** 


## For External Data (e.g. Weather Data)
_OMAFRA has a team working on building a solution to collect weather data directly. This covers an approach that we would take._


## For Analysis
A tool that allows users set up and run repeated analyses with new data as it is received
1. Users should be able to set up parameters for repeated analyses
2. Users should be able to set triggers for automated analyses
3. Tool should generate visualisations for these analyses exportable in various formats - image (e.g .jpg, .png) or document (e.g. .pdf)

![alt_text](images/image3.jpg "image_tooltip")



# Prioritization
We’re using a scored prioritization framework for products (features) to help determine our development roadmap.
This is not in contrast to the success spectrum earlier developed, but helps support our team in implementation of our development plans in a manner that will drive the most value to users while the solution is being developed, while making the best use of resources.


## Framework
The scoring framework is found below. All metrics are scored on a scale of 0 - 3. An exception is made for dependencies - where the scoring metric scale is 0, 1, 2 and 10.

<table style="width:100%">
  <tr>
   <td></td>
   <td><strong>0</strong></td>
   <td><strong>1</strong></td>
   <td><strong>2</strong></td>
   <td><strong>3</strong></td>
  </tr>
  <tr>
   <td>Impact</td>
   <td>No impact</td>
   <td>Some impact</td>
   <td>Significant impact</td>
   <td>Radical impact</td>
  </tr>
  <tr>
   <td>Users</td>
   <td>No users</td>
   <td>Less than 30%</td>
   <td>Btw 30 & 70%</td>
   <td>Over 70%</td>
  </tr>
  <tr>
   <td>Dependent Apps</td>
   <td>No apps</td>
   <td>Only 1 app</td>
   <td>>=2 apps</td>
   <td>All apps 
   (score of 10 assigned)</td>
  </tr>
  <tr>
   <td>Cost</td>
   <td>Significant cost</td>
   <td>Some cost</td>
   <td>Low cost</td>
   <td>No cost</td>
  </tr>
</table>



## Scoring the Priorities
<table>
  <tr>
   <td></td>
   <td><strong>Entry Tool</strong></td>
   <td><strong>Upload Tool</strong></td>
   <td><strong>External Tool</strong></td>
   <td><strong>Analysis Tool</strong></td>
   <td><strong>Storage Tool</strong></td>
  </tr>
  <tr>
   <td>
      <strong>Impact</strong><br>
      How impactful would this be in respect to delivering on our vision of reducing time spent generating insights?
   </td>
   <td>3</td>
   <td>3</td>
   <td>2</td>
   <td>1</td>
   <td>3</td>
  </tr>
  <tr>
   <td><strong>Users</strong><br>
   What portion of our users would likely go ahead and use this tool immediately after it launched?
   </td>
   <td>2</td>
   <td>2</td>
   <td>3</td>
   <td>2</td>
   <td>3</td>
  </tr>
  <tr>
   <td>
      <strong>Dependency</strong><br>
      How much do other tools require this tool to be built to work? 
   </td>
   <td>1</td>
   <td>1</td>
   <td>1</td>
   <td>0</td>
   <td>10</td>
  </tr>
  <tr>
   <td>
      <strong>Cost</strong><br>
      What is the cost to deliver this? Cost includes man-hours as a proxy for difficulty and effort
   </td>
   <td>0</td>
   <td>1</td>
   <td>2</td>
   <td>1</td>
   <td>0</td>
  </tr>
  <tr>
   <td><strong>Total</strong></td>
   <td><strong>6</strong></td>
   <td><strong>7</strong></td>
   <td><strong>8</strong></td>
   <td><strong>4</strong></td>
   <td><strong>16</strong></td>
  </tr>
</table>


Based on this, our order of development would be:
1. Storage tool
2. External data tool
3. Upload tool
4. Entry and Analysis tools


## User Types
1. **Level 1** - External users
    1. Can enter data into data sets they’ve been given access to by Level 2 or 3 users
2. **Level 2** - Internal users 
    1. Can manage their own data structures
    2. Can manage their own data sets
    3. Can view and duplicate data structures owned by other users
    4. Can view and export datasets owned by other users
    5. Can grant other users access to their datasets to enter new data
3. **Level 3** - Admins
    1. Can do everything on Level 2 
    2. Can upgrade and downgrade user levels
    3. Can suspend users
    4. Can manage global data structures and datasets (i.e. primitives)