1.Introduction
===============
This is a Java-based system for analyzing the differences between gene expressions 

1.1 purpose
^^^^^^^^^^^^^^^^^^^^^
According to the genes of the two cell samples input, the related charts can be formed to help the people who need to analyze the samples more easily and easily. 

1.2.Overview
^^^^^^^^^^^^^^^^^^^^^
A simple UI interface is designed to read the gene text document input by the user. According to the gene text, scatter plots are generated randomly. At the same time, coordinates are output from the console.a scatter plot of these genes whose X-axis is ControlSample and Y-axis is KnockOutSample. 

1.3.User Characteristics
^^^^^^^^^^^^^^^^^^^^^^^^^
Biologists or biologists who need to analyze a large number of comparisons between the two groups of genes.

1.4.Network Application of JAVA Language 
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Java programs can acquire images, sounds, HTML documents and text of nodes on the network, and process the acquired resources. For example, Java programs can read the latest data provided by a node at regular intervals and display it in a chart. In programming, the general gentleman forms an object of URL type, and then obtains the resources represented by the object by the corresponding method in Java. Java Applet can get the image directly from the nodes on the network and display it. 

1.5. Terminologies & Abbreviations Explaination
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

1.51.Terminology 
>>>>>>>>>>>>>>>>>
*   *Cells in the experimental group*: Cells cultured under experimental or abnormal conditions.           
*   *Control group cells*: cells cultured under normal conditions            
*   *Differentially expressed genes*: genes with significantly different expression levels between the two samples.           
*   *Upregulation*: If a gene is expressed higher in therapy than in the control group, then the gene is up-regulated. 

1.52 abbreviation           
>>>>>>>>>>>>>>>>>>>
  Logfc-logarithmic variation of gene expression. Log 2 [t/c], where t is the gene expression level of the treatment sample, and C is the gene expression level of the control sample.


2.Functional Requirements
===========================

2.1.Input
^^^^^^^^^^
  A text document submitting genes containing three columns of information (gene_id, ControlSample, KnockOutSample) 

 *text file:*

============            ===================              ====================
gene_id                   Controlsample                     KnockOutSample
============            ===================              ====================
AT1G01010	            1.198558083	                        2.036161827
AT1G01020	            13.75736234	                        13.370796
AT1G01030	            0.833779536	                        0.203616183
AT1G01040	            9.58846466	                        7.126566394
AT1G01046	               0	                             0
AT1G01050	            23.81482799	                        21.10821094
AT1G01060	            0.625334652	                        1.221697096
AT1G01070	            1.719670292	                        0.950208853
AT1G01080	            28.34850421	                        25.24840665
AT1G01090	            58.26034505	                        42.96301455
AT1G01100	            1066.508249	                        1308.030358
AT1G01110	            2.709783491	                        1.425313279
============            ===================              ====================

2.1.Output(Data Analyzing)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 a **table** and a **scatter plot** 

Table Analyzing
>>>>>>>>>>>>>>>>

   The table contains a list of differentially expressed genes with the following format:

===========  =================  =================  =============
gene_id       control_sample     knockout_sample     log_2[FC]
===========  =================  =================  =============
 AT1G01020      13.75736234       13.370796          0.041
===========  =================  =================  =============

  The X-axis is Control, and Y-axis is KnockOut. Replace 'Control' and 'KnockOut',and where the mouse clicks, it shows gene_id. 

Plot Analyzing
>>>>>>>>>>>>>>>



3. Non-functional Requirements
===============================
  It refers to the characteristics that software products must possess in order to satisfy users'business needs, besides functional requirements, including system performance, reliability, maintainability, scalability and adaptability to technology and business. 


3.1. Response Time
^^^^^^^^^^^^^^^^^^^^^
  For the user's experience, the response time should be as small as possible, and the response time should be controlled within half a minute. 

3.2. Aesthetic aspect 
^^^^^^^^^^^^^^^^^^^^^^        
  The interface should be clear and simple, otherwise tedious analysis will cause users to lose patience.
           
3.3. Confidentiality policy
^^^^^^^^^^^^^^^^^^^^^^^^^^^^          
   Data security must be considered. When the system is generated, confidentiality and security should be taken into account ,preventing User Information Leakage ,so that users can use it more safely. 


4.Feasibility analysis 
=======================

4.1.Constraints
^^^^^^^^^^^^^^^^^^^^^
  The system should consider some constraints (such as spatial complexity, version compatibility, etc.) and solve them when it encounters problems. 

4.2.System Development Environment  
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  It is very important to choose a good programming language. Nowadays, facing many programming languages, many people have no choice. We choose Java language in this system. The reason for choosing the Java language is that it can easily separate the interface display from the business logic with its powerful object-oriented function. 


4.3.Technical Feasibility Analysis 
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^          
   The technical feasibility analysis mainly includes four aspects: whether the current technology can support the new system developed; the number and level of new system developers, namely human resources; hardware and software resources. 


5. Change case 
===============           
It is possible to provide a gene library directly without user input, or not just text. 


6.Milestones 
===============          
 1.submit SRS analysis report on **March 27**.          
 #.submission phase results ,May.           
 #.the software application described in my SRS.( Final result ),June 6.


7. Appendices
===============
Implementation of User System Module(temporarily)

8. References 
===============
Format Specification of SRS:
https://www.cnblogs.com/yaoyu126/p/8479740.html


