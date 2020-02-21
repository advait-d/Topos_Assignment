**Overview:**
We extract data from the website https://en.wikipedia.org/wiki/List_of_United_States_cities_by_population about population in cities in the US, clean the data and store it in a dataframe. Further, we parse through links to each city from the table to get a snippet of information about the city, we are going to use as the summary. The collected data can then be exported to a BigQuery importable csv file.

**Files:**
We have the main.ipynb which is our main code used to extract and clean data. The second file is the output of the code as a .csv file

**Steps to upload data to BigQuery:** 
1. Run the jupyter notebook to create csv file at desired location
2. Go to Google Cloud's BigQuery page from your account
3. Create a Project if there is no project in your account else select the project in which you wish to upload the data
4. Create the data-set if there is no data-set in your project else select the data-set under which you want your data
5. Once the data-set is selected Go-to Create Table
6. In Source Select create table from as - Upload
7. Browse the path where you have exported your CSV file
8. Select File Format as CSV
9. Go-to Table Name and Give the Table the desired name.
10. Go-to Schema => And select the Checkbox under Auto-detect Schema and input parameters
