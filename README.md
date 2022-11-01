# RCNJ Course Checker

RCNJ Course Checker works to determine the number of remaining seats available in a course. The script can then either register in the course automatically or simply notify (open the course link).

To minimize the need to install extra modules like mechanize or requests for people who may not be tech-savy, only libraries that are already part of Python's Standard Library are included.

## Usage
The script supports both python 2.7 and python 3.5.

Save the code into a file called CourseChecker.py

You can run the file using either  <code>python rcnjCourseChecker.py</code> or simply right clicking and using the launcher.

Some notes:

* Make sure you enter the section URL, it should look like this: `https://courses.students.ubc.ca/cs/main?pname=subjarea&tname=subjareas&req=5&dept=XXXX&course=XXX&section=XXX`
* Only enter <b>y</b> or <b>n</b>, not yes or no. There's no catching protocol.
* Mac users: If you want to keep your laptop awake until it registers you (or you terminate the process), use: <code>$ caffeinate -i -s python rcnjCourseChecker.py</code>. The screen will turn off but python will keep running.
