# 2048C-Mod2-Demo1-Lesson1

# Lesson 2: Styling an HTML5 Page

### Demonstration: Adding CSS Styles to an HTML Page

#### Preparation Steps 

Ensure that you have cloned the 20480C directory from GitHub (**https://github.com/MicrosoftLearning/20480-Programming-in-HTML5-with-JavaScript-and-CSS3/tree/master/Allfiles**). It contains the code segments for the labs and demos in this course. 

#### Demonstration Steps

#### Create New Styles by Using Visual Studio

1.	Open Visual Studio.
2.	In Visual Studio, on the **File** menu, point to **Open**, and then click **Project/Solution**.
3.	In the **Open Project** dialog box, browse to the **[Repository Root]\Allfiles\Mod02\Democode\Starter** folder, click **DemoWebSite.sln**, and then click **Open**.

>**Note**: If **Inconsistent Line Endings** dialogue box appears, clear **Always show this dialog** checkbox and then click **Yes**.

4. In Solution Explorer, expand the **DemoWebSite** Project , and then expand the **styles** folder.

5. Double-click **ContactUsStyles.css**.

6. Review the existing rules for the **body** and **h1** elements.

7. Modify the **body** rule, remove the **color** rule, and change the font used on the whole page as shown in the following code example.

   ```css
       body {
         font-family: "Segoe UI", Helvetica, Arial, sans-serif;
       }
   ```

8. Remove the following rule from the stylesheet:

   ```css
       h1 {
         font-family: 'Copperplate Gothic';
         color: red;
       }
   ```

9. To make the header appear separately from the rest of the content, add the following rules:

   ```css
       header {
         padding-bottom: 10px;
         border-bottom: 2px dotted blue;
         margin-bottom: 10px;
       }
   
       header h1 {
         margin-left: 20px;
         display: inline-block;
       }
   ```

10. Add the following empty rule:

    ```css
        section {
        }
    ```

11. Verify that the section rule now looks like this:

    ```css
        section {
          padding-bottom: 5px;
          border-bottom-style: dotted;
          border-bottom-width: 1px;
          border-bottom-color: grey;
        }
    ```

12. To style the form and its elements, add the following rules:

    ```css
        fieldset {
          background-color: pink;
          margin-bottom: 10px;
        }
    
        legend {
          font-size: 1.2em;
          font-style: italic;
        }
    
        fieldset li {
          list-style: none;
          margin-bottom: 10px;
        }
    
        input[type="submit"] {
          background-color: pink;
          opacity: 0.6;
          width: 200px;
        }
    ```

13. On the **File** menu, click **Save All**.

#### Use the F12 Developer Tools to Inspect Styles

1.	In Solution Explorer, double-click **ContactUs.html**.
2.	On the **Debug** menu, click **Start Without Debugging**.
3.	In Microsoft Edge, if the **Intranet settings are turned off by default** message appears, click **Don’t show this message again**.
4.	Verify that the new styles have been applied to the page.

![alt text](D:/610 - Curso Desarrollo Web/Practicas/JavaScript/2048C/Instructions/Images/20480B_2_ContactUs_Styled.png "The ContactUs page with styling")

5. In Microsoft Edge, press F12.

6. In the **F12** window, select the **DOM Explorer** tab, and then double-click the **&lt;html&gt;** element.

7. Click the **&lt;body&gt;** element.

8. In the right pane, verify that the following CSS rule appears:

   ```css
       font-family: "Segoe UI", Helvetica, Arial, sans-serif;
   ```

9. In this rule, select the text **"Segoe UI"**, change it to **"Times New Roman"**, and then press Enter.

10. In Microsoft Edge, verify that this font change reflects on the page.

11. In the left pane, expand the **&lt;body&gt;** element, expand the **&lt;article&gt;** element, and then click the first **&lt;section&gt;** element.

12. In the right pane, verify that the following styles are specified for this section:

    ```css
        inherited – body
          body
            font-family: "Times New Roman", Helvetica, Arial, sans-serif;
        section 
          padding-bottom: 5px;
          border-bottom-color: grey;
          border-bottom-width: 1px;
          border-bottom-style: dotted;
    ```

13. To close the **F12** window, press F12.

14. Close Microsoft Edge, and then close Visual Studio.

### Demonstration: Creating and Styling an HTML5 Page

#### Preparation Steps 

Ensure that you have cloned the 20480C directory from GitHub (**https://github.com/MicrosoftLearning/20480-Programming-in-HTML5-with-JavaScript-and-CSS3/tree/master/Allfiles**). It contains the code segments for the labs and demos in this course.

#### Demonstration Steps

1.	Read the lab scenario to the students and point out that they should read each scenario before attempting the lab for a module.
2.	Point out to the students that the exercise scenario for each exercise contains a description of what they will accomplish in the exercise, and is also essential reading.
3.	Start Visual Studio. Then, in the **Allfiles\Mod02\Labfiles\Solution\Exercise 2\ContosoConf** folder, open the **ContosoConf.sln** solution.

>**Note**: If **Security Warning for ContosoConf** dialogue box appears, clear **Ask me for every project in this solution** and then click **OK**.

4.	In Solution Explorer, expand the **ContosoConf** project, and then double-click **index.htm**.
5.	In code editor, briefly scroll through the HTML markup for the web page, and explain to the students that they will be creating the **Home** page for the web application and adding the HTML markup to display the elements on this page.
6.	In Solution Explorer, double-click **about.htm**.
7.	In code editor, explain that this page contains information about the conference, but the current data is just placeholder text that the conference organizers will replace later with specific information about the conference.
8.	In Solution Explorer, expand the **styles** folder, and then double-click **site.css**. Explain to students that this style sheet contains the initial global styles that they will be defining for the application, and that these styles will be applied to the **Home** and **About** pages.
9.	On the **Debug** menu, click **Start Without Debugging**.

>**Note**: If the **Intranet settings are turned off by default** message appears, click **Don’t show this message** again. 

10.	In Microsoft Edge, show the simple styling for the **Home** page. The labs in later modules will modify and extend some of these styles, for example, to change the appearance of the navigation bar.
11.	In the navigation bar, click **About**. Again, explain that the simple styling used by this page will be modified in later labs to generate a more appealing layout.
12.	Close Microsoft Edge.
13.	Close all open windows.