\`**\# How to Set Up, Run, and Submit Your Code**

*\_This file contains instructions for what software you need to run the assignment, how to set up the code for this assignment, and how to submit your code\_*

**\#\# Installation Instructions**

**\#\#\# Prerequisites**

*\_Provided are instructions for Mac OS X and Linux; if you're on Windows, we recommend you use the Windows Subsystem for Linux (WSL) and follow the Linux instructions.\_*

1\. Make sure you have Python 3 installed.

\- If you are using Linux or WSL in Windows, use the following \[instructions\]([https://www.digitalocean.com/community/tutorials/how-to-install-python-3-and-set-up-a-programming-environment-on-an-ubuntu-20-04-server](https://www.digitalocean.com/community/tutorials/how-to-install-python-3-and-set-up-a-programming-environment-on-an-ubuntu-20-04-server)).  
\- If you are on Mac OS X, first make sure you have \[Xcode\]([https://developer.apple.com/xcode/](https://developer.apple.com/xcode/)) installed. Next, install the Xcode command line tools using the following command \`xcode-select \--install\`. Then, use the following \[instructions\]([https://opensource.com/article/19/5/python-3-default-mac](https://opensource.com/article/19/5/python-3-default-mac)) on making Python 3 the default Python environment.

2\. Install \[Git\]([https://git-scm.com/book/en/v2/Getting-Started-Installing-Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)).

**\#\#\# Microblog**

*\_All starter code for all of the assignments is available through the LMS.\_*

1\. Download the assignment's starter code from the LMS.

2\. Change the directory into the start code example directory.

3\. Create and activate a virtual environment for Python. This should be run in your terminal.

\`\`\`sh  
python3 \-m venv venv && source venv/bin/activate  
\`\`\`

4\. Install the required Python dependencies.

\`\`\`sh  
pip3 install \-r requirements.txt  
\`\`\`

5\. Setup the database for the Flask service.

\`\`\`sh  
flask db upgrade && flask translate compile  
\`\`\`

6\. Run the flask application.

\`\`\`sh  
python3 \-m flask run  
\`\`\`

7\. Verify you can access the application using your web browser by navigating to the microblog at: \[[http://127.0.0.1:5000/\](http://127.0.0.1:5000/)](http://127.0.0.1:5000/]%28http://127.0.0.1:5000/%29).

**\#\#\# Code Submission Instructions**

To package your code for submission to the TechBridge LMS, do the following:

1\. Change into the starter code directory, where you have made modifications to complete the assignment.

2\. Run the following command in your terminal:

\`\`\`sh  
make zip  
\`\`\`

This should produce a zip file called \`assignment.zip\` containing your assignment. You will need to do this every time you make a modification to your code before you submit to the LMS, to ensure it contains your most recent changes. Please use this command instead of making your own zip file, as this command excludes dependencies that, if included, would cause the zip file to be too large for the LMS submission system.

3\. Upload \`assignment.zip\` to the LMS.