# Japanese-Frequency-Analysis

Project Context:
In linguistics, a lexeme is the set of forms that a word, or more specifically a single semantic value, can take on in a language regardless of the number of ways it can be modified through inflection.

A lemma is the dictionary form of a word that is chosen by the conventions of its individual language to represent the entirety of the lexeme.

Lemmas and word stems are different in that a stem is the portion of a word that remains constant despite morphological inflection while a lemma is the base form of the word that represents the distinct meaning of the word regardless of inflection.

When studying a language, multitudes of different approaches can be taken. One method of efficient study is to memorize or learn the base form of a concept, or the lemma, and through the application of the grammatical rules of the language, begin to incorporate the remainder of the lexeme into their usage.

More information on lemmas can be found on its corresponding Wikipedia page:
(https://en.wikipedia.org/wiki/Lemma_(morphology%29))


Project Goals:
This project examines the frequencies of lemmas in the Japanese language, and what factors influence those frequencies, in order to determine a more efficient approach towards Japanese second language acquisition and the ordering of teaching materials for this purpose.

Efficiency will be measured by the estimated frequency, and thus number of applications or general usefulness, that learning a word will give, assuming that the student can apply grammatical rules to utilize all appropriate forms of the word, as determined by the frequency of the lemma in the Internet Corpus.

Additionally, the part of speech that each lemma is classified as will be used to look into ideas for a more efficient order of learning various sets of grammatical rules in Japanese.


Data Sources:
- The lemma dataset can be found hosted at http://corpus.leeds.ac.uk/frqc/internet-jp.num and similar datasets for other languages can be found at http://corpus.leeds.ac.uk/list.html

- The Part of Speech distribution frequency dataset can be found athttp://corpus.leeds.ac.uk/frqc/internet-jp-pos.num

- The JLPT tier dataset was created from this webpage https://www.nihongo-pro.com/kanji-pal/list/jlpt

- The Kanji .json dataset is found athttps://thekanjimap.com/kanji.html

- Character information is additionally gathered from http://www.edrdg.org/cgi-bin/wwwjdic/wwwjdic?1C


Main Findings:
1. Lemma frequency is most strongly affected by its length and both total and average character stroke counts.

2. When weighting the importance of learning a lemma, kanji and hiragana script words should be prioritized more.

3. While longer lemmas are generally used less frequently, the lemmas included in the JLPT n5 exam vocabulary list should be made exempt from negative weighting from length due to the type of hiragana words in this category.

4. A more efficient Japanese learning order will have the largest focus on nouns, verbs, and adjective syntax, but will cover auxiliary verb, conjunction, and particle rules in earlier stages.


Visualizations for Presentation:
1. The 'Frequency by Lemma Length', 'Frequency by Lemma Total Stroke Count', and 'Frequency by Lemma Average Character Stroke Count' plots all have extremely similar trend lines, which means that lemma length, lemma total stroke count, and lemma average character stroke count all have similar impacts on a lemma's frequency. Combining these as subplots on a single plot makes this comparison clear.

2. The 'Lemma Frequency by Script' plot shows that while the differences in medians and interquartile ranges among the script types show the varying importance of focusing on each script, the sheer number of extremely high frequency outliers in the hiragana script is worth discussion and study alone.

3. The 'Lemma JLPT Level by Frequency' plot shows the distributions of each JLPT level's frequencies. While the n5 exam has only the third highest median and third quartile of the scripts, it also has the most outliers and the highest frequency values of all. When compared to the 'Lemma JLPT Level by Lemma Length' plot, the reason for this becomes apparent: the JLPT n5 exam has the highest mean and range of lemma length.

4. The 'Distribution of Lemma Parts of Speech' shows the ratio of each lemma part of speech, with nouns, verbs, and adjectives having the most representation by far. Comparing this information with the 'Lemma Average Character Stroke Count' and 'Lemma Average Character Frequency' plots shows why language ordering cannot be only based on ratios, as three of the least common parts of speech in the dataset are shown to have the highest average character frequencies.
