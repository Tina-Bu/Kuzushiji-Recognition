# Kuzushiji-Recognition

This is a Kaggle competition hosted by https://www.kaggle.com/c/kuzushiji-recognition.

## What is Kuzushiji?

Kuzushiji, a cursive writing style, was used in Japan for over a thousand years, beginning in the 8th century. Over 3 millions books, on a diverse array of topics such as literature, science, mathematics and cooking are preserved today. However, the standardization of Japanese textbooks known as the “Elementary School Order” in 1900, removed Kuzushiji from regular school curriculum, as modern japanese print became popular. As a result, most Japanese natives today cannot read books written or printed just 120 years ago.

Since Chinese characters entered Japan in the 8th century, the Japanese language has been written using Kanji (Chinese characters in the Japanese language) in official records. However, from the late 9th century, the Japanese began to add their own character sets: Hiragana and Katakana, which derive from different ways of simplifying Kanji. Individual Hiragana and Katakana characters don't contain independent semantic meaning, but instead carry phonetic information (like letters in the English alphabet).

In Kuzushiji documents, Kanji, Hiragana and Katakana are all used. However, the number of character types in each document varies by genre. For example, story books are mostly written in Hiragana while formal records are written mainly in Kanji.

**Challenges in Kuzushiji recognition**

**Large number of character types:** The total number of unique characters in the Kuzushiji dataset is over 4300. However, the frequency distribution is very long-tailed and a large fraction of the characters (Kanji with very specific meaning) may only appear once or twice in a book. Therefore, the dataset is highly unbalanced.

**Hentaigana:** One characteristic of Classical Hiragana or Hentaigana (“character variations'') is that many characters which can only be written a single way in modern Japanese can be written in many different ways in Kuzushiji. 
For example, this image shows that Hiragana *Ha* (は) can be written in a few different ways. 

**Similarity between characters:** A few characters in Kuzushiji look very similar and it is hard to tell what character it is without considering the above character as context.
For example, in the image below the red circles show 3 types of characters: *Ku* (く), an iteration mark and *Te* (て).

**Connectedness and overlap between characters:** Kuzushiji was written in a cursive script, and hence in many cases, characters are connected or overlap which can make the recognition task difficult. 
In the image below, the bounding boxes in the image below show that characters overlap. The color of the boxes are for visualization and don’t contain any specific meaning. 

**Various layouts:** The layout of Kuzushiji characters (while normally arranged into columns) does not follow a single simple rule, so it is not always trivial to express the characters as a sequence. Some examples of this include characters being written to wrap around or even integrate into illustrations. Sometimes, characters are written in a diagonal line. 

https://www.kaggle.com/c/kuzushiji-recognition/overview/about-kuzushiji



