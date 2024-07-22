# Fullcombinelot
Full Combine Lot KIOXIA
The project contain 5 main python file.
1. convert_csv.py
   - Purpose : Receive trace code csv file from automation team then convert and generate 2 file tracode.csv and C_tracecode.csv_temp
   - WorkFlow : 
2. convert_asc.py
   - Purpose : When MAGNUM machine generate asc file for Full Combine Lot the program convert to a new asc file with trace code get from trace code list C_tracecode.csv_temp.
   - WorkFlow :
     + First check path contain csv files created in the last 1 hour -> if "Yes" -> the process will waiting 60 second then continue processing. If "No" continue processing immediately.
     + Next check new asc file was created in last 1 hour then keep going on processing with asc file.
     + Next check trace code in Database if it is file for Fill Combine Lot or not -> If "Yes" Move file. If "No" keep processing.
     + 
