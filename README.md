# Data repository

Data repository for the paper entitled "Design and Analysis of Push Notification-BasedMalware on Android"

## Application Source Code

* [Backdoor Application](https://github.com/rymuff/os-app-backdoor)
* [Trigger Application](https://github.com/rymuff/os-app-attacker)

Both of repositories are Android Studio project. Therefore, you can simply build the applications by checking out the projects using Android Studio.

## Evaluation Data

###  Stealthiness of push notification-based malware

#### VirusTotal

* [VirusTotal](https://goo.gl/5vOeuG)

#### SandDroid

* [com.kweisa.backdoor.pdf](https://github.com/rymuff/os-data-availability/blob/master/SandDroid/com.kweisa.backdoor.pdf): Analysis report of our Backdoor app
* [results.txt](https://github.com/rymuff/os-data-availability/blob/master/SandDroid/results.txt): Score results of normal app (from Google) and malicious app
* [malware results](https://github.com/rymuff/os-data-availability/tree/master/SandDroid/malware%20results): Analysis reports of malicious apps

### Execution time

We used 5,000 PINs (or patterns) randomly selected from real datasets of PINs (or patterns), and measured the average execution time (i.e., the average time taken to identify the lock mechanism and crack the password) of the backdoor application after it has been triggered by a push message.

* [results.txt](https://github.com/rymuff/os-data-availability/blob/master/Execution%20time/results.txt): Results of execution time

### Power consumption

[PowerTutor](http://ziyang.eecs.umich.edu/projects/powertutor/) was used to measure the power consumption of the backdoor. To see the impact of the password cracking process only, we compared the power consumption of the backdoor in two different cases; *Changed* and *Not changed*. In *Changed* case, the password is changed for every execution, and thus the password cracking process in the backdoor application is always executed. On the other hand, in *Not changed* case, the password is never changed, and so the only thing the backdoor application does is to show up a notification of the previously cracked password without performing the password cracking process.

* [Power consumption.txt](https://github.com/rymuff/os-data-availability/blob/master/Power%20consumption.txt): Results of power consumption
