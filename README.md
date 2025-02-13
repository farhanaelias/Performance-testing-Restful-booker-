# Performance Testing on Restful-Booker API

This repository contains a performance testing report for the Restful-Booker API (https://restful-booker.herokuapp.com/). 

The tests were conducted using Apache JMeter, a popular open-source tool for load testing.

 # Test Overview

Tool Used: Command-line performance testing tool (Apache JMeter)

API Tested: Restful-Booker API

Report Format: Interactive HTML Dashboard

Test Objective: Measure response time, throughput, and overall performance under load.


# Test Plan
Testplan > Add > Threads (Users) > Thread Group

Number of Threads (user): 100

Ramp-Up Period (in seconds): 10

Loop Count: 1

# Test execution (from the Terminal)

JMeter should be initialized in non-GUI mode.

Make a report folder in the bin folder.

Run Command in jmeter\bin folder.

# List of API

auth

createBooking

getBooking

updateBookingByPut

UpdateBookingByPatch

deleteBooking

# for jtl file

jmeter -n -t performance-testing.jmx -l report\performance-testing.jtl

# for html file

jmeter -g report\performance-testing.jtl -o report\performance-testing.html


# Key Metrics in the Report

APDEX Score: Application Performance Index to assess user experience.

Requests Summary: Breakdown of API requests and their response times.

Throughput Analysis: Number of requests processed per second.

Error Analysis: Logs of failed requests with details.

# Observations

The API performs well under 100 concurrent users. 

# Number of Threads 100 ; Ramp-Up Period 10s

![image](https://github.com/user-attachments/assets/1dee9121-a635-4899-81b4-12cf2db5b4b4)

![image](https://github.com/user-attachments/assets/7ce88f4d-2c49-4e9d-8e1e-fe6a2364bf6d)

![image](https://github.com/user-attachments/assets/42e01960-f581-48c7-9614-385841275914)

![image](https://github.com/user-attachments/assets/07faa5c4-389e-47ce-9098-27c525d55b21)



