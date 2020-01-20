# PROJECT REPO FOR SOFTWARE ENGINEERING COURSE
ASHOK: E18CSE029: aj5671@bennett.edu.in
ABHINAV: E18CSE006: ar1576@bennett.edu.in
BHAVYA: E18CSE035: bb3768@bennett.edu.in
SRISHTI: E18CSE181: sv3451@bennett.edu.in

# DATA LEAK DETECTION

To check if any data is leaked, or lost and to check the source of the leakage. We'' use data tunneling on a regular basis.
# DATA TUNNELING

to transfer data in a single space, to keep a cnstant check on the data being transferred. Can be repeated to chech the data loss after each step, which helps to check where we lost the data.
# DARK DATA
Dark data is a type of unstructured, untagged and untapped data that is found in data repositories and has not been analyzed or processed. Basiaclly urequired data, that uses up space.



>>>//
.
>>>//

# Data-Leakage-Detection

Data leakage is an uncontrolled or unauthorized transmission of classified information to the outside. It poses a serious problem to companies.It is essential to discover data leakage as soon as possible, as it poses a serious threat to companies on the scale of going bankrupt. The purpose of this PROJECT is to design and implement a data leakage detection system based on special information retrieval models and methods, and also try removing the dark data. Data is to be stored in .pdf or as an image file.

Dependency Req as of now
..Python/Java
.. Numpy
.. DJango
..if python (pdf dependency)
.. Git
.. Database 
.. Web (we'll use a template)
.. something to mail you the data
.. file generator, or a core level to have a log of all the actions taking place in the app (both Java and Python have app plugins for that)
.. basic nowledge on .jsp setup. (It is a web-based file which has java in it rather than php or nodeJS)

implementing data allocation strategies, that improve the porbability of finding the location of a packet of data, hence detecting where a certain data packet has been leaked. 



# PROBLEM DEF
IN COURSE OF BUSINESS, WE TRANSFER CERTAIN DATA THAT IS PRIVATE TO US, TO A THIRD PARTY SOURSE TO BUILD IT, for example, big league companies like apple give their phone design to foxconn to build the device. In the mean time, online renders are being leaked, and the device comes out aritficially months ahead. OUR GOAL IS TO DETECT LEAKS LIKE THESE. 

# WHAT IT ACTUALLY LOOKS LIKE

  from the ADMIN SIDE
  
                    ADMIN --------> LOGIN -------> DATA
                    
from the USER SIDE
   
                                AGENT_1 --------> LOGIN --------> VIEW DATA
                                AGENT_2 --------> LOGIN --------> VIEW DATA --------> SHARE DATA (SEND A NOTIF TO ADMIN)
                                .
                                .
                                .
                                AGENT_n --------> LOGIN --------> VIEW DATA



ACTIVITY DIAGRAM


                                                                                ADMIN
                                                                                  |
                                                                                  |
                                                                                  V
                                                                         ENTERS CREDENTIALS
                                                                                  |
                                                                                  |
                                                                                  V
                                                                                 AUTH
                                                                                  /\                                                                          
                                                                                 /  \
                                                                                /    \
                                                                               /      \
                                                                              /        \
                                                                             /          |
                                                                          error         |
                                                                                        |
                                                                            selects a file to uploaded
                                                                                        |
                                                                                        |
                                                                                enters private key
                                                                                        |
                                                                        selects which agent to share with
                                                                                        |
                                                                                        /\
                                                                                        \/
                                                                                      /    \
                                                                                      1    2
                                                                                      
                                                                                      1. finds the exact agent which leaks the data
                                                                                      2. creates a probability chart
                                                                                      
                                                                                
