# jmeter

# What is Load Testing 

- Load testing is a type of performance testing 
- The testing determines a system's performance according to real-life conditions 
- It confirms if the prsent infrastructure is enough to run the application 
- Checks how much load a system can handle 
- Helps to indenfity the maximum operating capacity of any applications 
- The test idenfities the number of usrs that can work on an application coccurrenly 

# Different Tools for Load Tesing
- Apache JMeter
- WebLoad
- LoadUI 
- LoadRunner
- LeoLoad
- LoadNinja

# What is JMeter

- Apache JMeter
- Opensource & free of charge 
- Used to test load testing functional behavior and measing performance 
- Test applications and other functions 
- (How it works) It can simulate 1000 - 10000 users accessing the website concurrently

# Typical Use Cases for JMeter 

| Name of Use Case | Example Use | Description | Important Notes |
| --- | --- | --- | --- |
| Performance Testing | Testing static and dynamic resources | JMeter tests both static resources (JavaScript, HTML) and dynamic resources (JSP, Servlets, AJAX). It helps identify the maximum number of concurrent users your website can handle. | Test results can be influenced by system resources (CPU, RAM) and network conditions. |
| Load Testing | Simulating multiple user access | JMeter simulates multiple user access to Web services concurrently, helping identify capacity limits and potential bottlenecks. | System resources and network conditions should be considered when interpreting test results. |
| Stress Testing | Finding the maximum load the web server can handle | Stress Testing is used to find the maximum load the web server can handle. When the load goes beyond the limit, the web server starts responding slowly and produces errors. | Stress testing helps identify the breaking point of your system. |
| Server Performance Analysis | Analyzing server performance under high traffic | JMeter is used to identify whether the web application under test can manage high traffic. It also analyzes a server’s overall performance when it is under a lot of strain. | Server performance analysis can help optimize your system for better performance. |
| Non-HTTP Testing | Testing databases or message queues | JMeter can test endpoints that aren't HTTP-based, such as databases or message queues. | JMeter can be used for a variety of testing scenarios, not just HTTP-based applications. |


# Why Use JMeter for Load Testing 
- Free or charge 
- Performance testing of applications
- Platform independent (Java based)
- Customizable
- Recording and playback 
- Community support

# JMeter Installation
(on MacOS X)

```bash
$brew install jmeter
```

# JMeter GUI Simple Load Test

![JMeter-Thread-Group.png](https://github.com/vuhung16au/jmeter/blob/main/JMeter-Thread-Group.png?raw=true)
![JMeter-Listener-Test-Result.png](https://github.com/vuhung16au/jmeter/blob/main/JMeter-Listener-Test-Result.png?raw=true)

# JMeter Commandlines

```bash
$ jmeter -n -t LoadTestLocalhost.jmx -l Loading.csv
```

# Generate JMeter Reports 
```bash
$jmeter -n -t BingLoadTestLocalhostWithVariables.jmx -l BingLoadTestLocalhostWithVariables2.csv -e -o JMeterDashboard/
```

# HTTP(s) Load Testing Basic with JMeter
TODO 

# HTTP Requests Load Test with JMeter 
TODO 

GET/POST 

# Jmeter API Testing
TODO 

# Jmeter Database Testing 
TODO 

# JMeter Variables, Random Number, Functions 
TODO 

# JMeter Logic Controllers
TODO 
# Generate JMeter `jmx` with ChatGPT

The prompt

Write a jmx file for JMeter version 5.6 load test.

JMX file name: LoadTestLocalhost.jmx (in XML format)

Define JMeter variables 
- protocol: http
- servername: localhost
- target URL port: 8000
- main website: / 
- blog post 80: "?p=80"
- blog page 2: "page_id=2"

Target website: 
- http://localhost:8000 

Target URLs
- http://localhost:8000/
- http://localhost:8000/?p=80
- http://localhost:8000/?page_id=2

Requirements 
 - Threads
  + Number of threads: 100
  + Ramp-up period (seconds): 2
  + Loop Count: 10


# JMeter Useful Resources 
1. https://jmeter.apache.org/
2. https://jmeter-plugins.org/
3. https://www.tutorialspoint.com/jmeter/index.htm



