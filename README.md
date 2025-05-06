# cs455-project-2-solved
**TO GET THIS SOLUTION VISIT:** [CS455 Project 2 Solved](https://www.ankitcodinghub.com/product/cs455-project-2-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;96329&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS455 Project 2 Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 0px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
&nbsp;

Objective

In this project you will combine many cloud and local resources to build a solution where some of its parts run in the cloud and others run on local premises. This is referred to as “hybrid architecture”.

Overview

To get started, let’s review the architecture of Project1 (Figure 1) and point out how a hybrid architecture differ from it.

Figure 1: Design diagram from Project1.

In Project1, all the resources of the CDC are cloud components: S3, the Lambda, and the database. There are many reasons that this might not always be the case. For example, the CDC might already have a database running on premise and it wants to use this database to save vaccination data. That is, it does not want to create a second database in the cloud and, instead, prefer to use the existing one they have. There might be several reasons why having their database in the cloud is not a possible option. Here are a few possible reasons (but there can be many more):

<ol>
<li>a) &nbsp;There are other legacy applications that are running on premise that use the database. Putting it in the cloud breaks these applications or require major design changes to update them to work with a cloud database.</li>
<li>b) &nbsp;The CDC might be worried about security issues and would like to keep their data on their local network.</li>
<li>c) &nbsp;There might be country regulations that prohibit certain industries from saving data in the cloud.</li>
</ol>
</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
<ol start="4">
<li>d) &nbsp;The CDC does not want to spread its data in multiple locations (some on premise and some in the cloud). It prefers to centralize them in one place.</li>
<li>e) &nbsp;Their IT team has invested resources, money, and expertise in tuning and maintaining the database and they want to leverage this.</li>
<li>f) &nbsp;There are disagreements among the different teams and pushbacks from their developers who are not familiar with cloud programming. The CDC wanted to hire a consulting company to do the cloud work. Their developers are worried about the security of their jobs and are against bringing an outside consulting company to do the work.</li>
</ol>
If a decision was made to use an on premise database (instead of the RDS one), then the design diagram from Figure 1 will need to be updated to the one shown in Figure 2.

Figure 2: An updated design diagram of the one from Figure 1. In this case, the database is not located in the cloud. Instead, it is installed and running on the local network at the CDC building.

You can see now that not all the components of our hypothetical solution run in the cloud. The S3 bucket and Lambda are still in the cloud. But the database is not. There is also a need of a new component (green box in Figure 2) to facilitate the movement of data from the cloud Lambda to the on premise database. For example, this component can be a Windows service or a Linux daemon running on a local computer at the CDC and listening to data emitted by Lambda. A setup like Figure 2 is an example of a hybrid architecture. Hybrid architectures are very common and widely used.

One way to link cloud resources with local resources is to use a combination of queues and a service as shown in Figure 3

</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column">
Figure 3: Using 2 queues (DownwardQueue and UpwardQueue) and a service to allow Resource A (a cloud component) to retrieve data from a non-cloud resource (database DB on a local network).

The numbers in Figure 3 specify the sequence of execution steps that we list below:

<ol>
<li>Resource A puts a message in the DownwardQueue (JSON with enough data to allow the service to know what to do or what type of information Resource A wants).</li>
<li>The service polls the DownwardQueue (using long-polling) and reads the message.</li>
<li>The service retrieves needed information from the local network resource (e.g., database, file, etc.).</li>
<li>The service puts a message in the UpwardQueue (JSON with the data that Resource A asked for).</li>
<li>Resource A polls the UpwardQueue and reads the message that has the data it needs.</li>
<li>Note that ResourceA doesn’t necessarily have to both put a message in the DownwardQueue and read a message from the UpwardQueue. You can have another resource (say ResourceB), where ResourceA put a message in the DownwardQueue and ResourceB reads the returned message from the UpwardQueue. We will use this methodology in this project.</li>
</ol>
To simplify setup in this project we will assume that the local DB is an XML file that can be queried using XPath.

</div>
</div>
</div>
<div class="page" title="Page 4">
<div class="layoutArea">
<div class="column">
Requirements (Part 1)

The workflow of Project2 is summarized in the diagram of Figure 4.

</div>
</div>
<div class="layoutArea">
<div class="column">
Figure 4: Workflow diagram. Note that red arrows represent event triggers.

<ol>
<li>Medical labs drop patient files in an S3 bucket (3 patient files were given to you: patient1.xml,
patient2.xml, and patient3.xml).
</li>
<li>A lambda function (PatientReaderFunction) is listening to events on the above bucket and extracts the data from such files. There is one missing piece of information that is not in the XML: details of the patient’s insurance policy. This information is only available in the insurance company database (InsuranceDatabase.xml), a file local to the insurance company network.</li>
<li>PatientReaderFunction put a JSON message in the DownwardQueue with the patient ID it read from the XML.</li>
<li>The InsuranceDataService is polling the DownwardQueue for incoming messages (using long- polling – more on that in the Implementation Hints section). When it reads a message, it queries the local database (InsuranceDatabase.xml) to check if the patient has insurance or not. It then deletes the message from the DownwardQueue and responds back by putting a response message (in JSON) in the UpwardQueue. The response should have the patient ID and whether the patient has insurance or not. If the patient has insurance, the policy number and insurance provider should be returned as well.</li>
<li>The second Lambda function (InsuranceDataFunction) is listening via a notification trigger to messages that arrive to the UpwardQueue. When a message arrive, it retrieves it, parses it, and print information to CloudWatch. It should print the following:</li>
</ol>
</div>
</div>
</div>
<div class="page" title="Page 5">
<div class="layoutArea">
<div class="column">
<pre>      Patient with ID xyz has medical insurance
</pre>
or

Patient with ID xyz: policyNumber=aaaaa, provider=bbbbb

where aaaaa and bbbbb are the policy number and insurance provider name, respectively.

InsuranceDataFunction should then delete the message from the UpwardQueue.

6. The service (the blue rectangle in Figure 4 below) should print to a log file the following message every time it reads a message from the DownwardQueue:

Date: Read message: { … JSON of the message … }

And the following every time it posts a message to the UpwardQueue:

Date: Posted message: { … JSON of the returned message … }

Requirements (Part 2)

Create a CloudFormation script to install all the cloud components: the S3 bucket, the two Lambda functions, the S3-to-Lambda event trigger.

Implementation Hints

<ol>
<li>Before you start, study the workflow diagram of Figure 4, understand what each component should do, and where a given component should run (is it a cloud resource or something that should run on premise).</li>
<li>Use UploadData.exe from Project1 to upload XML files to the bucket. Change the UploadData code to remove the tag you add to every file you upload (no need for tags in this case).</li>
<li>You can use any programming language you want.</li>
<li>For XML and JSON parsing, use industry standard ways of parsing.</li>
<li>For queue polling by the InsuranceDataService, use long polling. You can read about short vs. long polling here.
Example how to use long polling in .NET is shown here. You can set WaitTimeSeconds to 20 which is the maximum. For example, here is how a ReceiveMessageRequest can be created with WaitTimeSeconds set to 20:
</li>
</ol>
</div>
</div>
</div>
<div class="page" title="Page 6">
<div class="layoutArea">
<div class="column">
<ol start="6">
<li>After reading and processing a message from the DownwardQueue, InsuranceDataFunction should delete the message from the queue.</li>
<li>Regarding the Service component (shown in dark blue in Figure 4), use Module 16 as a guideline to create and install the service.</li>
</ol>
Requirements (Part 2)

Create a CloudFormation script to install all the cloud components:

<ul>
<li>The S3 bucket</li>
<li>The two Lambda functions.</li>
<li>The two queues</li>
<li>The S3-to-PatientReaderFunctionLambda event trigger.</li>
<li>The UpwardQueue-to-InsuranceDataFunction event trigger.
Refer to the CloudFormation module for help in how to work with CloudFormation.

When you demonstrate your project, you start with nothing in AWS. You should run the CloudFormation script and have it create and configure all the resources listed above.

Grading

Ping me when done. You and I will do a 5-minutes Teams meeting where you demonstrate Part 2 and Part 1 of the project. Ping me only when you have tested your work several times and you are confident that Part 2 and Part 1 are working.

Grading Rubric
</li>
</ul>
<ul>
<li>Part 1 (75 points):

o Workflowworksstart-to-endwithnoerrors(60points).

o Youcanexplainyourcode,answerquestions,anddemonstratethatyouunderstandall

the components and how they interact with each other (15 points). I might ask you to

walk me through your code. I don’t ask all students, but randomly pick a few.
</li>
<li>Part 2 (25 points):
o YouCloudFormationscriptcreatesallcomponentsandneededconfigurations(25 points).
</li>
</ul>
</div>
</div>
</div>
<div class="page" title="Page 7">
<div class="layoutArea">
<div class="column">
Late Presentation Rules

<ul>
<li>2 days late: 25% penalty.</li>
<li>More than 2 days late: not accepted. You will lose the percentage points allocated to this
project.

Cheating Policy

This is an individual project and you should present your own code and work.
</li>
</ul>
<ul>
<li>If I notice unusual resemblance between the codes of two students, both students will get a 0 (the student who gave help and the student who received help).</li>
<li>If you present a working system but you sound not confident in explaining how it works, I usually assume that you didn’t do all of it. You will lose points in this case too.</li>
</ul>
</div>
</div>
</div>
