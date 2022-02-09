tags:
#python
#computer_science


# How do Computer Programs Work?
- computers programs work by using many simple instructions ontop of other simple instructions to perform tasks
- Computers cannot innately understand instructions in something such as english: they need a **language** they understand

## What is a Language
- language is used all over the world
- We undaerstand **natural languages**, or languages devolped over time such as english, German, Korean, Hindu, Arabic, Mandarin, and more
- Computers understand language throuhg simple **Instrictions**. We call these **Instruction lists**, or IL for short. They are **Machine Languages**
- Different computers understand different languages. For example, a windows machine knows powershell and DOS. A linux machin will probably know BASH (Bourne Again Shell). They can both learn languages like Javascript, Ruby, and **Python**. Both of them natively understand Binary.
### What Makes a Language
Languages consist of 4 main elements:
- An **alphabet** - "a set of symbols used to build words of a certain language" 
	- "the Latin alphabet for English, the Cyrillic alphabet for Russian, Kanji for Japanese"
- A **lexis** - Words understood in a language, such as print, make, see, etc
	- Words understood in a language, such as print, make, see, etc
- A **syntax** - Rules on the order of things
	- Think of <u>grammar</u> for natural languages
	- Think of the <u>order of arguments</u> in machine languages
- **Semantics** - Does it make sense?
# Compilation vs Interpretation
There are 2 ways of changing programs from high level languages to machine code: **compilation** vs **interpretation**
## Compilation
in compilation the program is compiled once as the entire program. This is amde into a file such as a .exe, or one of the many choices on linux. This contains the machine code.
### Advantadges
- compiling once at the start allows for some performance gains
- This is easiest for normal people to use as they don't have to have the installer
- easiest to distribute code, as all of the code needed could be contained withing the executable
- Code that has been compiled is harder to understand and steal
### Disadvantadges
- Changes are slow - program must be compiled each time to run
- programs must be compiled for different operating systems: this can grow cumbersome, especially for enterpiese software that needs to support multiple approaches
## Interpretation
In interpretation, code is shipped as is, and is made into machine code on the sport by an **interpreter**.
### Advantadges
- Allows for faster testing
- Programs can be more dynamic
- Programs can run on any computer that has an interpreter
### Disadvantadges
- Program must be interpreted each time it is ran - a bottleneck for some alrger applications
- end users must have the interpreter and pckages installed to run the code
## How does the Interpreter Function?
- Programs are just text, so we put our code into text files to allow them to run
- programs must be written in **Pure Text** or **Plain Text**. This means
	- No images
	- no media
	- no decorations like fonts
	- Programs may still contain unicode characters, such as emoji or certian special characters, as these are just rendered plaintext items (such as this article)
- Interpreters read left to right, top to bottom, line by line
- If the compiler finds an error, the task is exited with an error code. You may be told where the error might be, but this can be misleading
- The interpreter then executes the line of code. This can be follows in the process "read-check-execute"
- Programs that use interpreters are called scripting languages, and the programs they use are called scripts
## Is Python Interpreted or Compiled
- Python is an **Intepreted Language**
- You need the **Python interpreter** to run python code. Luckily, it is **Free**, both in the sense of cost and *libre*, or free to do with as you want.
# What is Python?
- Python is a high level object oriented programming purpose used for a lot o thigns
- the create is **Guido can Rossum**
- The creator names the language after [Monty Python's Flying Circuis](https://en.wikipedia.org/wiki/Monty_Python%27s_Flying_Circus), A comedy show that you may recognize from **Monty Python and the Holy Grail**
## What Were the Goals of Python?
In 1999, the goals for python were outlined by Guido van Rossum. His goals were:
- "an **easy and intuitive** language just as powerful as those of the major competitors"
- "**open source**, so anyone can contribute to its development"
- "code that is as **understandable** as plain English"
- "**suitable for everyday tasks**, allowing for short development times."



# Key Vocabulary
- Natural Language - human spoken languages
- Programming Language - Machine languages such as Java, Python, Powershell, and more
- Instruction List - a set of instructions from a **programming Language** that a computer understands
- Syntax - the structure of a language, both natural and machine
- Source code - the source programming language ran by an interpreter
- Source file - the file that contains the source code for a program
- Interpreted Language - a **programing language** that utilizes an interpreter to run its code
- Editor - a text editor, as that is all source files are
- Console - a space to interact with programing languages. Sometimes called a console, it interfaces with languages to accomplish tasks.
- Debugger - a tool that runs through your program line by line to find errors and report them back to the programmer. It is **YOUR** job to fix them
- IDLE - Integretad learning and Development Environment, Sometimes just refered to as an IDE. Contains most of the tools necessary for coding a specific language, or multiple depending on the setup.
