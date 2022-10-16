# Quran-Similarity
Subject : Data mining 
# Overview
   This part of this work what I learned in the data mining section.This is a text mining, program using a program called KNIME.By using the data as an Excel file in the translation section of the Holy Quran from Surah Al Fatiha, which includes translations from 14 recognized translators.
 1.  Abdul haleem 
 2.  Pickthal 
 3.  Yusuf ali 
 4.  Fadel soliman 
 5.  ghali 
 6.  Ibu kathir 
 7.  Maarif 
 8.  Maulana wahiduddin khan 
 9.  Mufti taqi usmani 
10.  Muhammad taqi ud din al hilali amp Muhammad muhsin khan 
11.  Mustafa khattab 
12.  Ruwwad 
13.  Tafheem adul ala maududi 
14.  irv                                 
        And the goal of text mining is to find out how much synonyms in each translation have been measured as a percentage. 
# Method 
There are 4 parts 
 * Access Data
 * Tranfrom Data
 * Text preprocessing
 * Model
### Access Data 
Make a selection of the specified data used is the Excel file data.
   Node Repository is
  **Excel Reader**
### Tranfrom Data
In this step will be used **row filter** to select which part of the information you want and continue to select until 13 rows are complete and make **GroupBy** all row filter
and then weld them all together by **concatenate**Then change from the **strings to document.**

Node Repository is
 * **Row Filter** 
 * **GroupBy**
 * **Concatenate**
 * **Strings to document**
### Text preprocessing
In this step we will remove the symbolic words and eliminate the words that are (a,The),Then convert all letters from uppercase to lowercase.and abbreviate them to be the same word
Then remove the numerical words and spread the word. Node Repository used is
 * **Punctuation Erasure**
 * **Stop Word Filter**
 * **Case Converter**
 * **Snowball stemmer**
 * **N Chars Filter**
 * **Bag of Words Creator**
### Model(TF-IDF)
In this step, the frequency values ​​in each row will be determined (TF) Then again all the frequencies in the document.The TF and IDF values ​​are then multiplied together to find a greater accuracy.
Then the words are put together using nodes **document vecter**and select the column and row filter to make the similarity search is to compare similar values,Node Respository used is
 * **TF**
 * **IDF**
 * **Math Formula**
 * **Document Vecter**
 * **Column Filter**
 * **Row Filter**
 * **Similarity Search**
# Results
#### Access data

![Imgur](https://i.imgur.com/PbdX3Uq.jpg)
![Imgur](https://i.imgur.com/SG5aAmn.jpg)
![Imgur](https://i.imgur.com/XG8Bmsi.jpg)
![Imgur](https://i.imgur.com/1Roy7RB.jpg)
![Imgur](https://i.imgur.com/IvdaYP7.jpg)
![Imgur](https://i.imgur.com/SX0kwmb.jpg)
![Imgur](https://i.imgur.com/oxLPTyi.jpg)
![Imgur](https://i.imgur.com/5IOPVMg.jpg)
![Imgur](https://i.imgur.com/gg9udLu.jpg)
![Imgur](https://i.imgur.com/AAKoMbK.jpg)
![Imgur](https://i.imgur.com/BTNU6fY.jpg)
![Imgur](https://i.imgur.com/pfEjxGR.jpg)
![Imgur](https://i.imgur.com/fD5kfjR.jpg)
![Imgur](https://i.imgur.com/Ove3exg.jpg)
![Imgur](https://i.imgur.com/D0X7Spp.jpg)
![Imgur](https://i.imgur.com/l6uCcur.jpg)
![Imgur](https://i.imgur.com/81Vepjg.jpg)
![Imgur](https://i.imgur.com/Plxj80k.jpg)
![Imgur](https://i.imgur.com/PD58zE0.jpg)



