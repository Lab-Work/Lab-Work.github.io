---
key: "traffic_performance"

order: 1

name: "Large-scale traffic estimation with performance guarantees"

description: "<p>Despite important advances in computation and sensing, real-time traffic estimation problems are still open to a number of critical issues including: (i) the entire state of the transportation network is too large for the estimators to scale in real time; (ii) few results are available which provide a theoretical analysis of the performance of traffic estimation algorithm, and (iii) the non-observability of the traffic model is inevitable due to the existence of shocks and the sparsity of sensor measurements.</p>
<p>Our work aims at designing scalable distributed traffic estimation algorithms to address issues (i) and (ii) with specific care of issue (iii). Large-scale networks can be partitioned into overlapping local sections, with the traffic density on each local section described by a traffic model on the local state, and estimated by a cheap commodity computer (e.g., an agent).  The main algorithmic challenge is to obtain theoretical bounds on the performance of the estimator, even as the system state switches between observable and unobservable modes. We are also interested in the development of estimation algorithms when with performance guarantees when not all sensor data can be transmitted due to energy and communication costs.</p>"

funding: "National Science Foundation"

students: "Ye Sun"

publications: "<li>Y. Sun and D. Work. \"Online estimation with synthetic measurements under an event-triggered sensor scheduler.\" <em>submitted to the IEEE Transactions on Control Systems Technology</em>, 2016.<em> </em><strong>Download</strong>: <a href='https://www.dropbox.com/s/5fr1u8hnds4fr43/SunWork2016.pdf?dl=0'>preprint.</a></li>
<li>Y. Sun and D. Work. \"Kalman filtering with synthetic measurements under an event-triggered sensor scheduler.\" <em>to appear in the European Controls Conference, June 2016.</em></li>
<li>Y. Sun and D. Work. \"Scaling the Kalman filter for large-scale traffic estimation.\" <em>submitted to the IEEE Transactions on Control of Network Systems, February 2015. </em><strong>Download: </strong>  <a href='https://www.dropbox.com/s/i4pa1lhd09f3dyv/DLKCF_TCNS_extended.pdf?dl=0'>extended version</a>, <a href='https://github.com/yesun/DLKCF'>source code</a>.</li>
<li>Y. Sun and D. Work. \"A distributed local Kalman consensus filter for trafﬁc estimation.\" <em>in Proceedings of</em><em> the IEEE Conference on Decision and Control, pp. 6484–6491, 2014.</em></li>"

image: /images/largescale.png
---
