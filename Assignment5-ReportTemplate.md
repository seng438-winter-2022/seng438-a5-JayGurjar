<!-- Output copied to clipboard! -->

<!-----

Yay, no errors, warnings, or alerts!

Conversion time: 0.518 seconds.


Using this Markdown file:

1. Paste this output into your source file.
2. See the notes and action items below regarding this conversion run.
3. Check the rendered output (headings, lists, code blocks, tables) for proper
   formatting and use a linkchecker before you publish this page.

Conversion notes:

* Docs to Markdown version 1.0β33
* Wed Apr 06 2022 15:27:04 GMT-0700 (PDT)
* Source doc: SENG 438 Assignment 1 Report
* Tables are currently converted to HTML tables.

WARNING:
You have 5 H1 headings. You may want to use the "H1 -> H2" option to demote all headings by one level.

----->


<p style="color: red; font-weight: bold">>>>>>  gd2md-html alert:  ERRORs: 0; WARNINGs: 1; ALERTS: 0.</p>
<ul style="color: red; font-weight: bold"><li>See top comment block for details on ERRORs and WARNINGs. <li>In the converted Markdown or HTML, search for inline alerts that start with >>>>>  gd2md-html alert:  for specific instances that need correction.</ul>

<p style="color: red; font-weight: bold">Links to alert messages:</p>
<p style="color: red; font-weight: bold">>>>>> PLEASE check and correct alert issues and delete this message and the inline alerts.<hr></p>


**SENG 438 Assignment 5 Report	**

**Group: (18)**


<table>
  <tr>
   <td>
    Sr.
   </td>
   <td>
    Name
   </td>
   <td>
    UCID
   </td>
  </tr>
  <tr>
   <td>
    1.
   </td>
   <td>
    Ali Siddiqi
   </td>
   <td>
    30092156
   </td>
  </tr>
  <tr>
   <td>
    2.
   </td>
   <td>
    Jay Gurjar
   </td>
   <td>
    30096042
   </td>
  </tr>
  <tr>
   <td>
    3.
   </td>
   <td>
    Kai Wang
   </td>
   <td>
    30002810
   </td>
  </tr>
  <tr>
   <td>
    4.
   </td>
   <td>
    Mohamed Numan
   </td>
   <td>
    30086940
   </td>
  </tr>
</table>


**<span style="text-decoration:underline;">SENG 438 GROUP</span>**

**Introduction**

This lab consists of analyzing test data through reliability assessment tools. We will be assessing failure reliability growth testing and a reliability demonstration chart. We will use C-SFRAT to analyze the sample failure data provided.

**Assessment Using Reliability Growth Testing**

![](Screenshots/CSFRAT1.PNG)

C-SFRAT allowed us to compare the various models with the Model Comparision feature where we could view how each model fits with the failure data. We could decide upon the best model by checking which line is the closest to the failure data input we provide. The following figure displays the correspondence between failure data and the best model that uses the geometric sequence to closely track the data. It is fairly visible that the Geometric and IFR sequence models closely model the failure data when it is calculated with respect to all three parameters.

![](Screenshots/CSFRAT2.PNG)

The following figure shows the relation between Geometric and IFR models between intervals of 2 to 10 and 22 to 26. In the upper interval, IFRGSB tracks the data better compared to Geometric while Geometric tracks data better compared to the IFRGSB model in the lower data interval.

![](Screenshots/CSFRAT3.PNG)

The following figure models the data failure rate of Geometric and IFRGSB using the physical time between the intervals as the parameter. This parameter models the data failure rate the best given the parameters we set. We can observe that the models are more accurate on higher data intervals compared to lower intervals.

![](Screenshots/CSFRAT4.PNG)

This graph reflects the trends from all three parameters. The observed trend is followed as the models are more accurate for higher time intervals. The models do not reflect the failure data at the lower data interval. But the models are decently accurate in intervals 8-14. This graph confirms that the models we choose are accurate as they model the failure data is reflected more clearly.


# **Assessment Using Reliability Demonstration Chart**

![](Screenshots/RDC1.png)

Mentioning the RDC1 figure in the RDC folder. Using a developer and customer risk tolerance of 1 failure for every 10 seconds and also a discrimination ratio of 2, so then the system will get accepted with a Failure Intensity object of 3 failure per second. So the customer and developer need the program to have a max of 1 failure for every 10 seconds. The discrimination ratio shows the quantity of error the calculation accepts and correlates to the area between the acceptance and rejection lines. To be acceptable for developers and customers the software must achieve a  Failure Intensity object of at least 3 failures per second.

![](Screenshots/RDC2.png)

RDC2 figure shows that making Failure Intensity object (FIO) in half. Failure data reset in the continue part of the graph which shows that the FIO data does not pass or fail the risk requirements. Instead, is undetermined because of the permissible error created by the discrimination ratio. For instance, reducing the discrimination ratio, failure data will be rejected in that scenario. 

![](Screenshots/RDC3.png)

The RDC3 figure reflects what happens when FIO is increased by 2 times. The FIO is 6 so it causes the failure data that is a lot more than the acceptance rate. FIO of 6 definitely exceeds customer and developer requirements. 


# **Comparison of Results**

From the plots in part one, an estimation of a failure intensity objective can be drawn. We can see from the plots the least failure is at 0 intervals which are expected and most failures can be seen at the final interval. Given this data, the slope of linear failure intensity is 3.2 = 95/30. We choose the 30th interval since 95 failures are found at the 30th interval. This gives us a rough estimate of the minimum failure intensity objective to ensure the failure data is accepted. In part 2, we calculated the minimum failure intensity objective to accept the failure data was 3, so the result from part 1 which was 3.2 is very close. The approximation included for part 1 is linear and the region in the interval is 18-20.


# **Discussion on Similarity and Differences of the Two Techniques**

Both techniques are different but analyze the failure rates of data provided visually with reference to the expected values. Reliability growth testing allowed us to visualize the entire dataset over the given time range while Reliability Demonstration Chart only allowed us to compare certainly accepted and rejected conditions. Reliability Demonstration Chart is more about showcasing the system’s reliability while Reliability Growth Testing allows us to increase system reliability and shows us where the system lacks overall.


# **Difficulties encountered, challenges overcome, and lessons learned**

SRTAT and the excel sheet were not working as described by the lab handout so C-SFRAT had to be used for part one of the lab. Also, it was not clear what needed to be done in the lab too. 


# **Comments/feedback on the lab itself**

The lab was difficult because the resources mentioned were not working as described by the lab manual. SRTAT not working easily with the csv file provided the program failed to run properly. Also the lack of lab instructions given made the lab hard to do as there was little direction. 

**Teamwork/effort division:**

We decided that half of us would work on part 1 while the other half on part2 so we ended up with a fair division of work. Each team later checked on each other to ensure the other team's parts were satisfactory and we also asked each other questions throughout the process. 
