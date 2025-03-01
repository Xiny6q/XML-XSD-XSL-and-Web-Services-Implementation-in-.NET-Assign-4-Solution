Download link :https://programming.engineering/product/xml-xsd-xsl-and-web-services-implementation-in-net-assign-4-solution/

# XML-XSD-XSL-and-Web-Services-Implementation-in-.NET-Assign-4-Solution
XML, XSD, XSL, and Web Services Implementation in .NET Assign 4 Solution
Introduction

The aim of this assignment is to make sure that you understand and are familiar with the concepts covered in the lectures, including XML elements, attributes, statements, XML schema, XML validation, XML transformation (XSL), and their classes in .Net FCL. By the end of the assignment, you should have applied these concepts and techniques in creating an XML file, its schema, its style sheet, and have written Web services and an SOA application to process these files.

This is an individual assignment. Each student must complete and submit independent work. No cooperation is allowed, even among the team members for assignment 3. Do not use WebStrar or V–Lab to host your files and services that are shared among your team members. You may use your ASU personal Web site space to host your XML, XSD, and XSL files, see Part I question 4.

Part I Practice Exercises (No submission required)

No submission is required for this part of exercises. However, doing these exercises can help you better understand the concepts and thus help you in quizzes or exams.

1. Reading: Textbook Chapter 4.

2. Answer the multiple choice questions 1.1 through 1.16 of the text Section 4.8. Study the material covered in these questions can help you to prepare for the class exercises, quizzes, and the exam.

3. Study for the questions 2 through 8 in text Section 4.8. Make sure that you understand these questions and can briefly answer these questions. Study the material covered in these questions can help you to prepare for the exam and understand the homework assignment.

4. If you have not activated your file service and personal Web hosting site at ASU, you can activate them at: https://selfsub.asu.edu/apps/WebObjects/ASURITEActivation. Then, you can search for Uploading Your Personal Web page within ASU search page to find the steps of uploading your file. Notice that ASU Personal Web site space hosts files only. It does not host programs such as Web services and Web applications. IIS are not installed.

Part II Assignment/Project Questions (Submission required)

The diagram below shows the structure of the XML file and an instance under this structure. Notice that different shapes of boxes have different meanings.

(.xsd) file. The Web method returns “No Error” or an error message showing the available information at the error point. [20 points]

4.2 Web operation “transformation” takes the URL of an XML (.xml) file and the URL of the XSL file as inputs and generates the HTML file based on the XML and XSL files. The generated HTML file can be stored in a text file or in an .htm (or .html) file. You can also display the file in the GUI of your Web application (question 5). [20 points]

4.3 Web operation “search” takes the URL of an XML (.xml) file and a keyword as input. It returns the node’s information related to the keyword: [20 points] (1) If the node has content, return the first content found. For example, if keyword = title, return

Service-Oriented Computing;

(2) If the node has no content, return all the child node’s names. For example, if keyword = Contact,

return Phone and Office. Note that the attribute is considered a child node too.

(3) If the node is the leaf node, return the parent node name. For example, if keyword = Doe, return

Last.

4.4 Web operation “XPathSearch” takes the URL of an XML (.xml) file and a path expression as input.

It returns the path expression value of the given path. [20 points]

4.5 Web operation “searchWsdl” takes the URL of a wsdl file. It reads the WSDL file as an xml file and returns the list of operation names in the wsdl file. [20 points]

Notice that, for all the questions above, do not place the XSD file as a namespace in your XML file. It may cause an exception to some library classes. The absence of the XSD namespace will not cause a problem with the schema validation, as your validation method will take two parameters as input: the XML file and the schema file.

5. Create a Web site application (ASPX), and add the project into the same “solution” that hosts your web service. In other word, the two projects must be kept in the same solution, in order for the application to call the service running on the development server. The Web site application must provide a GUI, which allows entering the required inputs, such as URLs and keyword, and path, based on the questions that you select. The GUI must have the buttons required to invoke the service operations, depending on the methods that you implement in the previous question, for example,

 The button validates of the XML file against the schema file;

 The button generates the HTML file;

 The button searches by keyword or by path in the XML file.

 The button searches the WSDL file

The application must use the Web service created in question 4 to perform the required processing, and display the return message in the GUI. You can use a textbox, a list box, or a label to display the html file, or display it in a separate page. [20 points]

6. Testing: Based on your selection of the sub questions in question 4, provide test inputs and test results. For example, place the three files: Books.xml, Books.xsd, and Books.xsl, into a Web site and use them to test your program on your .Net development server. Inject an error in your XML file and make sure the validation service can detect the error. For this question, you must submit the test results (inputs and outputs) in screenshots. For example [5 points]

(1) A screenshot of the GUI, including the output of the XML validation displayed in the GUI, with no error and with error message;

(2) A screenshot of the GUI, including the input and output for keyword search; (3) The Books.htm file (or Books.html) file generated.

After testing, make sure you remove these files from the Web site: Make sure the students in the same class will not see your assignment before the submission due date. When the TAs grade the assignment, they will download these from your Blackboard submission and place the files in a different location.

Submission Requirement

All submissions must be electronically submitted to the assignment folder where you downloaded the assignment paper. All files must be zipped into a single file.

For Part 1 submission, zip the files, e.g., Books.xml, Books.xsd, Books.xsl, Books.htm, etc., into a single file.

For Part 2 submission: The complete solution folder with all project files for the service and the application, all files generated, and the screenshot of the testing results in a Word or PDF file. The files that you have submitted in Part 1 must be included in Part 2 submission as well.

Zip all these file into a zip file for submission.

Grading

The TA will grade your program following these steps:

(1) The TA will read your program and give points based on the points allocated to each component, the readability of your code (organization of the code and comments), logic, inclusion of the required functions, and correctness of the implementations of each function.

(2) Compile the code. If it does not compile, 40% of the points given in (1) will be deducted. For example, if you are given 20 points in step (1), your points will become 12 if the program fails to compile.

(3) If the code passes the compilation, the TA will execute and test the code. If, for any reason, the program gives an incorrect output or crashes for any input, 20% of the points given in (1) will be deducted.

Please notice that the TA will not debug your program to figure out how big or how small the error is. You may lose 40% or 20% of your points for a small error such missing a comma or a space!

Late submission deduction guidelines:

 For Part 1 submission, missing the deadline will result in a deduction of 5 points. No late submission for this part will be accepted. The submission folder will disappear after the deadline.

 For Part 2 submission, no penalty for late submissions that are received within 24 hours after the given deadline; and 1% grade deduction for every hour after the first 24 hours.
