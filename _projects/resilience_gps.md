---
key: "resilience_gps"

order: 7

name: "Quantifying resilience with coarse GPS data"

description: "<p>What effects do natural disasters have on our transportation infrastructure?  How resilient are our cities to extreme events, and how quickly do they recover?  Our work aims to answer these questions in a way that is low-cost and practical, by analyzing millions of GPS records from taxis equipped with GPS.  In this way, it is possible to determine the pace of traffic (i.e., travel time per mile) between various regions of the city, and detect atypical congestion. Our method is tested using a dataset of nearly 700 million taxi trips from New York City.  We have made the dataset publicly available <a title='Open data' href='/data'>here</a>.</p>
<p>The basic idea is that city traffic conditions follow a fairly periodic pattern.  The figure (left) shows the average pace (travel time per mile) between various regions of the city over the course of three weeks (East of the Hudson, Upper Manhattan, Midtown, and Lower Manhattan).  High travel times are obvious during rush hour each day, especially in the Midtown-to-Midtown trips (M-M).</p>
<p>On a particular day, the traffic conditions may deviate significantly from this expected behavior.  This is usually due to an extreme event such as a natural disaster or bad weather conditions.  Based on this deviation, it is possible to measure how \"usual\" or \"unusual\" the traffic conditions are.  For more information about how this probabilistic computation is performed, see our paper:</p>
<p>Brian Donovan and Daniel B. Work. Using coarse GPS data to quantify city-scale transportation system resilience to extreme events.  presented at the<em> </em><em>Transportation Research Board 94th Annual Meeting, January 2015. </em> <a href='https://www.dropbox.com/s/deruyszudfqrll0/TRB15DonovanWork.pdf'>preprint</a>, <a href='https://github.com/UIUC-Transportation-Data/gpsresilience'>source code</a>.</p>
<p>You can also download the data here:  <a href='http://dx.doi.org/10.13012/J8PN93H8'>http://dx.doi.org/10.13012/J8PN93H8</a></p>
<p>Brian Donovan and Daniel B. Work  &#8220;New York City Taxi Trip Data (2010-2013)&#8221;. 1.0. University of Illinois at Urbana-Champaign. Dataset. <a href='http://dx.doi.org/10.13012/J8PN93H8' target='_blank'>http://dx.doi.org/10.13012/J8PN93H8</a>, 2014.</p>
<p>This <a href='https://www.youtube.com/watch?v=cIACwnqLT5E'>video</a> shows all of the taxi trips during the weeks before, during and after Hurricane Sandy, color coded by their pace.  On the right is a normal week for comparison.  The graph at the top indicates how typical or atypical the traffic conditions are, and indicates that it took over five days for the city traffic network to recover from the storm.</p>
<p>One interesting finding is that travel times are actually lower than expected in many parts of the city during the recovery process.  This indicates a change in the usage of the transportation infrastructure – it is likely that the hurricane caused a decrease in usage.  This is especially true in areas like Lower Manhattan, which experienced severe flooding and power outages.  Another surprising result is observable throughout the city on Wednesday the 31st, when the network is completely congested by people try to return to normal operations. This result  indicates that there is room for further research in the post-disaster process of repopulating the city after an evacuation.</p>"

funding: "National Science Foundation"

students: "Brian Donovan"

publications: "<li>Source Code: <a href='https://github.com/Lab-Work/gpsresilience'>https://github.com/Lab-Work/gpsresilience</a></li>
<li><a href='/data'>2010-2013 NYC Taxi Dataset</a></li>
<li><a href='/data'>2010-2013 NYC Traffic Estimates</a></li>
<li>B. Donovan, J. Lee, and D. Work. \"A high resolution method for quantifying resilience of urban road networks.\" <em>submitted to IEEE Transactions on Intelligent Transportation Systems, 2016. </em><strong>Download:</strong> <em> </em><a href='https://www.dropbox.com/s/d2d2xgfw89p8jg6/DonovanLeeWorkTransITS.pdf?dl=0'>preprint</a>.</li>
<li>X. Guan, C. Chen, and D. Work. \"From Warnings to Awareness and Actions: Insights from Hurricane Sandy.\" <em>submitted to the 2017 Transportation Research Board Annual Meeting</em>, 2016.</li>
<li>B. Donovan and D. Work. \"Empirically quantifying city-scale transportation resilience to extreme events.\" <em>submitted to Transportation Research Part C: Emerging Technologies</em><em>,</em> 2016. <strong>Download:</strong> <a href='https://www.dropbox.com/s/hk4kxosxs0umyx8/DonovanWorkTR-C2016.pdf?dl=0'>preprint</a>.</li>
<li> X. Guan, C. Chen, and D. Work. \"Tracking the Evolution of Infrastructure Systems and Mass Responses Using Publically Available Data.\" <em>submitted to PLOS ONE</em>, 2016.</li>
<li>B. Donovan and D. Work. \"Using coarse GPS data to quantify city-scale transportation system resilience to extreme events.\" <em>presented at the</em> <em>Transportation Research Board 94th Annual Meeting, August 2014. </em><strong>Download: </strong><a href='https://www.dropbox.com/s/deruyszudfqrll0/TRB15DonovanWork.pdf'>preprint</a>, <a href='https://github.com/UIUC-Transportation-Data/gpsresilience'>source code</a> <a href='http://dx.doi.org/10.13012/J8PN93H8'>data</a>.</li>"

image: /images/2943c-color_pace_3weeks.png
---

