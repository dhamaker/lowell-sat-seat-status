# Status SAT Seats at Lowell

Create a single page for quickly checking status fo SAT test seats at Lowell High School according to College Board.  The query is run on load and the content is updated.  

Always verify availability on official site [SAT Test Center Search](https://satsuite.collegeboard.org/sat/test-center-search)


## Testing notes

As the latest update, there were no seats available for the upcoming tests.  I have tested the page with an out of state zipcode where seats are available, so I am highly confident that the page will say "AVAILABLE" when the seat availability changes on College Board.

I show the test date, seat availability, and test school name of the first result (the location closest to the requested zipcode).

## About the HTML

Page calls collegeboard's JSON API to shows results for specific dates. It lists the first school for a given zipcode.

It is hardcoded to check for March, May, and June 2024 dates near zipcode 94132. 

To include additional dates, copy the page and edit to request additional dates.
