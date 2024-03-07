# PeopleBox_Assessment
In the process of transforming the data, several key steps were taken. Initially, the dataset underwent preprocessing to handle missing values by forward-filling them in columns related to compensation, review, and engagement. Additionally, date columns were converted to the datetime format for consistency. 

The transformation process involved iterating through each row of the DataFrame while maintaining dictionaries to track the most recent values for compensation, review, and engagement for each employee. During iteration, the effective date and end date were adjusted based on available data, ensuring consistency across records. Several assumptions were made throughout the process, including interpreting missing values as indicating no change in parameters and inheriting the most recent values for missing periods. 

Moreover, tenure in the organization was calculated relative to the start date of the first employee in the dataset, and the end date for the last record of each employee was set to a far-future date (2100-01-01). Lastly, when replacing values in the DataFrame, it was assumed that specific rows corresponded accurately to the intended rows for modification.

Google Spreadhsheets Link: https://docs.google.com/spreadsheets/d/18Up0Ada5ovg7fF4_06746fFmLr3vP_4rigAfmf8m52A/edit?usp=sharing
DB-Fiddle Link: https://www.db-fiddle.com/f/2VBk7BJpCZK3xVhuLTPgwq/1

