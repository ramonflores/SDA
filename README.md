# Scan Domain Architecture

Scan Domain Architecture (SDA) is an script created with the purpose of doing some things easier when you are working with domains in proteins. SDA takes an **input file** in FASTA format with some amino acid sequences or as a PFAM list, and an **annotation list** (in [trinotate][1] format) and return a file with the coincidences or similarities found.


## Requirements
To get a better experience, there are some considerations you have to take before start using SDA.

* SDA was developed in a UNIX/Linux environment, so it might not work if you use it on a Windows or MAC environment.
* SDA is a script developed with Perl v5.18.2. We didn't use any version pragma, so we hope you can use it no matter your Perl  version.
* SDA uses the Perl module **SVG** to make graphics. You have to install this module to make SDA works.
* You have to get the [**HMMER suite**][2] to make SDA works. For SDA we use HMMER v3.1b1.
* You also need the **Pfam-A.hmm** file, this file is used for searching and getting some useful information about the input file. For this work, we use the Pfam version 29 (February, 2016), you might download it from **FTP->releases->Pfam29.0->Pfam-A.hmm.gz** on the pfam site [pfam.xfam.org/][3].
* For the GUI, you need Java 7 or later.


## What does SDA do?
With SDA you can get almost the same as with the pfam site but with some differences. SDA creates the summary table of the **hmmscan** for the input, a file with the coincidences (or similarities) and frecuencies of each PFAM architecture, and a file with the graphics of the architecture for the FASTA sequence(s).

An important difference is that SDA not only shows coincidences, SDA is capable to show similarities. This similarities may help you to understand some things or, make you doubt about some other things.


## Finally
We really hope this work might be useful for you because that is its purpose. Check the [SDA user guide.pdf](https://github.com/ramonflores/SDA/blob/master/SDA%20user%20guide.pdf) to know more about SDA.



## Contact
We will feel it great if you test this script and make us greetings, comments or report us any bug or fail. Please, contact us.

Ramon Flores (ramon.flores.r@outlook.com)

[1]: http://trinotate.github.io/
[2]: http://hmmer.org/
[3]: http://pfam.xfam.org/
