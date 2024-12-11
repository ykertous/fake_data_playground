Description of the dev datasets : 
Note : These datasets have the format (column names, possible values) of real datasets, but all patients information have been replaced by fake data.


fake_dataset_dev_1.xlsx : 
        MSI Gastric Aigora
- contains a header of metadata from the eCRF,
- has empty rows
- contains missing values flagged by : '','Uk','None',' ', np.nan"

fake_dataset_dev_2.csv
        dev dataset that used to test DOpe
- has problems in column names ('ab Value 1', 'Type of treatmetn','Date of biobsy', 'Smoking history\n'
- all types are objects \n- has dates problems : double dash, /MM/YYYY, DDD/MM/YYY, DD/MMM/YYYY, NA/MM/YYYY
- has different empty values : '' '', '', 'unk', 'N/A','NA', 'None', '.', 'Uk'
- has units when there shouldn't be : for 'Pack Years (PA)' : '50 pks' instead of 50
- in biopsy, variables not mapped (capital letters or not, orthographe)
- outlier at 100 for Lab Value 3
- Lab value 2 : '10:2' instead of '10.2'
- PSA level : date in the middle of floats
- Line of treatment : '/n' 

fake_dataset_dev_3.csv
        Bladder Vienna omics
The dataset is empty of data, just the headers/metadata of the -Omics table

fake_dataset_dev_4.csv
        Bladder Vienna pathology
- NA in the middle of dates 
- x for empty values
- many empty columns
