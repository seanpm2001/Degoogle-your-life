
***

## Project language file

The **project language file** is a script file that talks about itself, inserted into all projects that sets/denotes the intended/current majority programming language. It is used to increase the amount of 1 programming language over another, or give the project a programming language (even if the project isn't programming related)

Project language files can be written in any language that [GitHub](https://github.com) will highlight on the code percentage section (such as Python (blue), JavaScript (yellow), HTML (orange) and more) This discludes markdown, xml, svg, rst, mediawiki, yaml, ini, and many more types.

Project language files are just a decoration, they are completely separate from the project. Removing them should not (and will not) affect functionality. Project language files are always placed at the root of the projects directory.

The syntax goes as follows:

1. `// Start of script` (line)

2. Comment with the program output

3. Normal programming language headers and imports (`#include`, `int main()`, `etc`)

4. An output statement with the same output as 1 (above)

5. Commented file info

6. `// End of script (line)`

For python projects, or projects with input/output, this is how it goes:

1. `# Start of script` (line)

2. Comment with the program output

3. Normal programming language headers and imports (`#include`, `int main()`, `etc`)

4. An output statement with the same output as 1 (above)

5. Exit condition output input (ie: `noMore = input("Press [ENTER] key to quit")` )

6. Quit string for when any input is given, that stays on the screen until the window closes (usually: `print("The program has now been closed. If the window is still open, try pressing the close button. If this doesn't work, end the process/task with a task manager/process manager")` )

7. Commented file info

8. `# End of script` (line)

For languages that let you title the program (such as Eiffel, FORTRAN, BASIC, and many others) the program name is usually written as `projectLanguageFile`, `languageFile`, or something else that is similar, as follows:

1. `// Start of script` (line)

2. Comment with the program output

3. Normal programming language headers and imports (`#include`, `int main()`, `etc`)

4. Program name (`appName = "projectLanguageFile"`)

5. An output statement with the same output as 1 (above)

6. Commented file info

7. `// End of script` (line)

The syntax is written differently depending on the programming language, but it always follows this order.

The comment for a project language file is usually related to a pun or something related to the name of the project, or what the project is mostly written in. Some examples being:

> The Tiny Tower image repo is written in **Eiffel**, as it is the only programming language I know based off a tower (like the **Eiffel** tower)

> My battery image repository is written in **Assembly**, as batteries typically require **assembly**.

> My mountain image repository is written in **C**, as I can **C** (see) the mountain from my house

> My AdVenture Capitalist image repository is written in **C++**, as **C++** has classes, capitalism also has economic classes. In reverse, my AdVenture Communist image repository is written in **C**, as **C** was originally a classless language, and Communism doesn't have economical classes.

However, sometimes I can't come up with a pun. Some exceptions have been made for this:

> Projects related to a farm or ranch are normally written in **Vala**.

> Projects that are for something I don't like too much are written in languages I don't like that much, such as **Go** (2009 language by Google)

This is all the info you need to know about the project language file system by Sean Patrick Myrick (seanpm2001)

***

## File info

File type: `Markdown (*.md)`

File version: `1 (Wednesday, December 23rd 2020 at pm)`

Line count (including blank lines and compiler line): ` `

***
