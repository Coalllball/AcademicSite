---
title: "From Punchcard to Unicode: A Brief History of Character Encoding"
date: 2022-02-11T15:04:23.066Z
draft: false
featured: false
authors:
  - admin
image:
  filename: featured
  focal_point: Smart
  preview_only: false
---
## Background

Characters are undoubtedly the most critical factor in every enduring civilization, driving the continued growth and development of culture and society. From the Cuneiform script of ancient Babylon to the Oracle script of ancient **China**, writing is the only long-standing visual practice in the history of visualization in human society. Many significant transformations have taken place in the history of character evolution to meet the new needs of humankind. As the world has entered the digital age, new challenges have come to light. Since the groundbreaking of the telegraph and the significant breakthroughs in computing technology, characters have needed to find a new form that better accommodates the high demands of human society for faster and more reliable recording and transformation. As a result, generations of intelligent people have dedicated their lives to adapting written-based characters to digital environments around the world in order to keep their unique cultures and histories thriving in the digital age, and to give them greater opportunities to achieve new heights in the new era. This report provides a brief history of the shift of written symbols to the digital environment and describes how people who use a character system different from English have worked to adapt their cultures to the new age.

## Process

Since there is a vast amount of documentation and literature on the development of character encoding in modern history, this report is best served by presenting the history through a timeline visualization. The visualizations used in this report were created by [TimelineJS](https://timeline.knightlab.com/), a powerful open-source tool developed by Knight Lab. TimelineJS provides creators with a simple tool that allows their readers to explore through different points in time and to be informed by reading the authors’ annotations and viewing illustrations of events.

The timeline used in this report contains three main periods, namely the foundation, development, and integration of the character encoding system evolution. The primary resources include [Character Encoding (2014)](https://link-springer-com.ezaccess.libraries.psu.edu/chapter/10.1007/978-1-4302-6653-2_19) and [CJK Information Processing (2009)](https://books.google.com/books?id=SA92uQqTB-AC&lpg=PA94&hl=zh-CN&pg=PA94#v=onepage&q&f=false).

## Findings

### **The foundation**

#### The Morse Code

The need to convert information through signals emerged before mankind entered the digital age. Morse code was a revolutionary innovation that turned the way people communicate upside down. With dots and dashes, messages could travel across continents with virtually no wait time, compared to physical mail. Morse code, however, was not the first character coding system. Long before the telegraph was introduced, people used beacons or flag semaphores to convert messages over long distances; however, Morse code was the first system to have a standard encoding method for each character in the English alphabet. It is also a non-negligible basis for the contemporary character encoding system.

#### The Punched Tape

When computers were first created, human-computer interaction as we know it today had not yet been invented. In the 1950s and 1960s, computers did not have keyboards and displays, and all input and output work had to be done using punched tapes. These tapes tell the computer how to perform some complex operations by conveying data and commands in binary code (0 or 1) and storing the results of the operations on other punched tapes. Initially, there was no uniform standard for how to use punched tapes to represent data, thus resulting in much unnecessary waste of resources. Therefore, in the 1960s, the American Standards Association led a project to develop a common code for data processing, which became ASCII (American Standard Code for Information Interchange).

![International Morse Code by Damon Self](https://i0.wp.com/studentwork.prattsi.org/infovis/wp-content/uploads/sites/3/2022/02/1_1mOO6Lmh9ASEp_BRZvOJKQ-1024x682.jpeg?resize=840%2C559&ssl=1 "International Morse Code by Damon Self")

![](https://i0.wp.com/studentwork.prattsi.org/infovis/wp-content/uploads/sites/3/2022/02/93217b38-2285-46c4-9308-c15dc6ad5af0_800x600.jpg?resize=800%2C532&ssl=1 "Computer paper tape with eight channels by CLIVE (MAX) MAXFIELD")

### **The development**

#### ASCII

ASCII was born in 1963 and was the first character coding system to be created in the modern sense. The introduction of ASCII was a major breakthrough in the history of human-computer interaction, allowing humans and computers to understand the same data simultaneously. For example, when a human wants to type a string of characters `HELLO` (in upper case) into a computer, the computer queries the ASCII table and stores it in memory as a binary code, i.e. `010010000100010100010011000100110011001111`. And conversely, when a computer wants to express `HELLO` to a human, instead of recognizing a string of binary numbers, he/she can read the text directly. Along with the creation of other human-computer interaction hardware, human-computer communication has become more efficient, and the key to everything is based on ASCII.

#### High ASCII

Although ASCII perfectly solved the core problem of human-computer interaction, its early days contained only 26 English alphabet letters and some punctuation and mathematical symbols. This meant that people could only communicate with computers in English, and for speakers of other languages, the efficiency improvements that computers offered were not significant. After years of refinement, ASCII contains 255 characters and their corresponding binary forms, covering the languages of most European countries. As Asian countries grew rapidly in the 1980s, they were eager to find a new character encoding system to join the wave of the digital age.

#### Asian Character Sets

In the 1980s, Asian countries began designing character encoding systems to support their languages in order to take advantage of the conveniences of the computer and digital age. For example, Chinese computer scientists invented the GBK character encoding to enable computers to recognize Chinese characters, Japan invented Shift_JIS, and Korea invented Euc-kr. However, despite the existence of so many character encoding systems, most of them only support their national languages and English. There is a  lack of a universal standard.

![US-ASCII Code Chart. 1972 by an unknown officer or employee of the United States Government](https://i0.wp.com/studentwork.prattsi.org/infovis/wp-content/uploads/sites/3/2022/02/1280px-USASCII_code_chart-1-1024x737.png?resize=840%2C605&ssl=1)



![](https://i0.wp.com/studentwork.prattsi.org/infovis/wp-content/uploads/sites/3/2022/02/ascii.png?resize=564%2C457&ssl=1)

Low & High ASCII Chart form [text-symbols.com](<>)

![](https://i0.wp.com/studentwork.prattsi.org/infovis/wp-content/uploads/sites/3/2022/02/cjk-typeface-google.jpg?resize=800%2C408&ssl=1)

*Sample shared characters in Chinese, Japanese, and Korean* by Timothy Saar

### **The integration**

#### Unicode

In the 1990s, the international organization ISO developed the Unicode character encoding system to enable universal support for all languages; Unicode uses 16 – 32 binary bits to correspond to a character, allowing it to support more characters than ASCII and other national character encoding systems do. As a result, it enables people from different regions and cultures to communicate with computers smoothly.

#### UTF-8

However, it was soon discovered that although Unicode solved the problem of unified character encoding, it took up more space and affected the quality of data transmission to the extent that garbled codes often appeared. In order to solve these problems, Unicode devised a wonderful solution, the UTF encoding rules, by using bytes of different lengths to read Unicode, ensuring that users in different regions could read characters in different languages at the same time without being affected, which greatly enhanced the popularity of the Internet.

![](https://i0.wp.com/studentwork.prattsi.org/infovis/wp-content/uploads/sites/3/2022/02/maxresdefault-1024x576.jpg?resize=840%2C473&ssl=1)

Unicode logo & Sample Characters by Unicode Consortium

![](https://i0.wp.com/studentwork.prattsi.org/infovis/wp-content/uploads/sites/3/2022/02/UTF8-t-1024x538.jpg?resize=840%2C441&ssl=1)

UTF-8 logo

### Reflection

This report only briefly reviews the history of character encoding and summarizes the challenges encountered in its development through a comparison of character encoding systems in Europe, the United States, and Asia. Unfortunately, due to length limitations, character encoding systems used in other countries and regions are not covered in this report. For example, Arabic, Hindi, and Cyrillic. The users of these languages have also worked very hard to develop their languages at this time in history. Without their efforts, Unicode and the Internet would not have been available. I will continue to explore these stories as I get the chance. In the meantime, this report does not go into the technical details of character encoding, which is also worth discussing in a possible follow-up project.

### References

SmartBear.com. “Ancient Computer Character Code Tables – and Why They’re Still Relevant.” Accessed February 1, 2022. <https://smartbear.com/blog/ancient-computer-character-code-tables-and-why-the/>.

Diana. “Overview.” *Unicode* (blog). Accessed February 1, 2022. <https://home.unicode.org/basic-info/overview/>.

“History of Character Encoding.” Accessed February 2, 2022.<http://latel.upf.edu/morgana/altres/cibres/unicode/pnoerr1.htm>.

“History of Unicode.” Accessed February 3, 2022. <https://www.unicode.org/history/>.

Lunde, Ken. *CJKV Information Processing*. Book, Whole. Beijing; Cambridge; O’Reilly, 1999. <https://go.exlibris.link/XBM93KlL>.

Sharan, Kishori. “Character Encodings.” In *Beginning Java 8 Fundamentals: Language Syntax, Arrays, Data Types, Objects, and Regular Expressions*, edited by Kishori Sharan, 727–37. Berkeley, CA: Apress, 2014. <https://doi.org/10.1007/978-1-4302-6653-2_19>.

“World Power Systems:Texts: Annotated History of Charactercodes.” Accessed February 10, 2022. <https://www.sr-ix.com/Archive/CharCodeHist/index.html>.