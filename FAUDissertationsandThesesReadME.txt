A LaTeX2? Document Class for Dissertations and Theses
This is the home page of the fauthesis.cls class file. This file is designed to allow students at Florida Atlantic University to create dissertations and theses using the LaTeX document preparation system that comply with the University's Graduate Thesis and Dissertation Guidelines. Its was written by Chris Beetle (cbeetle AT physics DOT fau DOT edu), of the Department of Physics.
Important Note
Version 1.0 of the class file has been revised in close collaboration with the Graduate College, but is still awaiting final approval. I'll post an additional update here, or remove this comment, when I receive word from the Graduate College. I will aim to do this no later than November 1, 2014. Until then, please use this new version as it incorporates all of the major revisions in the University's Graduate Thesis and Dissertation Guidelines.
Disclaimers and Related Stuff
Please note that this class file does not supplant the University's manuscript guidelines. While the Graduate College has reviewed the output it generates, and found it generally acceptable, they do not support or maintain it. Using this class file makes it more likely, but does not guarantee, that your thesis format will be approved by the Graduate College. Students should read and understand the manuscript guidelines so that any problems can be identified as early as possible.
It would also be a good idea to examine the Graduate College's procedures and deadlines for submission of theses well before your intended graduation date.
The class file is an independent effort on the part of its author, and will be supported by him in the immediate future. Students who find bugs or other problems should contact the author directly, not the Graduate College, with their questions. I (have grown weary of the third person and) will make every effort to work with individual students to resolve issues promptly while moving the class file out of beta status and into a suitable state for final release. However, please note that the class file is provided as-is, and with no guarantee that it will produce output acceptable to the Graduate College.
Downloads
The following five files are available.
User's Guide
The User's Guide offers detailed instructions for using all features of the document class. I know, I know, you don't need no stinkin' manuals. Until you do.
[ fautug.pdf output | fautug.tex source ]
Sample Thesis File
The sample thesis offers a complete, working source file using the fauthesis document class. It should compile immediately when placed in the same directory as the fauthesis.cls file. A quick look at this file should make it clear to 90% of students how to set up their thesis. But bear in mind that the sample file merely illustrates a "plain vanilla" case. If you don't have a Department Chair, but instead have a Director, or if you have a Co-Advisor on your thesis committee, then I'm afraid you may have to crack open the manual. Sorry.
[ fausample.pdf output | fausample.tex source ]
Source Code
The class file contains all of the code needed to create documents using this document class.
* To install, copy the .cls file linked below into the directory containing the .tex source of your thesis. Change the first line of the source file to "\documentclass[options]{fauthesis}" and you're ready to go.
* LaTeX will probably give several errors the first time you compile your .tex source using the fauthesis class, especially if your thesis has previously been formatted using another thesis template, style or class file. You will have to edit your source to make it work. Follow these steps:
o Obviously, be sure to save a copy if you already have a working file.
o Copy the preamble (lines 1 through 50) from the sample thesis source file linked above into the preamble (the bit before the \begin{document}) of your own source file. Modify them as needed. It should be fairly clear what they do.
o Copy the front matter (lines 51 through 77) from the sample thesis source file linked above into your own source file, putting them just after the \begin{document}. Modify the arguments of the vita, acknowledgements, abstract, and dedication commands as needed, but do not alter their order. If your thesis contains tables, then change \nolistoftables to \listoftables. Again, it should be pretty clear what's going on.
o If you have been using another thesis template, style or class file, then it is time to remove or comment out any code that previously generated the title, copyright, signature, vita, acknowledgements, abstract, or dedication pages. Also, remove or comment out any code that modified the chapter or other section headings.
o If you have been loading the geometry package (\usepackage[...]{geometry} in the preamble) or something like it, then don't. It is not compatible with the fauthesis class because it messes with the margins. See below for other common LaTeX packages known to conflict with the class file.
o You certainly may continue to define macros in the preamble of your source file, and to load most package files. Again, see below for known conflicts.
[ fauthesis.cls source ]
Known Conflicts
* The geometry package, and all packages that modify the document margins or page layout, are incompatible with the fauthesis class for obvious reasons.
* The sectsty package modifies how chapter headings are typeset in a way that violates FAU's 2-inch margin requirement for the top of the page beginning a new chapter.
Links
* The LaTeX Project has a great set of links to resources for learning how to use LaTeX and the many, many packages available for it.
* The LaTeX WikiBook is surprisingly comprehensive, offers introductions to many packages, and always remains free.
* The Comprehensive TeX Archive Network (CTAN) is a world-wide system of servers that mirror a complete collection of all available TeX packages. See their starter page if you need to get the software and get up to speed.

