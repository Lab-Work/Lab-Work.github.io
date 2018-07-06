---
key: "rail_eta"

order: 2

name: "Estimating arrival times on freight railroads using machine learning"

description: "<p>Numerous methods exist by which to estimate the arrival times (ETAs) of freight trains. Many have been applied to passenger rail, particularly in Europe. But few have investigated the predictability of freight railroads in the United States with large amounts of historical data. Using a dataset from CSX Transportation, we applied machine learning regression techniques on a rich feature set. The features mined from historical railroad operational data included train characteristics, crew information, and network state information.</p>
<p>The dynamics of train operations across route segments is very complex and varied due to numerous factors including topography, locations of passing sidings, and locations of intermediate yards. For this reason, independent regression models were built for a series of discrete points across each route segment. The intuition behind this modeling decision is that the factors contributing to ETA prediction change as the train completes its route. This hypothesis is supported if significant changes are observed in regression feature weights between independent models.</p>
<p>The methodology was tested on sections of the railroad with notoriously varied and unpredictable behavior. ETA predictive performance was compared to that of simple statisitcal methods, which are used in some prediction systems on the railroad. Results showed a consistent 20-30% improvement in prediction accuracy (mean average error) at the beginning of route segments.</p>
<p>Feature weights did indeed change significantly between various regression models on the same route segment. In fact, difficult topographical areas were even identifiable by increased feature weight observed for train tonnage and length.</p>"

funding: "Roadway Safety Institute, the University Transportation Center for US- DOT Region 5"

students: "Will Barbour"

publications: "<li>W. Barbour, J. C. Martinez Mori, S. Kuppa, D. Work. \"Estimating Arrival Times for US Freight Rail Traffic.\" <em>Transportation Research Part C: Emerging Technologies</em>, 2018. <strong>Download: </strong><a href='https://www.dropbox.com/s/ojet2nbntvfeo54/Barbouretal2017.pdf?dl=0'>preprint</a>.</li>
<li>W. Barbour, J. C. Martinez Mori, S. Kuppa, D. Work. \"Predicting Delay Occurrence at Freight Rail Sidings.\" <em>Proceedings of Transportation Research Board Annual Meeting, 2018</em> (to appear).</li>
<li>W. Barbour, S. Kuppa, and D. Work. \"Supporting Automated Operations with Improved Arrival Time Predictions on US Freight Railroads.\" <em>in Proceedings of the the ITRL Conference on Integrated Transport, Stockholm, Sweden</em>, 2016. <strong>Download: </strong><a href='https://www.dropbox.com/s/ojet2nbntvfeo54/Barbouretal2017.pdf?dl=0'>preprint</a>.</li>"

image: /images/route_feature_weights.jpg
---
