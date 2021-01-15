# Wireless Handover Experiment
This is the demonstration of handover progress via a simplified wireless network. There are 3 nodes in the network: 1 user (STA) and 2 access point (AP1 & AP2). 


## Frame format
  <br>|Node Type|ID|Frame Type|Frame Body|Status|Odd Check
 ----|----|----|----|----|----|----
 Length(bits)|2|1|1|3|1|1
 AP1|0|0|0: Command<br>1: Data||0: Wrong<br>1: Correct|
 AP2|0|1|0: Command<br>1: Data||0: Wrong<br>1: Correct|
 STA|1|0: AP1<br>1: AP2|0: Command<br>1: Data||0: Wrong<br>1: Correct|

- Control Frame Body
    <br>|AP|STA
    ---|---|---
    001|Connect|Connect
    010|Disconnect|Disconnect