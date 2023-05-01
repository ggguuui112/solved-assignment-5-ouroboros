Download Link: https://assignmentchef.com/product/solved-assignment-5-ouroboros
<br>
<h1>1.Objective</h1>




The main purpose of this assignment is to have you all become familiar working with custom data structures that are programmer defined. In class, it has already been established that this is a huge benefit in the sense that it allows for a high degree of flexibility in how things can be approached and accomplished. This also serves as good practice in understanding how to handle and keep track of object references, which is key in the successful completion of this assignment.







<h1>2.Provided Files</h1>




There will be two Python files that will be needed in the successful completion of this assignment.




The first file is named <strong>node.py</strong>. This file contains the basic class definition for a Node (see Section 3- <strong>Node Class Definition </strong>for further information).




The second file is the usual tester program: <strong>ouroborosTester.py</strong>. More information on the tester program can be found in Section 6- <strong>Testing</strong>.







<h1>3.Node Class Definition</h1>




Recall that, to begin working with a linked list, a Node object must be first defined. Python supports a programming paradigm known as object-oriented programming. Below is the class definition for a Node in a singly linked list:




class Node(object):

def __init__(self, data, next = None):        self.data = data           self.next = next




Please note that you do <strong>NOT</strong> have to include the above class definition of a <strong>Node</strong> within your program. The above definition can be found within the <strong>node.py</strong> Python file.




<strong>IF YOU PLAN ON USING THE CLASS DEFINITION TO TEST YOUR FUNCTIONS WITHOUT THE USE OF THE TESTER PROGRAM:</strong> you will have to import specifically the <strong>Node</strong> class definition. This can be accomplished by including the following line of Python code at the top of your program:




from node import Node

<strong> </strong>

From here, you can create <strong>Node</strong> objects simply by calling the name of the object (i.e. var1 = Node(data) as an example).







<ol start="4">

 <li><strong>Required Functions</strong></li>

</ol>




<h1>insert_and_link(head, data)</h1>

<strong> </strong>

<strong>            Description: </strong>Given the “head” of the Ouroboros data structure, and a piece of data (will always be an integer, and no other kind of data type), create and insert a new Node at the “tail” of the Ouroboros data structure while also linking the newly created Node (which is now the new “tail” of the Ouroboros data structure) to the “head” of the data structure.

<strong> </strong>

<strong>            Output: </strong>This function should not output anything to the screen.

<strong> </strong>

<strong>            Returns: </strong>This function should not return anything.

<strong> </strong>

<strong> </strong>

<h1>remove_and_link(head)</h1>

<strong> </strong>

<strong>            Description: </strong>Given the “head” of the Ouroboros data structure, remove the “tail” of the data structure. When the “tail” Node is removed, ensure to have the new “tail” Node link back to the “head” Node of the Ouroboros data structure.

<strong> </strong>

<strong>            Output: </strong>This function should not output anything to the screen.

<strong> </strong>

<strong>            Returns: </strong>This function should return the data stored within the node to be removed.

<strong> </strong>

<strong> </strong>

<h1>count_nodes(head)</h1>

<strong> </strong>

<strong>            Description:</strong> Given the “head” of the Ouroboros data structure, count every node comprising it up until the “tail” of the data structure is encountered.

<strong> </strong>

<strong>            Output: </strong>This function should not output anything to the screen.

<strong> </strong>

<strong>            Returns: </strong>This function should return the number of nodes that form part of the Ouroboros data structure.

<strong> </strong>

<strong> </strong>

<ol start="5">

 <li><strong>Requirements</strong></li>

</ol>




Your program must be named “ouroboros.py”.







<h1>6.Testing</h1>




The tester program will run a total of <strong>9</strong> test cases: <strong>3</strong> of the test cases will test the <strong>insert_and_link()</strong> function, <strong>3</strong> of the test cases will test the <strong>remove_and_link()</strong> function, and the remaining <strong>3</strong> test cases will test the <strong>count_nodes()</strong> function.




The test cases are split into <strong>3</strong> groups, each one testing a different Ouroboros data structure. For all of the groups, the <strong>insert_and_link()</strong> function will be tested first. From there, either the <strong>remove_and_link() </strong>or the <strong>count_nodes() </strong>function will be tested next, before testing the remaining function. In other words, if the <strong>remove_and_link()</strong> function is tested first, then the <strong>count_nodes()</strong> function will be tested next, and vice-versa.




<strong>IF TESTING IS DONE ON REPL:</strong>




I understand many of you will be using Repl on completing the assignment. As such, here is a suggested way of testing your program. Please note that this approach will <strong>NOT</strong> guarantee that it will work.




When a new Repl is created, the <strong>main.py</strong> file will be automatically created. Before moving forward, make sure that <strong>THREE</strong> files (excluding the <strong>main.py</strong> file) are to be present within the file hierarchy of the Repl: the <strong>node.py</strong> file, the <strong>ouroboros.py</strong> file (THIS IS YOUR PROGRAM), and the <strong>ouroborosTester.py</strong> file. From this point, your Repl should now have a total of <strong>FOUR </strong>files in no particular order: the <strong>main.py</strong> file, the <strong>node.py </strong>file, the <strong>ouroboros.py</strong> file, and the <strong>ouroborosTester.py</strong>. Within the <strong>main.py</strong> file, include the following line of code:




import ouroborosTester




When you click <strong>Run</strong> on Repl, the tester program should then start  running and providing feedback on your program.




This feedback will range from whether your program is not named correctly, or if its not found in the same folder as the other files, or if any of your functions are either not properly defined (in the sense of adhering to Python’s syntax), or is misspelled, this will raise an error.







<h1>7.Help &amp; Advice</h1>




If you feel overwhelmed by this assignment, don’t be. A good starting point is to first create skeleton definitions of the required functions that returns dummy values. From there, work on the function that you feel is the easiest to implement. Once defined, run the ouroborosTester.py program and see if you were able to successfully implement it. From this point, rinse and repeat.




If you need any kind of clarification to anything on this assignment, such as if you’re confused about the requirements for one of the functions, or if you encounter a bug error that you are unable to figure out on your own, please send an email to <strong><a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="9af9f2e9eae8f5fdecf5f6dafdf7fbf3f6b4f9f5f7">[email protected]</a></strong>. You may expect a response within 24 to 48 hours