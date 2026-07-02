# Unit 0: Getting Started 

### What you'll be able to do after this unit:

- Explain what Python is
- Explain how Python actually runs
- Access the terminal
- Install Python on your device
- Decide where to write code (an IDE)
- Write your first program
- Use AI to deepen your understanding
______________________________________________________________________

### Concepts

#### What is Python?

Python is a programming language! It's used to give instructions to a computer (which cannot understand our written English). [People love Python](https://www.python.org/doc/essays/blurb/) because it reads like English and it's versatile (used by both NASA scientists and game developers alike, for example)! 

On the spectrum of languages where the two extremes are a. machine-readable (completely incomprehensible to humans) and b. vernacular human language, Python is way closer to vernacular. Partly for this reason, it's considered a "high-level" language, while others that are less comprehensible to us are considered more "low-level". 

#### How does it "run"?

When we write a program, we just write a plain text file (which is the same thing as, say, a Google doc) of instructions. To "run" it means to tell your computer to execute those instructions. Because computers don't understand human languages (this one included), there's a middleman program (called the Python interpreter) that steps in. Very roughly, the process looks like this:

1) You write a Python script (set of instructions, "code")
2) The interpreter reads the code and translates it into machine code
3) Your computer, now able to understand the machine code, carries out those translated instructions
4) You see the output on your screen (this could be anything, like a math problem or a set of words)

It's a little more complicated than that, but that's the idea: it's a multi-step process that, if understood well, will help you understand why there are so many errors you can make it coding.

#### The terminal

Once we've written our script, how do we hand it over to the interpreter? We use a tool called the terminal (on Mac, at least, which is what I have; it might also be called the "command line" or "console" depending on what device you have). Think of it like a text-only doorway into you computer's brain. It accomplishes the same thing as clicking around colorful icons with your mouse, and more.

We'll come back to this in a second, after we actually get Python on our laptops (notice: if you type in "python" in the Terminal and hit enter, you'll get some error that tells you it doesn't exist there yet). To fix that, you have to install it!

#### Installing Python

Download the latest version of Python: go to [this website](https://www.python.org/downloads/) and find the link for your specific machine:
[alt text](image.png)

Follow the instructions. At some point, you'll be asked to check the box "Add python.exe to PATH".

To test that it actually worked and that it's now on your computer, open your terminal and write

```python --version```

If the output says something like "Python 3.12.3" (or Python anything), you're good to go! [Here's what mine looks like:](Unit_0/Images/image-1.png)

If not, this would be a good time to paste a screenshot of the output into your AI tool of choice (mine is Claude). Tell it that although tried to install Python by downloading it from Python's official website, it doesn't seem to be available, per the screenshot. Let it walk you through possible problems. 

There will be times throughout this course when things don't work as you expected. In these times, you'll be tempted to seek perfect answers to your questions so you can move on as fast as possible. Try to resist this urge, and only ask questions when you're truly stuck. Do it in a way that still lets you "do" the solution and remember it!

#### Well, where do I write the code? 

Once you have Python installed (and can verify it from your terminal), you can actually run it from there itself! It's waiting to execute your instructions. You'll soon realize that doing this is clunky and uncomfortable, like trying to send a novel's manuscriptas a copy-and-pasted iMessage.

A better way to do it is to write it in a specialized and powerful code editor, called an [IDE (integrated development environment)](https://www.ibm.com/think/topics/integrated-development-environment). An IDE is like Microsoft Word and Google Docs, but for code. A much better way to send a novel manuscript via text is to create a PDF of it, then send THAT via text, right?

There are many options here, but my IDE of choice is called Visual Studio Code, which is known to its friends as VS Code! I love that it color-codes words so it's easy for you to spot typos, auto-completes, and has a built-in terminal! No need to understand the importance of these features just yet. We now need to download VS Code.

Use [this link](https://code.visualstudio.com/download?_exp_download=fb315fc982). [Again, find the one for your system.](Unit_0/Images/image-2.png)

#### Writing your first program

The first thing you want to do is create a new file. Look in the top left corner of your screen:

- [File > New File](Unit_0/Images/image-3.png)

A small box will pop up, asking you to name it. Name it hello.py, then hit Enter. This .py extension is important here, because it tells VS Code that what you're doing is a Python "script" (a set of instructions) and that it should turn on those beautiful code-helper tools like the color-coding!

Save the file somewhere it'll be easy for you find later, like Documents or on Desktop.

Here's your first program. Type this single line into your blank file exactly as it is here:

```print("Hello, world!")```

Now save it by hitting Ctrl + S (Windows) or Cmd + S on Mac to save your progress. 

Now let's run it! Go back to your terminal window, and type this:

```python hello.py```

Note that if you're on a Mac, it might be "python3" instead, but isn't for me. See if the first thing gives you grief. Does it say "Hello, world!" in the line below now?

If so, CONGRATULATIONS! You just wrote, saved, and ran your first Python program! You can also do that entirely on VS Code, by writing the line, saving it, and hitting the "play" button (instead of typing the line in every time into the terminal).
______________________________________________________________________

### Common confusions

#### The terminal vs. the script file in VS Code: where do I type stuff?

 - The TOP half = notepad, script. This is where you write your code (print("Hello, world!"))
 - The BOTTOM half = the terminal, where you run the code you wrote ("python helloy.py")

#### Forgetting to save before running

- Remember that the computer runs the SAVED file, not just the text active on the screen at that moment.[VS Code will show you a solid white circle, which indicates that your code is unsaved:](iUnit_0/Images/image-4.png). The dot disappears once you save the file (Command + S on Mac).

#### The "file not saved" error

- To understand the reason for this error, you have to understand that everything on your computer has a physical location: all files, folders, and the terminal itself. So if your terminal is currently in the "main user" folder but your hello.py file is currently in your Projects folder, the terminal won't be able to see it
- This is like telling someone who's standing in your garage that "the book is on the night stand" (which is actually in your bedroom). They won't be able to find it, because the location is wrong!
- To help with this confusion, it's often easier to use the terminal built into your VS Code, which will always be in the same directory (physical location) as the code you want to run (which is in a file, whose location is the same as the VS Code terminal)
- Another option is to use the cd (change directory) terminal command to move to a different directory -- ideally, the one that your file is in

This is a good place to turn to AI-- ask it to explain, simply, why it is that the terminal thinks the file doesn't exist. Try to figure out a solution, then prompt it again if you can't.
______________________________________________________________________

### Try it

1. Repeat this process: create another file in the same folder called "goodbye.py", use another print() statement, save it, and run it both in the VS Code terminal and in the regular terminal.

2. Python runs your code line-by-line from top to bottom. Use multiple ptint() statements to draw a smiley face that shows up in the terminal when you run it.

3. Create another file called broken.py and put just one line in:

```prnt("Hello, world!")``` 

... there will be an error. Read it. What word does Python use to tell you it doesn't recognize your spelling of "print"?
______________________________________________________________________

### AI corner

Remember: everything on your laptop (each thing is called a "file") has a location. There are 2 different ways to give instructions TO one of these locations: absolute and relative path.

- An absolute path is the complete address of a file, starting from the very root of your computer's hard drive. It doesn't matter where your terminal is "currently standing" -- the root is the same. This is like giving someone GPS coordinates, which are the same no matter where you are in the world. An absolute path looks like this:

```/Users/sheoli/Desktop/Projects/Teaching_Code/Unit_0/hello.py```

- A relative path is directions FROM where your terminal currently is to a file. So if your terminal changes folders, a relative path will break unless you update your directions. This is like telling someone who you know is standing a block down from you to "walk up a block" to get to you. A relative path looks like this if your terminal is in the same folder a hello.py:

```hello.py```

Use an AI tool of your choice to figure out answers to these questions:

- If you open your terminal, type "cd Desktop" and hit enter. Then open up a new terminal window (Cmd + N) and try to run hello.py (which should be saved on your Desktop). Does it work? Why or why not?

- I have two different commands I could type into a Mac terminal to run a file. A: python /Users/student/Desktop/code/myscript.py and B:python myscript.py. Which of these two will work no matter which folder I'm currently in?

- Look at these commands a programmer typed:

```pwd
Terminal prints: /Users/student/Documents
cd Projects
pwd
# Terminal prints: /Users/student/Documents/Projects
python hello.py
# Terminal prints: No such file or directory```

-   Based on the absolute paths printed by pwd, where on the computer is the terminal currently looking for hello.py? If the file is actually sitting out on the main Documents folder, how did the programmer accidentally break their relative path?
______________________________________________________________________

### What next?

Now that we have the basic tools installed (Python and the IDE) and understand roughly how things run and how to find files, we can start working inside the IDE and writing more complex code than just "Hello, world!"

Unit 1 will be about introducing how Python handles text and data without overwhelming computers.