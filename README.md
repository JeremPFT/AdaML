# ChangeLog
## alpha version
Work in progress version. Keep tuned.

# Introduction
## What is AdaML?
- UML tailored for Ada 2012 programming language
- A modeling language to draw UML diagrams, implemented in PlantUML
- An easy way to learn Ada through the use of UML and OOP concepts

## Features
- UML tailored to use and show particular Ada language characteristics
- Coherent set of functions to design software components for Ada
- Generates high quality drawings (ps, eps) easy to embedded in other docs
- Easy to learn by example, both AdaML and Ada language

## What is /not/ AdaML?
- A model-based tool to generate Ada code
- A reverse engineering tool to draw UML diagrams from Ada code
- An interactive UML modeling or drawing tool

## Online Usage

## Local Usage
- [PlantUML](https://plantuml.com) installed and working in your system
- The AdaML files, check [AdaML](https://github.com/rocher/AdaML) installation
  instructions
- Your favorite text editor, preferably with PlantUML support (e.g. Emacs)
- Check the list of [supported editors](http://plantuml.com/running)
- For better visualization and integration with LaTeX, [computer
  modern](https://www.fontsquirrel.com/fonts/computer-modern) fonts

## Limitations
Make sure that the PlantUML environment you're using

- lets you use external files, not only a single piece of text
- the line `!include AdaML.puml` on top of your new files effectively includes
  the AdaML.puml file
- Still under development; feedback appreciated

# Online Usage
## Online Version - Quick Start
- Open [plantuml-previewer](http://sujoyu.github.io/plantuml-previewer)
- Remove default lines and paste the following code:

```
!include https://github.com/rocher/AdaML/raw/develop/AdaML.puml
begin_type("Pan_Dimensional")
  procedure("Ask_The_Question", "in out Natural")
end()

begin_package("Deep_Thought")
  function("Answer_The_Question", "", "Natural")
private()
  variable("The_Answer", "Natural", 42)
end()

depends("Pan_Dimensional", "Deep_Thought", "ask >")
#+end_example
```

## Embedded Diagrams in GitHub
- This is an example of the AdaML documentation:

<p align="center">
![test image](http://www.plantuml.com/plantuml/proxy?cache=no&src=https://raw.github.com/rocher/AdaML/develop/diagram/deep-thought.puml)
</p>

- Check the raw version of this `README.md` file to see the image link used
- The PlantUML source code can be found in GitHub here: (deep-thought.puml)[https://raw.github.com/rocher/AdaML/develop/diagram/deep-thought.puml]