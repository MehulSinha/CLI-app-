# CLI-app-
CLI app using golang 

A small Ping CLI application for MacOS or Linux. The CLI app should accept a hostname or an IP address as its argument, then send ICMP "echo requests" in a loop to the target while receiving "echo reply" messages. It should report loss and RTT times for each sent message.


It sends an ICMP packet and wait a response. If it receives a response, it calls "echo request" callback. After that, MaxRTT time      passed, it calls "idle" callback. This library needs to run as a superuser for sending ICMP packets when privileged raw ICMP endpoints is used so in such a case, to run go test for the package, please run like a following .

