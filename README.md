Download Link: https://assignmentchef.com/product/solved-cmsc203-junit-lab-06
<br>
You will be creating a JUnit Test Class for Gradebook.java, that has been provided for you.

<strong>Task #1:</strong>

<ol>

 <li>Add a getScoreSize() method to the Gradebook class which returns scoresSize;</li>

 <li>Add a toString() method to the Gradebook class that returns a string with each score in scores separated by a space.</li>

</ol>




.

<strong>Task #2:  </strong>Create the Test Class GradebookTester.

<ol>

 <li>Select the setUp and tearDown method.</li>

 <li>Select all of the methods of Gradebook, except for the constructor to create tests for.</li>

</ol>




.

<strong>Task #3:</strong>

<ol>

 <li>In the setUp method of GradebookTester, create at least two objects of Gradebook of size 5. Call the addScore method for each of the Gradebook classes at least twice (but no more than 5 times).</li>

 <li>In the teardown method of GradebookTester, set the two objects of Gradebook to null.</li>

</ol>




<strong>Task #4:  </strong>Create test for the methods of Gradebook:

<ol>

 <li>addScore

  <ul>

   <li>Use the toString method to compare the contents of what is in the scores array vs. what is expected to be in the scores array assertTrue( . . .)</li>

   <li>Compare the scoreSize to the expected number of scores entered, using assertEquals(. . .)</li>

  </ul></li>

 <li>sum</li>

</ol>

<ul>

 <li>Compare what is returned by sum() to the expected sum of the scores entered.

  <ol start="3">

   <li>minimum</li>

  </ol></li>

 <li>Compare what is returned by minimum() to the expected minimum of the scores entered.

  <ol start="4">

   <li>finalScore</li>

  </ol></li>

 <li>Compare what is returned by finalScore() to the expected finalscore of the scores entered. The finalScore is the sum of the scores, with the lowest score dropped if there are at least two scores, or 0 if there are no scores.</li>

</ul>







Example:




As a private member of GradeBookTest:

GradeBook g1;




In setup:

g1 = new GradeBook(5);

g1.addScore(50);

g1.addScore(75);




In teardown:

g1 = null;




in testSum():

assertEquals(125, g1.sum(), .0001);




in testMinimum():

assertEquals(50, g1.minimum(), .001);




in addScoreTest();

assertTrue(g1.toString().equals(“50.0 75.0 ”);





