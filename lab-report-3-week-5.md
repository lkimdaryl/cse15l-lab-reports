# Week 5 Lab Report

## Researching Commands
### *grep* commands and options

- *grep -v*: Inverts the sense of matching, to select non-matching lines  

The following are an example:
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
```
```
```

```




*grep -v* grabbed all the lines in the text but shows only the nonmatchnings lines. All the lines matching the "a" pattern are outputted as blank lines.

- **grep -i** : Ignores case distinctions in patterns and input data, so that characters that differ only in case match each other.

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

- **grep -c**: Suppress normal output; instead print a count of matching lines for each input file.  With the -v, --invert-match option (see below), count non-matching lines.