# Techlabs
A project in collaboration with local business Pickshare to help them get better understanding about their customers, provide their business partnes with optimal marketing strategies.


Make the code run:
 
- To properly run the code you need to change the location of the .json files (users.json and packages.json)
  These files are in the "Used Data & Results.zip" file in the folder: "Used_json_files"

  Example code:
  <img width="1079" alt="Samplecode" src="https://user-images.githubusercontent.com/84444401/138599641-f603bac3-7a88-4a62-b248-d885ed0394be.png">
  users = pd.read_json('**')      
  ** = path of the users.json file
  
  packages = pd.read_json('***')      
  *** = path of the packages.json file
  
- You can adjust the size of all figures and the text in them with the variables:
  <img width="1065" alt="Samplecode_2" src="https://user-images.githubusercontent.com/84444401/138600309-3158669e-646d-498e-8ead-ab88a1727159.png">
  my_font_size = 10
  
  figure_size = 9
  
  You have to adjust those two values seperately to achieve good figure appearence
  
  ![Cities_have_the_most_order-3](https://user-images.githubusercontent.com/84444401/138600642-a0c771d1-c8cd-4dbc-a5e3-712a4426546b.jpg)
  ![Cities_have_the_most_users](https://user-images.githubusercontent.com/84444401/138600651-480c8c7a-2009-4aef-8283-e5a2ef49ac53.jpg)
  ![packages_per_user-3](https://user-images.githubusercontent.com/84444401/138600744-ddaf923f-a25f-4382-8815-dcb4c7ac4704.jpg)

  
- There are two seperated files which run seperately of each other: 
  - Pickshare_Time_Series_Analysis.ipynb
  
    ![Top_5_most_ordered_senders_by_date-3](https://user-images.githubusercontent.com/84444401/138601180-abe10b84-ee4d-456e-987e-aa8603245b86.jpg)
    ![top_5_most_ordered_senders-5](https://user-images.githubusercontent.com/84444401/138601265-3320118a-b241-4005-94ee-cd1ab2bc43d7.jpg)
    ![Top_5_most_ordered_sorted_by_date](https://user-images.githubusercontent.com/84444401/138601306-f0378b06-333e-49f8-8090-2dcae80e4fb8.jpg)
    ![Top_5_cities_have_the_most_orders](https://user-images.githubusercontent.com/84444401/138601373-ca6cdb14-8fdd-407e-a027-4cfca93958a5.jpg)
    ![Top_5_cities_have_the_most_by_day](https://user-images.githubusercontent.com/84444401/138601432-f722b864-4183-414d-b83a-aeb4c23cc16f.jpg)
    ![Average_processing_time_by_day](https://user-images.githubusercontent.com/84444401/138601427-1393836e-d9ac-473f-9b9e-586bbc4b4d5c.jpg)


  - Pickshare_plz_&_maps.ipynb
  
  The three other files: 
  - old_version.ipynb
  - old_version2.ipynb
  - techlabs_notebook_titanic.ipynb
  
  can be ignored since these are only a backup for the developers



Nice to know
- Any changes in the figures will be saved as .jpg files in the folder "/content" with a resolution of 300dpi after you compile the code 


Futher improvements:

- In the Data Processing section the cleaning_text() function needs futher improvement. The main function right now is to get rid of unknown characters to make the             
  code work. Futher improvements could be to automate this procedur for all kinds of unknown characters and also unify the individual properties to a standart  
  format.

- Make the maps head maps for better visualation.


Known bugs and errors:
- Average processing time:
  There are a lot of missing values an therefore a lot of nonsense data. Because either the starttime is missing or the enddime and therefor the calculation makes no sense. 


Used sources in the code:

- Getting the city list of germany from: 

  https://moduliertersingvogel.de/2017/09/03/german-cities-list/
  https://de.wikipedia.org/wiki/Liste_derSt%C3%A4dte_in_Deutschland
- Getting plz of german cities from:

  https://www.suche-postleitzahl.org/downloads

