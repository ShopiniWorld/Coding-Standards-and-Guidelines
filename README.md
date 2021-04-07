# Coding Standards and Guidelines


Good software development organizations want their programmers to maintain to some well-defined and standard style of coding called coding standards.


##  Purpose of Having Coding Standards:

* A coding standard gives a uniform appearance to the codes written by different engineers.
* It improves readability, and maintainability of the code and it reduces complexity also.
* It helps in code reuse and helps to detect error easily.
* It promotes sound programming practices and increases efficiency of the programmers.

--------------------------------------------------
### Avoid using a coding style that is too difficult to understand:
`Code should be easily understandable. The complex code makes maintenance and debugging difficult and expensive.`

--------------------------------------------------
### Length of functions should not be very large:
`Lengthy functions are very difficult to understand. That’s why functions should be small enough to carry out small work and lengthy functions should be broken into small ones for completing small tasks.`

--------------------------------------------------
### Commenting and Documentation:

```
Commenting the code is very important. People can't read other people's minds. Commenting serves two purposes:
1. to ensure that the code is written as desired. This form of comment is usually put in the code before the code is written. It serves as a means of ensuring that the code does what it is supposed to do.
2. to ensure that the code is described in sufficient detail such that anyone else looking at the code can easily understand the design and the purpose of the code.
```
------------------------
### Proper and Consistent Scheme for Naming
| Identifier Type	 | Rules for Naming	 | Examples |
| :---         |     :---:      |          ---: |
| Packages   | The prefix of a unique package name is always written in all-lowercase ASCII letters and should be one of the top-level domain names. | com.sun.eng     com.apple.quicktime.v2     edu.cmu.cs.bovik.cheese |
| Classes     | Class names should be nouns, in mixed case with the first letter of each internal word capitalized.       | class Raster;  class ImageSprite;  |
| Interfaces     | Interface names should be capitalized like class names.	      | interface RasterDelegate;                interface Storing;      |
| Methods     | Methods should be verbs, in mixed case with the first letter lowercase, with the first letter of each internal word capitalize.        | run();                runFast();              getBackground();           |
| Variables     | Except for variables, all instance, class, and class constants are in mixed case with a lowercase first letter. Internal words start with capital letters. Variable names should not start with underscore _ or dollar sign $ characters, even though both are allowed. Variable names should be short yet meaningful. The choice of a variable name should be mnemonic- that is, designed to indicate to the casual observer the intent of its use. One-character variable names should be avoided except for temporary "throwaway" variables. Common names for temporary variables are i, j, k, m, and n for integers; c, d, and e for characters.       | int  i       char c           float myWidth         |
| Constants     | The names of variables declared class constants and of ANSI constants should be all uppercase with words separated by underscores ("_"). (ANSI constants should be avoided, for ease of debugging.)       |   static final int MIN_WIDTH = 4;   static final int MAX_WIDTH = 999;   static final int GET_THE_CPU = 1;              |


It is up to the choice of the developer which naming scheme to be used but it is very important to maintain the consistency of the naming scheme throughout the code. CamelCase is used in Java while PHP uses underscore in the naming convention.

-----------------------------------------
### Principle of DRY
```While coding, the coders should remember the principle of DRY, which stands for Don’t Repeat Yourself, also known as DIE (duplication is evil). It is a good practice to write your own code and don’t copy. It is a known fact that most software programs aim at automating repetitive tasks. Therefore, the code of the application should be such that the same code is not repeated over and over again.```

-----------------

### Deep nesting structure should be avoided
Too many nesting structures make it difficult to understand the code.
It is, therefore, advisable to avoid using deep nesting. For Instance:
```
if() {

    if() {

        if() {

            // logic here

        }

    }

}

```





