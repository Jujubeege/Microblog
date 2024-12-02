# Microblog: Requirements

## Learning Goals

The learning goals of this assignment are:

1. Identify the sources of requirements from a particular implementation.

2. Evaluate a particular implementation's realization or enforcement of a set of requirements.

## Overview

Requirements typically do not spontaneously appear: they are typically influenced by either a user feature, organizational, or legal requirement. In the case of the metrics involved in Lighthouse, these audits can be traced back to legal standards (e.g., Section 508, WCAG 2, WAI-ARIA.) However, even with this lineage, a question still remains open as to whether the audits properly implement and reflect the legal accessibility requirements that influenced them.

For this assignment, we provide you with the starter code. You should produce a Lighthouse report of the microblog.

From there, you should answer the following questions in a new file called `reflections.txt`:

1. How well does Lighthouse provide coverage for these requirements?

2. What new requirements does Lighthouse satisfy (if any?)

## Installation Instructions

### Prerequisites

_Provided are instructions for Mac OS X and Linux; if you're on Windows, we recommend you use the Windows Subsystem for Linux (WSL) and follow the Linux instructions._

1. Make sure you have Python 3 installed.

- If you are using Linux or WSL in Windows, use the following [instructions](https://www.digitalocean.com/community/tutorials/how-to-install-python-3-and-set-up-a-programming-environment-on-an-ubuntu-20-04-server).

- If you are on Mac OS X, first make sure you have [Xcode](https://developer.apple.com/xcode/) installed. Next, install the Xcode command line tools using the following command `xcode-select --install`. Then, use the following [instructions](https://opensource.com/article/19/5/python-3-default-mac) on making Python 3 the default Python environment.

2. Install [Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git).

### Microblog

_All starter code for all of the assignments is available through the LMS._

1. Download the assignment's starter code from the LMS.

2. Change the directory into the start code example directory.

3. Create and activate a virtual environment for Python. This should be run in your terminal.

```sh

python3 -m venv venv && source venv/bin/activate

```

4. Install the required Python dependencies.

```sh

pip3 install -r requirements.txt

```

5. Setup the database for the Flask service.

```sh

flask db upgrade && flask translate compile

```

6. Run the flask application.

```sh

python3 -m flask run

```

7. Verify you can access the application using your web browser by navigating to the microblog at: [http://127.0.0.1:5000/](http://127.0.0.1:5000/).

8. Audit with Lighthouse in the chrome devTools.

### Code Submission Instructions

To package your assignment for submission to the TechBridge LMS, do the following:

1. Upload your `reflections.txt` to the LMS. Compression should not be required.
