# datasets
# doc 1
memory usage: 21.1+ GB 
['CUSTOMER_ID', 'READING_DATETIME', ' CALENDAR_KEY', ' EVENT_KEY', ' GENERAL_SUPPLY_KWH', ' CONTROLLED_LOAD_KWH', ' GROSS_GENERATION_KWH', ' NET_GENERATION_KWH', ' OTHER_KWH']
->
*pivoted version*
Index: 42228 entries, 2011-10-06 12:30:00 to 2014-03-04 08:00:00
Columns: 13735 entries, 8143479 to 11590456
dtypes: float32(13735)
memory usage: 2.2+ GB

# doc 2  
LCLid                MAC000002  MAC000003  ...  MAC005567
DateTime     

DatetimeIndex: 39727 entries, 2011-11-23 09:00:00 to 2014-02-28 00:00:00
Columns: 5531 entries, MAC000002 to MAC005567
dtypes: float32(5531)
*Data in Kwh/hh(half an hour)*
                                                    
# doc 3
*2014*
['Time', 'Apt1',..., 'Apt114'] except Apt[1, 3, 6, 112, 113, 21, 65, 94]
RangeIndex: 8216 entries, 0 to 8215
Columns: 107 entries, Time to Apt114
dtypes: datetime64[ns](1), float32(106)
memory usage: 3.4 MB

*2015*
['Time', 'Apt1',..., 'Apt114']
RangeIndex: 56699 entries, 0 to 56698
Columns: 115 entries, Time to Apt114
dtypes: datetime64[ns](1), float32(114)
memory usage: 25.1 MB

*2016*
['Time', 'Apt1',..., 'Apt114']
RangeIndex: 503760 entries, 0 to 503759
Columns: 115 entries, Time to Apt114
dtypes: datetime64[ns](1), float32(114)
memory usage: 222.9 MB

# doc 4
all three :
RangeIndex: 12890736 entries, 0 to 12890735
Data columns (total 6 columns):
 #   Column                Dtype         
---  ------                -----         
 0   Customer              int64         
 1   Generator Capacity    float32       
 2   Postcode              int64         
 3   Consumption Category  object        
 4   Consumption           float32       
 5   DateTime              datetime64[ns]
dtypes: datetime64[ns](1), float32(2), int64(2), object(1)
memory usage: 491.7+ MB
-> pivoted : all three :
atetimeIndex: 17520 entries, 2012-07-01 00:00:00 to 2013-06-30 23:30:00
Columns: 300 entries, 1 to 300
dtypes: float32(300)
memory usage: 20.2 MB
Customer                  1         2         3    ...     298     299       300
DateTime                                           ...