# CISS222 Spring 2021 - Homework 1 - Instructions

## Notes
* All tasks that need to be completed will have an empty checkbox icon displayed next to it. You do not have to check the boxes as you complete the steps, but you can if you want. This is done using Markdown syntax. [More information about Markdown syntax for checklists can be found here](https://github.blog/2014-04-28-task-lists-in-all-markdown-documents/).
* At the end of the instructions, there will be a series of questions to answer based on your work in the assignment.
* You will need to take and capture screenshots and paste them into a Microsoft Word document, and upload that document to Canvas.
* You do not need to make any changes to this repository.

## Instructions


### Create an empty Microsoft Word document
You will be capturing a series of screenshots in the course of this assignment. Create a new Microsoft Word document titled "Homework1-" and your first and last name without a space (for example, I would create it as Homework1-DavidGreen.docx). You will be adding screenshots to this document and uploading it to Canvas upon completion of the assignment.

### Create a solution and project
When you are creating a solution within Visual Studio (VS), you will most likely want to create a project at the same time. That is the default way that VS operates, and in most cases that is completely fine. Just keep in mind that there are instances when you may want to create an empty project.

- [ ] Create an empty solution in VS called "Homework1-" and your first and last name without a space (for example, I would create it as Homework1-DavidGreen). This solution should contain a project that will let you create a .NET Core-based C# console app.
- [ ] Take a screenshot of the solution and project
- [ ] Add a heading in the Microsoft Word document called "New solution and project screenshot" and paste in the screenshot

### Navigating Visual Studio
When you open a Visual Studio (VS) solution and project, a lot of windows are opened up. Each window has a purpose, and depending on what you are working on, may be extremely valuable. In addition, some of the features that might also be helpful don't display by default, so you will need to know that they exist and how to show them.

As you work in VS, you may end up customising what windows are open and where, and that is great. However, sometimes, the view doens't quite work, or VS will open up a window in a place that you don't want it to be. To get things back to where they were when you first installed VS, you can reset your view.

- [ ] Reset your VS window view to defaults (*hint - what menu option likely deals with VS windows?*)
- [ ] Take a screenshot of the new VS window
- [ ] Add a heading in the Microsoft Word document called "VS window screenshot" and paste in the screenshot

### Manage folders and files
All but the most trivial C# programs involves creating multiple C# classes (and other core types) that are stored in individual files. Depending on the size of the project, you may want to organise your code into folders.
- [ ] Create a new folder called "Classes"
- [ ] Create a new class with a file name of "EmptyClass.cs"
- [ ] Take a screenshot of the Solution Explorer that shows the folder and class and add it between the below slashes
- [ ] Take a screenshot of the contents of the class file that was created (*if this was contained in the above screenshot, you don't have to take a second one*)
- [ ] Add a heading in the Microsoft Word document called "New folder and class screenshot" and paste in the screenshot (*if this was contained in the above screenshot, just state it in the Word document*)

At this point, you've created a new class called "EmptyClass." [That's a terrible name for a class](https://external-preview.redd.it/GSgbX1_nC49ZwGc9yGiN4lvEllsRNDxejwTJnnYR8iY.jpg?auto=webp&s=08d95e550e9fe215e45466c21b64b8c49fc09159). You will completel your first [refactoring](https://en.wikipedia.org/wiki/Code_refactoring) by renaming this class (and its associated file) to something better.

- [ ] Rename the "EmptyClass.cs" to something more interesting (whatever you want, as long as it is appropriate for school)
- [ ] Rename the class to match (note that class names don't have the .cs extension)
- [ ] Take a screenshot of the Solution Explorer that shows the renamed class
- [ ] Add a heading in the Microsoft Word document called "Renamed class screenshots" and paste in the screenshot
- [ ] Take a screenshot of the contents of the renamed class file and add it between the below slashes (*if this was contained in the above screenshot, you don't have to take a second one*)
- [ ] Paste the screenshot into the "Renamed class screenshots" heading

Sometimes, some files don't make the cut. As you are writing your code, it will evolve, and you will make decisions to remove a class or other object. You can [delete objects](https://www.theseoproject.org/wp-content/uploads/2016/08/delete-sp-meme-300x169.png) by deleting the file that contains it.

- [ ] Create a new class "ToBeDeleted" within the "Classes" folder
- [ ] Take a screenshot of the class within the Solution Explorer
- [ ] Add a heading in the Microsoft Word document called "Deleted file screenshot" and paste in the screenshot
- [ ] Delete the newly created class (you don't need to post a screenshot - when you submit the assignment, it won't be there)

### Managing code
The core of what a programmer does is write and manipulate code to make a computer operate as the programmer intends. That's why it is important to understand the some of the core benefits offered by VS.

When you create a solution with a console app, VS is nice enough to stub out a default file `Program.cs` with a default `Main()` method, and a nice `Hello world` output statement. Of course, a ["Hello World!"](https://pics.me.me/when-your-code-outputs-hello-world-4585493.png) program isn't particularly helfpul for anything that you would need to do. At this point, as a developer, you would start replacing this default boilerplate code with what you actually need. When writing code, VS offers a plethora of features to make your life as a programmer easier. Let's go through a couple.

- [ ] Take the following code and enter it above the `Console.WriteLine()` statement in your `Program.cs` file.
`string xyz = "Hello World!"`
- [ ] Replace the string `"Hello World!"` in the `Console.WriteLine()` statement with `xyz`.
- [ ] Take a screenshot
- [ ] Add a heading in the Microsoft Word document called ""Hello World" variable" and paste in the screenshot

Using variables, like you just did with the `stgring xyz` is a very helpful way to track application "state." We'll get into that later. But the name `xyz` isn't a very good variable name. What does it mean? In a tiny program like this, it doesn't matter. However, when your program contains hundreds (or thousands) of lines of code across many folder and files (or even projects), descriptive names are critical. This is another good opportunity for refactoring.

- [ ] On the line with `string xyz`, backspace out `xyz` and replace it with `abc`. Click on the "Debug" menu, and choose "Start Debugging" (you can refer to this as "running the program," "running," or "debugging"). You will get an error message. Take a screenshot
- [ ] Add a heading in the Microsoft Word document called "Rename variable" and paste in the screenshot
- [ ] If you haven't already click "No" on the dialogue that comes up. On the line with `Console.WriteLine()` backspace out `xyz` and replace it with `abc`. Debug the program again, take a screenshot
- [ ] Paste the screenshot into the "Rename variable" heading

Now, let's take a different approach to renaming.

- [ ] "Rename" the variable `abc` to a variable name of your choice that would be a better description of what this variable is. You can rename by doing either: right-clicking the variable name and choosing Rename; clicking on the variable, clicking Edit > Refactor > Rename; or pressing the key combination Ctrl and R twice on the keyboard.

A significant amount of a programmer's time is spent [debugging](https://meme.xyz/uploads/posts/t/22388-debugging.jpg). Ideally, the first time we write code, it will work flawlessly. Rarely, especially as the complexity of our programs grow, does this happen. Visual Studio offers best-in-class tools to make the debugging process easier. 

- [ ] Look for the line where the variable is delcared that you renamed. To the left of the line number, click on the blank area. The line should turn red and a red circle should appear. You have set a [breakpoint](https://docs.microsoft.com/en-us/visualstudio/debugger/using-breakpoints?view=vs-2019). Take a screenshot.
- [ ] Add a heading in the Microsoft Word document called "Breakpoints and stepping" and paste in the screenshot

Debug the program. You'll notice that the program stops at the red line and it has turned yellow. Program execution has stopped at the "breakpoint" - this is referred to as "break mode." Look for the black program window and notice that there isn't anything displayed. At this point, as a developer, you have options for continuing the program. Look for the menu option, toolbar button, or use the keyboard shortcut for "Step Into" an advance to the next line.

- [ ] Now the `Console.WriteLine()` is highlighed in yellow, and the previous line has returned to being red. Take your mouse and hover over the variable name on either line. Take a screenshot of what popped up
- [ ] Paste the screenshot into the "Breakpoints and stepping" heading

When navigating VS, you can use your keyboard to perform almost any critical function. In many cases, learning these keyboard shortcuts can save you time because you do not need to take your hands off of they keyboard to use the mouse, improving your productivity. If you take the mouse and click through menus, you will see the keyboard shortcut that will launch that menu option.

- [ ] Press the F5 key. Take a screenshot of the result.
- [ ] Add a heading in the Microsoft Word document called "Keyboard shortcuts" and paste in the screenshot

---

### Questions

Return to the assignment in Canvas and answer the questions.
