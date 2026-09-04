# rpa2
exp16
1)sequence 
2)get email list ( give mail id, add filter “Resume”, unread, with attachements,mark as read ,give output to emailist )
3)log message ( “no of messages” + emailist.count.tostring() shd be the msg and log level info ) 
4)For each (emailist download email attachment, email msg - whatever in for each header add a folder to destination path )

exp17
1) sequence 
2)try catch in that add
3) input dialog boxes take name and age 
4) build data table and edit the column names next add 
5) add data row 
New object (){name, cint(age)} give output as dt
6) write csv and message box saying process executed successfully 

In catch 
7)Message box “age is not an integer “

exp 18 
Exp 18) 
Sequence 
2)build data table create two columns name and amt output to data table 
3)for each email and add filter subject to expenditure 
In do 
4)download email attachment 
And email message and be for each’s item name 
Then filter by “.xls”
Give path to save these downloads 

5)assign to excelfile and value id directory.getfiles(previous path)

6) for each 
In -excelfile in body 
7) Use excel file 
Excelfile-current text 
Reference as excel 
In do 
8) read range ( excel.sheet(sheet1))
9) Save to data 
9)for each row in datatable 
Datatable-data
Item name-currentrow 
In body 
Add data row 
Array row-currentrow.item.array
Datatable-datatable 
Then 
10) assign 
Total 
Total+integer.parse(currentrow.item(1).to string ()
After 4 boxes 
Attach to fourth box 
11) add data row 
Arrayrow-{“total expenditure”,total.tostring}
Dtatatable 
12) write csv
Datatable 
Give file path

Emaillist-string 
Excelfile-string[]
Total -int
DTT-datatable 
Datatable -datatable (monthly report scope )
