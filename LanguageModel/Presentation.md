## Presentation Pronoun case error, Distributional Cues, *Acquisition*

### Introduction

1. English children make pronoun case errors

   Pronouns present a special case of the poverty of the stimulus problem (Chomsky 1980)

   Children are not uniform in their pronominal error production either. Some children produce many errors, others virtually none, although these differences could in part reflect sampling problems. Some children who make errors do so with a range of pronominal forms, others with only one particular pronoun type 

2. Some accounts: ATOM (nativism), Input and Usage Account

   Kirjavainen Theakson and Lieven Input Driven

   

### First study: The Corpus Analysis

#### Methods

1. I analyzed XX corpora, XX longitudinal, XX cross-sectional

2. selected criteria: 20-40 months

3. NLTK Python, %gra tier, SUBJ OBJ (accuracy rate)

4. What data I have about children: 

   Usage — words, pronouns, cased-pronouns, errors, number of each pronoun

   ATOM — verbs, tensed verbs, (+nounss)

   Input — same thing for parents

#### Results

##### General Data

1. Of all pronouns used by all children, only XX errors;  Of all pronouns used by adults, only XX errors 
2. Error rate for cross sectional children, Error rate for one-time children
3. Some charts 

##### Data Analysis

ATOM: errors — verbs/tensed verbs (##### FOUR VARIABLE TABLE)

Input: errors — parents everything

Usage: errors — words, pronouns, each pronouns

Developmental: errors — age/mlu 

1. Correlation: 

   Cross-sectional; Longitudinal (no significance)

2. Mixed Effects Linear Regression (no significance) POISSON 

3. Logistic Regression (no significance)



#### Why? What other accounts could explain children's acquisition on pronoun case?



#### 1. Pronoun case is a rare phenomenon

####2. The existing theories don't really work 



#### Do we need to account for this? 





#### Second Study: Distributional Cues (bigram, trigram)

#### Introduction

1. Toben (2002, 2004), St.Claire (2010)  Children can use distributional cues to learn word categories. 
2. Usage based people "let me go"  

##### Their Method

1. Generally limit which categories can be fomed on the basis of fixed frames, generally restricting learning to noun and verb categories

2. Flexible framework (From St.Clair et al., 2010): the preceding and succeeding word

3. Corpus in St.Clair and Mints: Anne and Aran, Eve, Naomi, Nina, Peter, younger than 30 months; coded on %MOR line, 95% accuracy (Sagae, MacWhinney and Lavie 2004)

4. Three fixed framework aX, Xb, aXb, One flexible framework aX + Xb

   #####  St.Clair et al Methods

   1. aX, Xb, aXb, basic stats
   2. feedforward neural network (200 hidden units)
   3. Adding hidden units
   4. train on most frequent frames

#### This study

##### Getting Data

1. Corpus: Peter, Nina, Naomi, Eve, (appeared before) + Abe, somebodyelse

2. get the aX, Xb, aXb, X as pronouns, tagged as NOM and ACC

   (some justification below)

##### Computational Model

1. Feedforward Neural Network (blackbox)

   a. aX (intrinsic train on parents, test on parents; extrinsic train on parents, test on children)

   b. Xb 

   c. aXb

2. Decision Tree (whitebox)

### Conclusion

1. One prediction is that languages mark accusative cases (like German on the articles, or Russian) would be easier for children to learn thus make less pronoun case errors. (Pelham 2011, "English-acquiring children frequently make pronoun case errors, while German-acquiring children rarely do. Nonetheless, German-acquiring children frequently make article case errors.")
2. 











### This study 

1. Before age 40 months: Peter, Eve, Nina, Naomi, 

2. baseline would be 0.5. if we randomly assign a case to the X, it's gonna be 0.5

3. first chart: (simple stats to see if framework is informative enough)

4. Accuracy: unique frame (NOM or ACC) (not including you and it) / all frame (including you and it) [rationale: children can't tell you and it from framework thus they will be seen as unvalid]

   aX

   Corpus  NOM Token          NOM Type       ACC Token        ACC Type

   Peter    297/447 = 0.66      93/161=0.57   192/202=0.95   63/93=0.67  

   Naomi 526/926 = 0.57      108/205 = 0.53  344/362 = 0.95  90/143 = 0.63

   Eve 	 629/1221=0.52    103/206=0.5        463/525=0.88   101/166=0.61

   Nina   2682/7778=0.34   218/500=0.44   2223/3159=0.70 259/543=0.48

   Xb

   Corpus  NOM Token        NOM Type         ACC Token          ACC Type

   Peter     375/444 = 0.84  128/209 = 0.61  132/205 = 0.64   62/103= 0.60
   
   Namoi  771/926 = 0.83 152/288 = 0.53 208/288 = 0.72    78/146 = 0.53
   
   Eve         936/1217=0.77 180/325=0.55    299/527=0.57    102/170=0.6
   
   Nina    3813/7766=0.49 442/1094=0.40 1218/3175=0.38 215/516=0.42
   
   aXb
   
   Corpus  NOM Token  NOM Type               ACC Token       ACC Type
   
   Peter    1.0                   301/320 = 0.94        1                      126/142=0.89

##### rational for treating all pronouns as NOM or ACC

1. errors are not equally made on each pronoun
2. errors on each pronoun are not related to input or total production
3. if we attribute it the error to something else
4. if we just wanna see how powerful the framework is
5. hypothesis: each pronoun has different framework, the more frequent framework will have less errors

1. 
2. 



```
*CHI:	can't she have dese [: these] ?
758	%mor:	mod|can~neg|not pro:sub|she v|have pro:dem|these ?
759	%gra:	1|4|AUX 2|1|NEG 3|4|SUBJ 4|0|ROOT 5|4|OBJ 6|4|PUNCT
```

```
*CHI:	there she goes .
4606	%mor:	adv|there pro:sub|she v|go-3S .
4607	%gra:	1|3|JCT 2|3|SUBJ 3|0|ROOT 4|3|PUNCT
```

Haggerty 

```
4297	*CHI:	when me <see Fra> [//] see he again ?
4298	%mor:	conj|when pro:obj|me v|see pro:sub|he adv|again ?
4299	%gra:	1|3|LINK 2|3|SUBJ 3|0|ROOT 4|3|OBJ 5|4|JCT 6|3|PUNCT
```

Brown/Eve/020100

```
662	*CHI:	the time we were given (.) is Land Before Time three .
663	%mor:	det:art|the n|time pro:sub|we aux|be&PAST part|give&PASTP cop|be&3S
664		n:prop|Land n:prop|Before n:prop|Time det:num|three .
665	%gra:	1|2|DET 2|6|SUBJ 3|5|SUBJ 4|5|AUX 5|2|CMOD 6|0|ROOT 7|8|NAME
666		8|6|PRED 9|10|MOD 10|8|OBJ 11|6|PUNCT
```

Weist/Matt/030810



