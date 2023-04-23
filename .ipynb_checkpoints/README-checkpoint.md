# IDS Analysis

## Executive Summary
To determine what patterns can be seen in network traffic, we are analyzing February 20, 21, 22, and 23 of 2018. This dataset contains the network traffic from the University of New Brunswick servers with details about said traffic and a label showing if it was malicious traffic or not. To get the dataset go to https://www.kaggle.com/datasets/solarmainframe/ids-intrusion-csvLinks. Our goal was to be able to determine how malicious traffic compares to benign traffic, so as to be able to later recognize malicious traffic. 


In our analysis, we had the following findings : 


1) 


2)


3) 


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

## CNN Tester
Mark u useless baboon

## Conclusion 