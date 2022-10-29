# Week 5 Lab Report

## Researching Commands
### *grep* commands and options

- *grep -v*  

The following are an example:

command:
```
grep -v "a" technical/911report/chapter-1.txt
```

This outputs:
```



"WE HAVE SOME PLANES"  



INSIDE THE FOUR FLIGHTS
.
.
.
IMPROVISING A HOMELAND DEFENSE
.
.
.
United Airlines Flight 175
.
.
.
    Center: Do you know who he is?
.
.
.
    FAA: Yes.
.
.
.
    FAA: Yes.
.
.
.
    NEADS: He's down?

    FAA: Yes.


    NEADS: Oh, he's down? Down?
.
.
.
NATIONAL CRISIS MANAGEMENT
.
.
.
The Agencies Confer
.
.
.
```

The three "**.**" in vertical signifies large spaces. 
#
command:
```
grep -v "o" technical/biomed/rr37.txt
```
This outputs:
```




        sharply since the late 1970s, which may reflect increasing
        4], despite recent therapeutic advances. Understanding the
        characteristics, health care access, and disease severity 
        22].
        care access.



          24, 25, 26]. Each subject underwent a structured,       
          care.
          Physicians registered 669 eligible patients. After      
          interviews (
          n = 539), we later restricted the
          survey interviewer [ 26, 27]. This restricted data set  
          the 371 baseline subjects, the present study excludes an
          study findings.
          (
          n = 371) with registered subjects (

          race/ethnicity (62% versus 71%;
          P < 0.001 and
          P = 0.10, respectively). There were
          P > 0.15 in all cases).




          aspirin sensitivity at baseline interview. Since
          Generic health status was measured using the Medical


          Statistical analysis
          (SAS Institute, Cary, NC, USA). We evaluated the



        Results

          Health care access


          race/ethnicity (71%).


          bivariate analysis
          risk (OR, 11.6; 95% CI, 5.3-25.2). Other clinical
          Better baseline generic physical health status (SF-36)
          2.5; 95% CI, 1.1-5.5).


          analysis
          severity.
          repeated the multivariate analysis excluding these
          (OR, 1.2; 95% CI, 1.03-1.4).



        sharply in the USA since the late 1970s [ 2].
        asthma severity and health status, suggesting that greater
        results.
        13]. African-American asthma patients similarly had a
        may explain these variable results.
        30].
        Because adults with asthma treated by specialists


        therapy.


        Supplementary material



          increments (less than $5000, $5001-$10,000, $10,000
          We measured generic health status using the Medical



```
#
command:

```
grep -v "i" technical/plos/journal.pbio.0020001.txt
```
This outputs:
```











        2002).


            Canada?




        programs.


        journals (
        Nature and
        to the top 11–20 journals.
        In


        A Long Road Yet to Travel
        world.







```




*grep -v* inverts the sense of matching, to select non-matching lines. Hence, it grabs all the nonmatching lines and outputs it in the terminal. 
#

- *grep -i*

The following are an example:

command:
```
grep -i "north" technical/911report/chapter-1.txt
```
This outputs:
```
About five minutes after the hijacking began, Betty Ong contacted the American Airlines Southeastern Reservations Office in Cary, North Carolina, via an AT&T airphone to report an emergency aboard the flight. This was the first of several occasions on 9/11 when flight attendants took action outside the scope of their training, which emphasized that in a 
hijacking, they were to communicate with the cockpit crew. The emergency call lasted approximately 25 minutes, as Ong calmly and professionally relayed information about events taking place aboard the airplane to authorities on the ground...(some more text)
```
#
command:

```
grep -v -i "a" technical/911report/chapter-1.txt
```

This outputs:
```






INSIDE THE FOUR FLIGHTS
.
.
.
    Center: Do you know who he is?
.
.
.
```
The three "**.**" in vertical signifies large spaces. 
#

command:

```
grep -i "north" technical/biomed/rr37.txt
```
This outputs:
```
from physician practices in Northern California. Details
```

*grep -i* ignores case distinctions in patterns and input data, so that characters that differ only in case match each other.
#
- *grep -c*

command:
```
grep -c "local" technical/911report/*  
```
This outputs:
```
technical/911report/chapter-1.txt:3
technical/911report/chapter-10.txt:1
technical/911report/chapter-11.txt:3
technical/911report/chapter-12.txt:13
technical/911report/chapter-13.1.txt:7
technical/911report/chapter-13.2.txt:1
technical/911report/chapter-13.3.txt:4
technical/911report/chapter-13.4.txt:1
technical/911report/chapter-13.5.txt:4
technical/911report/chapter-2.txt:3
technical/911report/chapter-3.txt:14
technical/911report/chapter-5.txt:2
technical/911report/chapter-6.txt:1
technical/911report/chapter-7.txt:6
technical/911report/chapter-8.txt:5
technical/911report/chapter-9.txt:4
technical/911report/preface.txt:0
```
#
command:
```
grep -c "calls" technical/911report/chapter-1.txt
```
This outputs:
```
6
```
#
command:
```
grep -c -v "calls" technical/911report/chapter-1.txt
```
This outputs:
```
725
```

*grep -c* suppress normal output. Instead, it prints out a count of matching lines for each input file. When combined with -v, it would count the non-matching lines.