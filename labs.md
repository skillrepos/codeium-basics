# Codeium Basics
## Practical Tips and Best Practices
## Session labs
## Revision 2.2 - 08/20/24

**Follow the startup instructions in the README.md file IF NOT ALREADY DONE!**

**NOTE: If you are in VS Code and don't see a terminal, click on *Terminal -> New Terminal* in the menu.

![Open new terminal](./images/cb18.png?raw=true "Open new terminal")


**Lab 1 - Learning how to create good prompts for Codeium**

**Purpose: In this lab, we’ll start to learn about Codeium and how it generates code based on the prompts we provide**

1. Create a new file. In the terminal, enter

   ```
   code index.js
   ```
![Create file](./images/cb19.png?raw=true "Create file")

2. Afterwards this file should be open in a tab in the editor.

3. Let's see how Codeium responds to a generic request. Go to that tab and type in a comment that says

```
// function to parse data
```
4. Hit return and notice the code that Codeium suggested. This is likely more generic than we want, but hit tab to select that line.
   
5. After hitting tab, Codeium will generate another part of the function. (If not, you may need to hit return.) Hit tab to accept it. Continue until you get a complete function. One example of what code may look like is below.

![Codeium generated function](./images/codeium-15.png?raw=true "Codeium generated function")
   
6. This prompt is not specific enough for Codeium to interpret what we want to do.  Highlight the code and delete it, so we can try again.

7. Now type a comment at the top that says

```
// function to parse url
```
8. Hit enter and you will probably see a similar line to the below. If not, you may need to use the ">" button in the acceptance bar to flip to the next option.

```
function parseURL(url) {
```

9. Just hit Tab to accept it and Enter again. Continue to use Tab and Enter to build out the function from the suggestions that Codeium provides until you get a complete function definition - something like shown below.

![Codeium generated function](./images/codeium-16.png?raw=true "Codeium generated function")    

10. Let's do one more pass at getting a specific prompt for Codeium. Delete all the code currently in index.js. This time we will not enter a comment, but will enter a specific funtion name.
Type the following in the empty file. (There are no parentheses after the *splitURLandReturnComponents* text.)  Do not hit tab or return yet.

```
function splitURLandReturnComponents
```

11.  With this function name, Codeium should suggest a full function definition - in fact it may suggest several.  To see the options, hover over the first line and a small window should appear. This window will note how many options there are and provide "<" and ">" links to toggle between them.  Click on the "<" and ">" buttons to see the differences in the available suggestions. Some may be full function suggestions and others may be only partial suggestions.  Choose an alternative you like and then select Tab to accept it.

![alternative suggestions inline](./images/codeium-17.png?raw=true "alternative suggestions inline")   


<p align="center">
**[END OF LAB]**
</p>

**Lab 2 - Using Codeium to refactor existing code**

**Purpose: In this lab, we'll explore options for refactoring with Codeium**

1. Create a new file named prime.py. Create it via the same process as we used in Lab 1 by entering the line below in the terminal.

```
code prime.py
```

2. Start typing a function definition as below and enter to get to a suggestion from Codeium.
```
def is_prime(n):
```
3. Pick one of the offered suggestions and hit Tab. Continue until you get a full function definition. One example is shown below.

![alternative suggestions inline](./images/codeium-18.png?raw=true "alternative suggestions inline")   

4. Let's next try some of the refactor options provided by Codeium. Click on the *Refactor* link in the Codelens menu above the code. Then select the option to *Make this faster and more efficient* (You can click on the entry in the list or type in the selection in the text entry area.)

![codelens refactor](./images/codeium-91.png?raw=true "codelens refactor")   
![refactor for efficiency](./images/codeium-25.png?raw=true "refactor for efficiency")         

5. Codeium will then generate any suggested changes inline. Give it a moment to complete and then click on *Accept* to accept the changes.

![refactor to add comments](./images/codeium-32.png?raw=true "refactor to add comments") 

6. Next, click on the *Refactor* link and select the option to *Clean up this code*.

![refactor to clean up code](./images/codeium-22.png?raw=true "refactor to clean up code") 
  
7. Give Codeium a moment to generate is suggested changes. This time after reviewing, we'll reject the changes. Click on the *Reject* option.

![refactor to clean up code](./images/codeium-33.png?raw=true "refactor to clean up code")     

8. Finally, let's add some print statements for debugging. Select the *Refactor* link again and this time, start typing "Add print" in the text box to filter the choices. You can then select the full option from the filtered list.

![refactor to add print statements](./images/codeium-34.png?raw=true "refactor to add print statements")  

9. After a moment, Codeium will suggest a set of changes for adding the print statements. You can just go ahead and accept these.

![refactor to add print statements](./images/codeium-35.png?raw=true "refactor to add print statements")  

    
<p align="center">
**[END OF LAB]**
</p>

**Lab 3 - Using Codeium to explain and document code**

**Purpose: In this lab, we’ll see a few other ways to leverage Codeium after the initial coding is done**

1. Let's have Codeium explain how our current function works. In the Codelens menu above the code, click on the *Explain* link. 

![explain link](./images/codeium-36.png?raw=true "explain link") 

2. The explanation is provided in the Codeium chat window. Notice the context that Codeium used (the function *is_prime* next to */explain) and the full explanation in the section below.

![explain function](./images/cb20.png?raw=true "explain function") 

3. Suppose we want to save this chat for future reference or to easily share.. Click on the 3 vertical dots in the upper right of the *CHAT* tab.

![chat menu](./images/codeium-38.png?raw=true "chat menu") 

4. Next, click on the *Export Conversation* item and download the file as a .md (*markdown*) text file.

![download markdown file](./images/codeium-39.png?raw=true "download markdown file") 

5. From wherever you downloaded it to, you can open up the .md file and view it.

![view chat file](./images/codeium-40.png?raw=true "view chat file")    

6. We can also use shortcut commands to do these same kind of tasks like *explain*. In the Codeium Chat interface, enter the text below to see the results. Notice the results may be more in a numbered list order than the free-form text previously used.
```
/explain is_prime
```
![explain in chat](./images/codeium-41.png?raw=true "explain in chat") 

7. We are done with the explanations, so let's clear those Chats from the history. Click on the *Conversations* icon (the one that looks like a clockface with a circular arrow) and select that.

![conversations icon](./images/codeium-42.png?raw=true "conversations icon")    

8. From this screen, you'll see a list of any previous chats. Hover over any chats that you want to delete, and click on the trash can icon to delete the chat. Then, when done, click on the *Back to chat* link to return back to the main chat interface.

![conversations icon](./images/codeium-43.png?raw=true "conversations icon")    

9. Next, let's generate some doc for this code. Click on the *Generate Docstring* link in the Codelens section. (If you don't see a *Generate Docstring* link, you can just click on the *Refactor* menu item and type in "Generate Docstring".)

![generate docstring](./images/codeium-44.png?raw=true "generate docstring")    

10. The proposed change will show up in the chat interface. When it is ready, you can click on the *Apply Diff* link and then *Accept* the change in the editor.

![apply docstring](./images/codeium-45.png?raw=true "apply docstring")  

11. Finally, let's have Codeium add some more comments in our code. Click on the *Refactor* link again and this time, select the last item *Verbosely comment this code so that I can understand what's going on.* When Codeium finishes the suggestions, you can just *Accept* them. (If there is some part of the proposed change that you don't like, you can just delete those lines.)

![add comments](./images/codeium-46.png?raw=true "add comments")  
    

<p align="center">
**[END OF LAB]**
</p>

**Lab 4 - Using Codeium to generate tests**

**Purpose: In this lab, we'll see some examples of having Codeium automatically generate test cases for our code**

1. Start out in the *prime.py* file we've been using. Position the cursor on a blank line below the existing code. Bring up the inline chat interface with *CMD+I* and enter the following directive. Then click on the *Codeium: Submit* button.

```
create a function to do 5 unit tests of the code
```
![generating tests via comment](./images/codeium-47.png?raw=true "generating tests via comment") 

2. This gives us a set of unit tests, but let's see what other ways we can generate testing code. Go ahead and *Reject* the suggestion.

![suggested tests via comment](./images/codeium-48.png?raw=true "suggested tests via comment") 

3. Bring up the inline chat interface with *CMD+I* and enter the following directive. Then click on the *Codeium: Submit* button.

```
/test
```
![generating tests via command](./images/codeium-49.png?raw=true "generating tests via command") 

4. Similar to the last option, this gives us a set of unit tests, but we may still be able to do better. Go ahead and *Reject* the suggestion.

![suggested tests via command](./images/codeium-50.png?raw=true "suggested tests via command") 

5. Let's try a slightly different way of generating tests.  Switch to the Chat interface and enter the following text. When you get the *"@prim"* part typed, Codeium should give you a popup to select from different categories of objects to complete the query.  Choose *Code Context Items* as shown in the screenshot below. 
```
 How would you design a comprehensive test suite for the code in @
```
![suggested tests via chat](./images/cb21.png?raw=true "suggested tests via chat") 

6. After selecting the *Code Context Items*, it should provide you an option to choose the *is_prime* function.  Select that and it should complete the query. Then you can hit Enter and generate test from that query.

![suggested tests via chat](./images/cb22.png?raw=true "suggested tests via chat") 
![suggested tests via chat](./images/cb23.png?raw=true "suggested tests via chat") 

7. After a few moments, Codeium should propose a set of steps for the test suite in the Chat interface, along with example code afterwards.

![suggested tests via chat](./images/codeium-52.png?raw=true "suggested tests via chat") 

7. Let's take the output of the chat and add it as a new file for the tests. Create a new file and call it *prime-tests.py*. You can do this from the codespace's terminal by typing the following:
```
code prime-tests.py
```
8. Switch to the new file if its not already open. Now, at the start of the code listing in the Chat interface, select the *Insert* tab and insert the code into the new *prime-tests.py* file.

![copied_tests via chat](./images/codeium-53.png?raw=true "copied tests via chat") 
  
9. Let's double-check with Codeium for any missing test cases. With the *prime-tests.py* file open, go to the Chat interface and enter the following:
```
identify any missing test cases and provide code for them

```
10. After this runs for a bit, you will likely see it generating test cases for a few more areas. When its done generating them, you can select the ones you want from the suggested code and paste into your file.

![copied_tests via chat](./images/codeium-54.png?raw=true "copied tests via chat") 
    
11. Save the new files if desired.


<p align="center">
**[END OF LAB]**
</p>


**Lab 5 - Using Codeium to help with SQL**

**Purpose: In this lab, we’ll see some examples of how to have Codeium help with writing SQL and also see how to add additional context**

1. Create a new file named dev.sql. You can create it via entering the line below in the terminal.

```
code dev.sql
```
   
2. Afterwards this file should be open in a tab in the editor. Assume we want to work with a database or database definition that defines a dataset for students, staff, curriculums, courses, schools of study, locations, and registrations for a university system. Let's see what Codeium would generate without any other context for a query to get all students in a course. Enter the following comment below and press Tab to accept suggestions. 

```
-- define a select statement to get all students enrolled in a course
```
![generated query](./images/codeium-55.png?raw=true "generated query") 
    

3. Go ahead and save this file as part of the project.  You can do this from the menu under *File->Save*.
   
4. Let's see if we get any different results if we provide Codeium additional context. Open the file create-tables.sql in the editor from the GitHub repository. (You can either select and open it from the file list or use the command below from the terminal.) Scroll through it and take a quick look at the contents.

```
code create-tables.sql
```

5. Now with that file open, go back up to the top of the *dev.sql* file.  Highlight and delete the comment and resulting query from step 2.
  
6. Enter the same comment as before to request the query. (Basically, repeat step 2.) See what Codeium suggests this time. You can accept the suggestions or cycle through options. 

```
-- define a select statement to get all students enrolled in a course
```

7. If all goes well, this second pass should generate multiple completion options with many more specific references to the names and identifiers used in *create-tables.sql*. (You may want to cycle through the suggested options to get to the later ones - i.e. 8/8 for example.) Take a look at the query and then compare the names/identifiers used to the ones in the *create-tables.sql* file. This will show that Codeium picks up on context from other files available to it to make better suggestions.

![New query](./images/codeium-58.png?raw=true "New query") 

8. However, if you don't get a good suggestion from Codeium for the comment, try copying the code from the *create-tables.sql* file and pasting it in below the comment in the *dev.sql* file. Then try the query again. (If there are multiple suggestions, click through them.) After it works, you can remove the duplicate code you copied in.

![Alternate approach](./images/cb24.png?raw=true "Alternate approach") 

Then try the query again. (If there are multiple suggestions, click through them.) After it works, you can remove the duplicate code you copied in. You can tab and enter until the query is done.

![Alternate approach](./images/cb25.png?raw=true "Alternate approach")
   
9. In some cases, we might be able to use a separate index to speed up operations.  Let's ask Codeium to create a new index based on the last query. Add the following line after the current query in the file *dev.sql*.

```
-- write an index to improve the performance of the query
```
![index](./images/codeium-59.png?raw=true "index") 

9. Let's suppose we also want to have a table to capture student attendance. We can ask Codeium to create the table definition for us.

```
-- define a table for student attendance to capture attendance by class
```

![status values](./images/codeium-60.png?raw=true "status values") 

10. Codeium can also create stored procedures. Let's ask it to create a new stored procedure for getting a list of enrolled students at a particular location. Let's use the **CMD+I** shortcut. Go to the bottom of the *dev.sql* file, invoke Codeium Chat via the shortcut and then enter the line below in the dialog and then click the *Submit* button. You can choose to **Accept** or **Discard** the result.

```
define a stored procedure to get course enrollment by location
```
![prompt for stored procedure](./images/codeium-61.png?raw=true "prompt for stored procedure") 
![results for stored procedure](./images/codeium-62.png?raw=true "results for stored procedure") 
  
11. Finally, let's see Codeium optimize a query for us. Suppose we want to get all the course registrations for September, 2023.  Enter the following query in the file.

```
select * from courses.registration where year(registration_date) = 2023 and month(registration_date) = 9
```

12. Ask Codeium to optimize the previous query. You can do this via highlighting the query, using the **CMD+I** shortcut and entering "optimize" in the dialog. 
```
optimize
```

13. Afterwards, Codeium should generate a suggested optimization. You can *Accept* or *Reject* the result.
 
![Optimization suggestion](./images/codeium-64.png?raw=true "Optimization suggestion") 
    
<p align="center">
**[END OF LAB]**
</p>

**Lab 6 - Teaching Codeium about updates**

**Purpose: In this lab, we’ll see an example of what to do when Codeium does not have the most up-to-date information**

1. Create a new file called *explore.go* via the same approach as you used to create other files.

2. This file should now be open in an editor tab. Let's say we want to seed a random number generator with Go. Let's ask Codeium to write a function to do that. Prompt it through the **CMD+I** interface using the statement below. Then you can accept the suggested code.

```
write a function to seed a random number generator
```
![Asking Codeium to write function to seed a random number generator](./images/codeium-65.png?raw=true "Asking Codeium to write function to seed a random number generator") 

3. Codeium has probably generated code using the rand.Seed function. The challenge is that as of Go 1.20, the Seed function is deprecated.  Ref: https://cs.opensource.google/go/go/+/refs/tags/go1.21.0:src/math/rand/rand.go;l=394

![codeium-generated seed function](./images/codeium-67.png?raw=true "codeium-generated seed function") 

4. So one way we can help Codeium understand language updates is by providing updated context in our file. So let's start again. Delete the current content in the explore.go file.

5. Now,let's provide Codeium some more direct context by copying in updated code examples. After deleting the code block from step 3, copy and paste in the following example of the replacement for the Seed deprecation into your explore.go file.  This is taken from pkg.go.dev/math/rand.

```
	// Create and seed the generator.
	// Typically a non-fixed seed should be used, such as time.Now().UnixNano().
	// Using a fixed seed will produce the same output on every run.
	// r := rand.New(rand.NewSource(99))
```

6. Now, let's try the creation of the function again. Underneath the comments and code you just pasted, invoke the dialog via **CMD+I** and enter the statement below again.
```
write a function to seed a random number generator
```

![codeium-generated seed function attempt 2](./images/codeium-70.png?raw=true "codeium-generated seed function attempt 2")

7. This time, the code should be using the same format and NewSource function as you put in the file in step 6. You can just Accept the change.

![Updated random number gen code after including updated usage](./images/codeium-71.png?raw=true "Updated random number gen code after including updated usage")

8. You can also ask Codeium via the chat if the function is deprecated. Switch to the Codeium Chat interface and enter the following prompt.

```
Is the Seed function deprecated in Go?
```
You will likely see a response in the Chat interface saying that it's deprecated and also showing the new function to use.

![codeium-generated seed function](./images/cb26.png?raw=true "codeium-generated seed function") 

<p align="center">
**[END OF LAB]**
</p>

**Lab 7 - Kubernetes, YAML generation and the version problem**

**Purpose: Show YAML generation and out of date content.**

1. Create a new file - **deployment.yaml**

```
code deployment.yaml
```

2. Bring up the Codeium Chat dialog via **CMD+I** and enter in (or copy and paste) the following request and hit the Submit button.

```
write spec for deployment in Kubernetes with 2 replicas and image from busybox
add command to run in containers: sleep 3600
add label app: myapp
add label type: front-end
```
![request Kubernetes manifest](./images/codeium-72.png?raw=true "request Kubernetes manifest")

3. After a few moments, you should see it respond with the code. You can just Accept this.
![Kubernetes manifest](./images/codeium-73.png?raw=true "Kubernetes manifest")

4. Suppose we don't know how to execute this code. Let's ask Codeium. Highlight the generated YAML in the deployment.yaml file.  Then go to the larger Chat interface and ask it. Put the following in the Chat interface. (See parts 1 and 2 in the next screenshot.)

```
How do I execute this?
```

5. Codeium should respond with something similar to what's shown in the next screenshot.
   
![How to execute deployment](./images/cb27.png?raw=true "How to execute deployment")


6. While we're in the Chat interface, let's ask it for the latest K8s version that it knows of. Put the following into the dialog.

```
What is the current version of Kubernetes?
```

7. Codeium will probably respond that it does not know the current version. This is unfortunate since we don't know how out-of-date the generated content may be.

![Answer to latest K8s version](./images/cb28.png?raw=true "Answer to latest K8s version")

8. We can at least ask Codeium how to determine the current version of Kubernetes. Enter the following in the Chat interface.

```
How do I determine the current version of Kubernetes?
```
  
9. This will create a suggested command to determine what the current Kubernetes version is, along with options to *Copy* or *Insert in Terminal*. Go ahead and select the *Insert in Terminal* option and try to execute the command.

![Answer to latest K8s version](./images/cb29.png?raw=true "Answer to latest K8s version")

10. If the command included the *--short* option, you'll get an *unknown flag*. This is because that option is deprecated but Codeium wasn't aware of that change. You can run the command without that option to see the current Kubernetes version.

![deprecated flag](./images/cb30.png?raw=true "deprecated flag")

11. Next, let's have Codeium generate some code to work with Kubernetes through the API. In the chat interface, enter the following.

```
How do I call the K8s API for scaling a deployment to 5 replicas with Python?
```

9. Create a new file and then paste the suggested code into the new file via the *Copy* or *Insert* option.

![Add code to new file](./images/codeium-78.png?raw=true "Add code to new file")


10. Suppose we change our mind and want to convert this code to Go. Click in the new file, and highlight the new code. Then, in the *Refactor* interface tell it to translate to Go.

```
translate to Go 
```
![Go translation](./images/codeium-79.png?raw=true "Go translation")


11. If you look at the generated differences, you should now have the equivalent Go code available for accepting.

![Go translation](./images/codeium-80.png?raw=true "Go translation")

<p align="center">
**[END OF LAB]**
</p>
    
**Lab 8 - Exploring Javascript, regular expression generator, auto-generating data**

**Purpose: Show Javascript and regular expression generation, auto-generate routine mappings**

1. Create a new file as **phone.js**

```
code phone.js
```

2. Prompt Codeium to create a function with a regular expression to validate a US phone number. You can use the **CMD+I** interface.
```
create a function to validate any global phone number using a regular expression
```
![prompt to validate phone #](./images/codeium-81.png?raw=true "prompt to validate phone #")

3. You can just *Accept* the suggested implementation.

![Regex function to validate phone #](./images/codeium-82.png?raw=true "regex function to validate phone #")   

3. Now let's see how Codeium can generate some data and mappings for us automatically. Enter the prompt below in the main Chat text entry area.
```
create a mapping of states to area codes in JavaScript where the key is the state abbreviation and the value is an array of area codes of max size 5
```
4. After running this, Codeium will generate the a list as shown below. Click on the *Insert* tab to insert the updates at the cursor in the *phone.js* file. (This assumes the cursor is below the previous function in the file.)

![Automatic gen of data](./images/codeium-84.png?raw=true "Automatic gen of data") 

5. While this works fine, there may be times we only get partial completions or want to augment the data later. Codeium can handle this use case also. To see this, try the prompt below in Chat and notice the 5 states you get data for.
```
create a mapping of 5 states to area codes in JavaScript where the key is the state abbreviation and the value is an array of area codes of max size 5
```

![Automatic gen of data](./images/cb31.png?raw=true "Automatic gen of data")

6 To get the rest of the mappings for the other states, you can try a prompt like the following (note the use of the term "the other states" in it):

```
create a mapping of the other states to area codes in JavaScript where the key is the state abbreviation and the value is an array of area codes of max size 5
```
k, you can copy the mappings and add them into the code file. 
![Completing the mappings](./images/cb32.png?raw=true "Completing the mappings") 
   

<p align="center">
**[END OF LAB]**
</p>


<p align="center">
**THANKS!**
</p> 
