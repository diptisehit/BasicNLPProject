# Normalizing Textual Data in NLP >> NLP Pre-processing

Text Normalization transforms text into a consistent format improves the quality and makes it easier to process in NLP tasks.

Key steps in text normalization includes:

1. Regular Expressions (RE) are sequences of characters that define search patterns.
   
2. Tokenization is a process of splitting text into smaller units called tokens.

3. Lemmatization reduces words to their base or root form.

4. Stemming reduces works to their root by removing suffixes.

5. Stopword removal is a process to remove common words from the document.

6. Parts of Speech (POS) Tagging assigns a part of speech to each word in sentence based on definition and context.
   
![twilio_NLP](https://github.com/user-attachments/assets/82036038-d11c-483f-b824-a1d39f03e7ff)


# 1. Lexical analysis
Lexical analysis deciphers and segments language into units—or lexemes—like paragraphs, sentences, phrases, and words. NLP algorithms categorize words into parts of speech (POS) and split lexemes into morphemes—meaningful language units that you can’t further divide. 

There are 2 types of morphemes:

1. Free morphemes function independently as words (like “cow” and “house”).

2. Bound morphemes make up larger words. The word “unimaginable” contains the morphemes “un-” (a bound morpheme signifying a negative context), “imagine” (the free morpheme root of the whole word), and “-able” (a bound morpheme denoting the root morpheme’s ability to end).

   The analysis isolates and divides the first sentence into lexeme phrases, like “the understandable vocabulary that makes up a language.” This analysis further divides the phrase into word lexemes, like “vocabulary” and “language,” categorizing both as noun POS. Then, the analysis derives free morphemes, like “words,” “vocabulary,” and “understand-,” and bound morphemes, like “-able.”

# 2. Syntactic analysis
Syntax describes how a language’s words and phrases arrange to form sentences. Syntactic analysis checks word arrangements for proper grammar.

For instance, the sentence “Dave wrote the paper” passes a syntactic analysis check because it’s grammatically correct. Conversely, a syntactic analysis categorizes a sentence like “Dave do jumps” as syntactically incorrect.

# 3. Semantic analysis
Semantics describe the meaning of words, phrases, sentences, and paragraphs. Semantic analysis attempts to understand the literal meaning of individual language selections, not syntactic correctness. However, a semantic analysis doesn’t check language data before and after a selection to clarify its meaning.

For instance, “Manhattan calls out to Dave” passes a syntactic analysis because it’s a grammatically correct sentence. However, it fails a semantic analysis. Because Manhattan is a place (and can’t literally call out to people), the sentence’s meaning doesn’t make sense.

# 4. Discourse integration
Discourse describes communication between 2 or more individuals. Discourse integration analyzes prior words and sentences to understand the meaning of ambiguous language.

For instance, if one sentence reads, “Manhattan speaks to all its people,” and the following sentence reads, “It calls out to Dave,” discourse integration checks the first sentence for context to understand that “It” in the latter sentence refers to Manhattan.

# 5. Pragmatic analysis
Pragmatism describes the interpretation of language’s intended meaning. Pragmatic analysis attempts to derive the intended—not literal—meaning of language.

For instance, a pragmatic analysis can uncover the intended meaning of “Manhattan speaks to all its people.” Methods like neural networks assess the context to understand that the sentence isn’t literal, and most people won’t interpret it as such. A pragmatic analysis deduces that this sentence is a metaphor for how people emotionally connect with places.
