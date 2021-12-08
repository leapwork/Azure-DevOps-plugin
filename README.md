# Leapwork Integration  
Easily include Leapwork as part of your Azure DevOps pipeline using Leapwork Azure DevOps extension

# More Details 
Leapwork’s completely visual, no-code automation platform makes it easy for business and IT users to automate repetitive processes, so enterprises can adopt and scale automation faster. For rapid results, at lower cost, and requiring fewer specialist resources than traditional automation approaches. 

# Features:
•	Setup and test Leapwork connection in few clicks

•	Run automation flows in your Azure DevOps pipeline

•	Automatically receive results

•	Build status-based results

# A couple of requirements
There are just a few requirements to ensure seamless integration:  
1.	.NET framework 4.5  
2.	Team Foundation Server 2015 Update 1 minimum required.
3.	Agent version 1.83.0 minimum required.

# Installing
You are just one click away from seamless automation. Simply install the extension from Visual Studio Marketplace.  
If you have already installed previous version, delete it first/  
Alternatively, you can install it using gallery extension manager. Here is a small guide for you:
1.	Open extensions manager {hostname}:port/_gallery/manage 
2.	Click "Upload new extension" button
3.	Choose downloaded VSIX-file 
4.	Install extension
5.	Choose Collection
6.	Click Confirm button
7.	Now you are ready to get started/

# Instructions
1.	Azure DevOps: Add build step "Leapwork" to your build definition.   
	Azure DevOps: Add an agent phase and then add task "Leapwork" to this agent phase.  
2.	Enter Leapwork controller hostname or IP-address. 
3.  Enter your Leapwork controller API port, by default it is 9001.  
4.  Enter your API access key. You can find it in Leapwork controller Settings section.  
5.	Enter time delay (in seconds, by default 5 seconds). While schedule is running extension will check schedule state with a specified delay before the schedule is finished.  
6.	Select how the extension should process "Done" status: “Success” or “Failed”.  
7.	Enter JUnit report file name. The default name is "report.xml".  
8.	Enter schedule titles you want to run, each one must be entered from a new line.  
9.	Enter schedule ids, each one must be entered from a new line. Using id is preferable, because schedule title can be changed.  
10.	Azure DevOps: Add Test build step "Publish Test Results" to your build definition.  
	Azure DevOps: Add a task " Publish Test Results " to the previously added agent phase.  
11.	Choose JUnit report format. Enter JUnit report file name. It MUST be the same you've entered in point 5. 
12.	Run your schedule and get results. Enjoy! 
13.	Check build results in a detailed report, which can be found in Build summary  
14.	Download logs if needed.  

# Troubleshooting
- If you catch an error "No such run [runId]!" after schedule starting, increase time delay parameter.

# Screenshots
![ScreenShot](https://github.com/leapwork/Azure-DevOps-plugin/blob/main/images/screen1.png)
![ScreenShot](https://github.com/leapwork/Azure-DevOps-plugin/blob/main/images/screen2.png)
![ScreenShot](https://github.com/leapwork/Azure-DevOps-plugin/blob/main/images/screen3.png)
