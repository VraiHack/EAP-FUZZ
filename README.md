# pyfuzz
Mutation Protocol Fuzzing tool developed in python, act like "client" that will send malformed RFC packets (e.g malformed http-get) toward SUT/DUT. 

PyFuzz is a linux tool which use scapy as a principal module. The benefits from PyFuzz is to allow the end user to added more complex test cases depending on the SUT functionality.

pyfuzz responsable to verify the SUT health after the sending of each malformed packets.

#### Please note: pyfuzz will cover other protocols but for the moment pyfuzz focus only on EAPOL/RADIUS fuzzing.

### PyFuzz Funtionality
-------------------------------------------------------------------------------------------------------------------------------
Once you install pyfuzz by following these steps:
```diff
git clone https://github.com/VraiHack/PyFuzz
cd PyFuzz
pip install .
PyFuzz
``` 
1- The user will be asked to choose a Fuzzing protocol and a Fuzzing templates

2- Then, he will be aksed to configure PyFuzz according to the slected template.

3- An interporability check will be done to make sure that SUT respond on valid packet (e2e communciation).

4- If interoporability "passed" the end user will be asked to choose Fuzzing test cases to run.

5- The end user will be reminded to check and verify the health, alarms, status of the SUT during the Fuzz.

### pyfuzz Client Templates Status (release-1)
-------------------------------------------------------------------------------------------------------------------------------
| Protocols | Templates | Readiness | Tested-Verified | Templates-Version | Developer.name |
| --- | --- | --- | --- | --- | --- |
| EAP | EAPOL-MD5 | On-Going | Ubuntu 20.04.5 / Kali 2022.4  | 1.0.0 | VraiHack
| EAP | EAPOL-TLS | Not-Started | ...... | 1.0.0 | NotAssigned
| RADIUS | eap-md5-response | Not-Started | ...... | 1.0.0 | NotAssigned
| RADIUS | client access-response | Not-Started | ...... | 1.0.0 | NotAssigned
| RADIUS | client accounting-response | Not-Started | ...... | 1.0.0 | NotAssigned

release-1: mean only one template ready to use

These days, i am writing a book in HW security beside of my work so i really don't have time to complete this project alone even if i have all the code steps in my head ,concerning other templates but no time to type them.

For that, if you Want to contribute that will be Great, you will learn a lot! Please take a few minutes to [read this](https://github.com/VraiHack/PyFuzz/blob/main/contribute.md)!
