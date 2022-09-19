# performance_Testing using Jmeter

# Steps Of Working Procedure...........

Firstly, I downloaded the Apache JMeter's binary file. Then unzip the file and paste it into the C Drive. For opening the file click on jmeter.bat(C:\apache-jmeter-5.5\bin).

Then create a Test Plan. It's like a container that holds the full project. Then add Thread group into the "Test Plan". A number of threads(users) can be defined in a Thread Group. Each thread simulates a real user requesting to the server under a test.

And then add Request under the Thread Group. The environment is almost okay. Then set url, path, query in the request file.

For visualizing results you can add multiple listeners. Now you can add load(users) in the thread group.

Here, I used four method -------
     1.Post Method
     2.Get Method
     3.Update Method
     4.Delee Mehod.
     
# Report Generate Using Two Commands --------------

=======================keep your jmx file in bin===========create a folder in bin called "report"
jmeter -n -t PracticeJmeter_100.jmx -l report\PracticeJmeter_100.jtl
jmeter -g report\PracticeJmeter_100.jtl -o report\PracticeJmeter_100.html
