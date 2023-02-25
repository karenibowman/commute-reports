## Design Considerations

https://developers.google.com/maps/documentation/distance-matrix/usage-and-billing#distance-matrix-advanced
<$200 requests on api = free 
Pricing is at 5.00 USD per 1000, for 25 src & dest in matrix of traffic

Estimated entries < 10.

Morning - refresh from 8:30am - 11:30am every 30 min ( 7 times )
Evening - refresh from 3:30 - 7 ( 8 times )

estimate 16 - 20 calls per day.
Mon-Friday - 5x4= 20 days available

Minumum total cost = 20 * 20 = 400 calls = $2
Maximum free requests / day = 40,000 a mo / 31 days = 1290 calls/day

Within a safe margin; aim for an equivalent of 50 calls per hour (every 1.2 min) or less.

Hard Requirement : Add protection to limit supported calls
Limit 1000/ calls per day & only to IP Address from in-office.

## Auth Considerations

Secret is stored for gmap platforms

