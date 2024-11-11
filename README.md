# hotel-customer-analysis
On the basis of the customer data, relevant dashboard is created on Excel to understand the revenue patterns of the company.

## Problem Statement
You need to create the following dashboards - Revenue by Source(Column Z) month on 
month, Revenue by Source(Column Z) week on week, Average rate by source month on 
month, Total nights by source month on month. 
Status - N and C means cancelled bookings whereas O means occupied rooms. 

## Approach: 
1. The analysis and preprocessing of the data has been done solely on Power Query. 
This gives the added benefit of automatically updating the ‘Transformed Tables’ and 
the ‘Dashboard’ whenever new data is added on the ‘Raw Data’ Tab. 
Same results can be reciprocated on Power BI since Power BI also uses Power Query 
for data analysis.

3. While exploring the data, I noticed that the revenue on the bookings made at the 
end of a month which were more than a day need to be split into relevant months. If 
a booking of 7 days is made on 31st Jan then only 1 day’s revenue should be included 
in Jan and the remaining 6 days should be considered under Feb’s revenue. Hence, 
Total Revenue = Monthly Revenue – Next Month’s Revenue + Additional Revenue 
(Revenue transferred from previous month to current month) 
Same procedure has been followed to calculate Total Weekly Revenue.

5. Bookings with Status N and C have been excluded from the calculations of Total 
Revenue, Average Rate and Total Nights Booked.  

6. Revenue is 0 where the Rate is mentioned as ‘SRD’. I assumed this must be free stays 
offered by hotels to their loyal members and he

## Inferences: 
1. The first three months are the major Revenue generating months. The bookings 
seem to plummet post the 2nd week of April with an exception in the 2nd week of 
June.
 
3. The Direct Sources along with OTA generated the majority of the hotel bookings 
followed by LNR/Groups/Corporates and then OTA wholesale with the least share. 

4. A similar pattern is observed in the Average Daily Rate of the bookings where the 
Direct bookings proved to be the most profitable source of revenue as the highest 
rate is levied on such bookings. OTA also seemed to be a promising source of revenue 
since it was able to drive bookings during the later months of the year while 
maintaining a good average rate when the bookings from other sources significantly 
slumped. 
