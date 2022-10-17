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

# Method 
There are 5 parts 
 * Access Data
 * Tranfrom Data
 * Text preprocessing
 * Model
 * Similarity view
 
![Imgur](https://i.imgur.com/Pvkfwcu.jpg)

### Access Data 

![image](https://user-images.githubusercontent.com/96813273/196077109-ed02b6d9-7cfc-464a-8b07-3c2b59e65a70.png)

Make a selection of the specified data used is the Excel file data.
  **Node Repository is**
  **Excel Reader**
  
![image](https://user-images.githubusercontent.com/96813273/196077397-af05fb98-4d35-4667-98da-89608a96803f.png)

### Result

![image](https://user-images.githubusercontent.com/96813273/196077432-8072c3d0-50fd-4d89-8a75-52420271df08.png)

### Tranfrom Data

![image](https://user-images.githubusercontent.com/96813273/196077452-7760fb60-254d-46ee-8b41-2cdf06d7cee0.png)

![image](https://user-images.githubusercontent.com/96813273/196077497-443405d4-2940-4ab1-a7ed-677c1e030904.png)

**Node Repository is**
 * **Column Filter** 
 
![image](https://user-images.githubusercontent.com/96813273/196077526-bff31188-740b-4064-828c-2cf5b58a7ea3.png)

![image](https://user-images.githubusercontent.com/96813273/196077559-bfd8ff32-5689-4da7-be42-fa893b717cbe.png)

![image](https://user-images.githubusercontent.com/96813273/196077573-52d37430-8d55-436a-bfb5-abf405af906f.png)

 * **Transpose**
 
![image](https://user-images.githubusercontent.com/96813273/196077594-0db504d0-0079-4b6d-ac7b-cb296ac1c4cc.png)

![image](https://user-images.githubusercontent.com/96813273/196077608-1677848a-f6df-4761-9ffe-3d4d22291c2a.png)

![image](https://user-images.githubusercontent.com/96813273/196077620-33a684d1-696c-4bae-b9b4-1201de90859a.png)

 * **Column Combiner**
 
![image](https://user-images.githubusercontent.com/96813273/196077646-7a0ab52e-628c-41c3-9122-8b8bd003a827.png)

![image](https://user-images.githubusercontent.com/96813273/196077653-6e6abf8f-2963-4543-aff5-b7b22b9393ff.png)

 * **Column Filter**
 
![image](https://user-images.githubusercontent.com/96813273/196077689-77ec58b5-0d69-4316-992a-865560ad120e.png)

![image](https://user-images.githubusercontent.com/96813273/196077699-5fbd28b5-18f6-47ef-b772-73eb1783b77a.png)

![image](https://user-images.githubusercontent.com/96813273/196077711-1f41105c-5f9a-4cf1-b71e-1c71b85fb2d9.png)

 * **Column Appender**
 
![image](https://user-images.githubusercontent.com/96813273/196077802-d0cb1961-9383-4b1f-a0f1-cb2631515d07.png)

 * **Table Creator**
 
![image](https://user-images.githubusercontent.com/96813273/196077836-cd624c6a-1c30-4654-b1b2-55cad5f418d0.png)

![image](https://user-images.githubusercontent.com/96813273/196077863-495c44dc-ec68-40e1-adcc-cfba63e48fb4.png)

* **String Manipulation**

![image](https://user-images.githubusercontent.com/96813273/196077891-1db2f70b-aac7-42dd-8dd2-80796bd2f6ab.png)

### Text preprocessing

![image](https://user-images.githubusercontent.com/96813273/196077938-fa06edab-3b94-448f-8ff6-5f563681adda.png)

![image](https://user-images.githubusercontent.com/96813273/196077961-77297e97-498f-48d9-b7ae-42fc37275701.png)

In this step we will remove the symbolic words and eliminate the words that are (a,The),Then convert all letters from uppercase to lowercase.and abbreviate them to be the same word
Then remove the numerical words and spread the word. **Node Repository used is**
 * **String s to Document**
 
![image](https://user-images.githubusercontent.com/96813273/196078011-2950d9ca-c921-411a-a5bc-33bc45665108.png)

* **Column Filter**

![image](https://user-images.githubusercontent.com/96813273/196078026-fe55d79c-a03d-4876-8891-51171aca085d.png)

 * **Punctuation Erasure**
 
![image](https://user-images.githubusercontent.com/96813273/196078040-49333749-60d0-4d96-afa0-2eac0ea3362a.png)

![image](https://user-images.githubusercontent.com/96813273/196078067-6951db0b-d24c-4dc4-9534-f39e939de786.png)

 * **Case Converter**
 
![image](https://user-images.githubusercontent.com/96813273/196078106-8ac5e57b-b681-4b24-9cb8-ab55f7887778.png)

 * **Stop Word Filter**
 
![image](https://user-images.githubusercontent.com/96813273/196078128-a49502d9-219a-43e9-b681-40d1cef50e33.png)

 * **POS Tagger**
 
![image](https://user-images.githubusercontent.com/96813273/196078159-af853de7-7032-4bef-9fb0-be0e1608adbc.png)

* **Stanford Tagger**

![image](https://user-images.githubusercontent.com/96813273/196078176-89aa0ad1-7af8-4212-8d61-68a60af260f2.png)

* **Stanford Lemmatizer**

![image](https://user-images.githubusercontent.com/96813273/196078212-b825e047-10b0-431f-ac8f-aa9a6376b6f3.png)

![dish](https://user-images.githubusercontent.com/96813273/196081396-524af257-a219-4e11-a4fa-2f8ea9c1fa41.JPG)

* **Bag Of Words Creator**

![image](https://user-images.githubusercontent.com/96813273/196079779-513077d8-5632-4158-a8c2-f390e9c6aaa7.png)

### Result

![image](https://user-images.githubusercontent.com/96813273/196079805-d0439f12-cc66-4166-910d-9e4c7896ecfc.png)

### Model(TF-IDF)

![image](https://user-images.githubusercontent.com/96813273/196079853-212ded46-5d0f-4d22-8a27-cf4aa3bfbdc8.png)

In this step, the frequency values in each row will be determined (TF) Then again all the frequencies in the document.The TF and IDF values are then multiplied together to find a greater accuracy.
Then the words are put together using nodes **document vecter**and select the column and row filter to make the similarity search is to compare similar values.

![image](https://user-images.githubusercontent.com/96813273/196079912-55d64207-327d-4a7c-a06e-213c9d36ccda.png)

**Node Respository used is**
* **TF**
 * **Column Rename**
 * **IDF**
 * **Math Formula**
### Result

![image](https://user-images.githubusercontent.com/96813273/196080002-b0e32a16-1da2-4689-aaf5-0210e777f553.png)

 * **Document Vecter**

![image](https://user-images.githubusercontent.com/96813273/196080040-ce632f0f-a671-4d8e-b417-2b9c321a8d27.png)

### Result 

![image](https://user-images.githubusercontent.com/96813273/196080115-5676f265-46fa-4c9f-be53-c715d169590d.png)

 * ** Table Creator **

![image](https://user-images.githubusercontent.com/96813273/196080133-727cad5f-3b00-486b-9b68-d4e2972ff410.png)

![image](https://user-images.githubusercontent.com/96813273/196080143-52f0a6f2-ef88-4637-a7f0-e872de98b685.png)

#### Similarity View

![image](https://user-images.githubusercontent.com/96813273/196080168-f632966e-6419-48d1-8b1a-a72f1868068d.png)

* ** Column Appender**

![image](https://user-images.githubusercontent.com/96813273/196080190-2ecc760e-65f8-428b-8fb8-5c4117802dc1.png)

![image](https://user-images.githubusercontent.com/96813273/196080207-f44b03fa-3dd1-4cc3-b4aa-d5af08640830.png)

* ** Sorter**

![image](https://user-images.githubusercontent.com/96813273/196080234-aa4e6906-7947-4f74-8492-31978ef93c6a.png)

### Result

![image](https://user-images.githubusercontent.com/96813273/196080307-5fac2d41-fc21-4aaa-b65e-2dce2fed9d2c.png)

  * **RowID**

![image](https://user-images.githubusercontent.com/96813273/196080329-910b218a-4e4a-4f82-88dd-0fc0db6caa08.png)

* **Cosine**

![image](https://user-images.githubusercontent.com/96813273/196080372-401d206e-01f1-403c-b08f-5d57f28e9f6d.png)

![image](https://user-images.githubusercontent.com/96813273/196080456-2af445da-f2bf-4aa5-bf33-9b967ff3567d.png)

![image](https://user-images.githubusercontent.com/96813273/196080491-4aa6b31a-6f1c-4cd7-8fe1-8202471bbc6e.png)

![image](https://user-images.githubusercontent.com/96813273/196080514-7fbe4c84-d9d5-455b-9ffc-e3c481c9f041.png)

![image](https://user-images.githubusercontent.com/96813273/196080531-6369f412-d3ed-40b9-9b2a-5e095c6cdc68.png)

# Conclusion

And the goal of text mining is to find out how much synonyms in each translation have been measured as a percentage.

# Suggestions














