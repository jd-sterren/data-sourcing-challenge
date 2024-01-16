<h1>Data Sourcing Challenge</h1>
<p>
<b>Overview</b><br/>
The goal of this challenge was to use New York Times' API to gather movie reviews. 
The application then sorts out the titles to use in sourcing moving information 
from The Movie Database's API.  Once the data is sourced and formatted, the data 
is ordered by example csv file and then exported to csv file in the output folder.
</p>

<h2>Issues Along the Way</h2>
<p>
While we were given <b><i>lambda st: st[st.find("\u2018")+1:st.find("\u2019 Review")]</i></b> 
to use in pulling the title out of the headline.main column, a slight issue occurred. 
One of the headlines started with <b><i>Review: </i></b> which caused a title to 
be missed because it couldn't be found on TMDB.  The work around used included the 
same lambda function minus Review, leaving a space after \u2019 which also can 
indicate end of quoted title.
</p>
<p>Other issues when trying to compare the csv example to data collected as instructed 
involved missing data fields.  The order of columns wasn't specified but can be done 
if requested.</p>