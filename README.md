# IDS Analysis

## Executive Summary
To determine what patterns can be seen in network traffic, we are analyzing February 20, 21, 22, and 23 of 2018. This dataset contains the network traffic from the University of New Brunswick servers with details about said traffic and a label showing if it was malicious traffic or not. To get the dataset go to https://www.kaggle.com/datasets/solarmainframe/ids-intrusion-csvLinks. Our goal was to be able to determine how malicious traffic compares to benign traffic, so as to be able to later recognize malicious traffic. 


In our analysis, we had the following findings : 


1) 


2)


3) 


4)


5) The most common destination port for non-benign events was port 80 (with 188660 attacks), followed by port 500 (with 130 attacks).


6) The most common time for non-benign events to occur was around 2:00 a.m. and 10:00 a.m.


## Finding 1 Analysis - Packets
The average packet length came out to around 80 bytes per packet. However, we did also find that the average packet length for DDoS attacks was 38% less than that of benign traffic. 

The average forward packets in a connection is 6 packets, and the average backward packets is 7 packets. As we compare that to malicious packets, we can see the average total forward packets is significantly higher in malicious attacks at 275, most likely because of DDoS attacks, in comparison with the 6 of benign traffic. The backwords traffic is lower for malicious traffic at 1 per connection average, whereas benign traffic is 7. 

The average forward packet rate per second is around 26,795, and the average backward packet rate per second is around 3,056. When comparing benign and non-benign traffic, we see that the average packet rate per second is higher for benign is higher than malicious. 

## Finding 2  Analysis - Flags
Rate of Occurances

## Finding 3  Analysis - Duration
The average flow duration is around 12,991,373 millaseconds, and in comparison, the benign traffic lasts 4,999,788.76% longer on average than malicious traffic. 

The average idle time in a connection is 5,669,832 millaseconds. The average benign idle time is 1,949.23% longer for that of malicious connections. 

## Finding 4 Analysis - Features
Down/Up Ratio

The average packet count in subflows is forward packets is 35 and 6 in backward packets. The average subflow is significantly more in malicious packets with forward packets, but less in backwards packets. 

The average packet variance in forward packets is around 13, and they are relatively close in variance for both benign and malicious traffic. In backwards packets,  the average is 20 and it is 89.810% less for benign than malicious. 
## Finding 5 Analysis - Destination Port
The two most common destination ports for non-benign events were port 80 and port 500. We further broke down the destination ports by attack category. We found that the most common ports for brute force attacks specifically included 80, 500, 67, 0, and 31808. It should be noted that 67 and 31808 had very little occurences still. When it came to the rest of the categories (DDOS attacks and SQL injections), the only port with occurences was port 80.

## Finding 6 Analysis - Timestamps
The two most common times for non-benign attacks to occurr happened around 2:00 a.m. and 10:00 a.m. We further broke down timestamps for non-benign attacks by attack category. Brute Froce -Web attacks tended to take place between 10:00 a.m. and 11:30 a.m., while Brute Force -XSS attacks tended to take place between 1:00 a.m. and 2:30 a.m. SQL Injection attacks tended to take place around 2:45 a.m. In terms of the DDOS attack categories, the DDOS attack-HOIC category tended to take place between 2:10 a.m. and 2:15 a.m., while the DDOS attack-LOIC-HTTP and DDOS attack-LOIC-UDP categories tended to take place between 10:00 a.m. and 10:45 a.m.

## Convolutional Neural Network
It needed too much memory and took too many tears 🥲

## Conclusion 
