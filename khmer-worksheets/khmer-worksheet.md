# Multiple Choice Khmer Quiz Generator

Generate a multiple choice quiz with 10 questions to test Khmer vocabulary.

## Instructions

1. **Select 10 random words** from the khmerwords.json file
2. **Create multiple choice questions** with the following format:
   - Present the **English word** as the question
   - Provide **4 Khmer options** (a, b, c, d)
   - One option is the correct translation
   - Three options are incorrect (distractors from other words in the vocabulary list)

3. **Answer distribution**: Ensure the correct answers are evenly distributed:
   - Approximately 2-3 questions should have answer A as correct
   - Approximately 2-3 questions should have answer B as correct
   - Approximately 2-3 questions should have answer C as correct
   - Approximately 2-3 questions should have answer D as correct

4. **Format each question** as follows:

   ```
   Q1. What is "english word" in Khmer?
   a) khmer-option-1
   b) khmer-option-2
   c) khmer-option-3
   d) khmer-option-4
   ```

5. **Provide an answer key** at the end in this format:
   ```
   Answer Key:
   1. A
   2. C
   3. D
   etc.
   ```

## Requirements

- Use real words from the khmerwords.json vocabulary list
- Make distractors plausible (don't use obviously unrelated words)
- Randomize the order of questions
- Ensure correct answers are balanced across all four options (a, b, c, d)

---

# Matching Section Generator

Generate a matching section with 10 words and 10 answers to test Khmer vocabulary. Matching sections should not exceed 10 words and 10 answers. if instructed to make more than 10 matching questions, a new section must be built.

## Instructions

1. **Select 10 random words** from the khmerwords.json file
2. **Create two columns**:
   - Left column: Numbers (1-10)
   - Right column: Letters (A-J)
3. **One-to-one matching**: There are exactly 10 matches (no distractors, no multiple correct answers)
4. **Randomize the right column** so answers don't align with the left column
5. **Format** - English words and Khmer answers should be on separate lines for easy copy/paste into word processors:

   ```
   Match the English words with their Khmer translations:

   1. english-word _____
   2. english-word _____
   3. english-word _____
   ...
   10. english-word _____

   A) khmer-word
   B) khmer-word
   C) khmer-word
   ...
   J) khmer-word
   ```

6. **Provide an answer key** at the end in this format:
   ```
   Answer Key:
   1-D, 2-A, 3-F, 4-C, 5-J, 6-B, 7-E, 8-H, 9-G, 10-I
   ```

## Requirements

- Use real words from the khmerwords.json vocabulary list
- Ensure the right column (A-J) is shuffled and not in order

---

# Sentence Unscrambling Generator

Generate sentence unscrambling exercises with 5-8 sentences to test Khmer sentence structure.

## Instructions

1. **Select words** from the khmerwords.json file to create grammatically correct Khmer sentences
2. **Sentence types** - Create a mix of:
   - **Single clause sentences** (4-5 words): Simple subject-verb-object with modifiers
   - **Two clause sentences** (6-8 words): Use transition words like hai-nung (and), bpon-dtae (but), bpee-bprooah (because)
   - **Multiple clause sentences** (9-10 words): Combine multiple clauses with transition words
3. **Transition words available** in khmerwords.json:
   - and: hai-nung / nung
   - but: bpon-dtae / dtae
   - because: bpee-bprooah / bprooah / daoy-sa
   - also: gaw
   - if: baur / baur-sen
   - so: anh-jing / doj-ch'neh
   - then: bon-dtoab-mok
   - after: bon-dtoab-bpee / graowee
   - before: bpee-mun / mun-bpayl
4. **Scramble the word order** of each Khmer sentence
5. **Present only scrambled Khmer words** (no English in the questions)
6. **Provide lines for students to write**:
   - One line for the correctly ordered Khmer sentence
   - One line for the English translation
7. **Format**:

   ```
   1. Scrambled: psa / dtow / knyom / sa-aik
Khmer: __________________________________________________________________________________
English: _________________________________________________________________________________
   2. Scrambled: hai-nung / rean / layng / goad / knyom
Khmer: __________________________________________________________________________________
English: _________________________________________________________________________________
   ```

8. **Provide an answer key** at the end with both Khmer and English:
   ```
   Answer Key:
   1. Khmer: knyom dtow psa sa-aik | English: I go to the market tomorrow
   2. Khmer: goad rean hai-nung knyom layng | English: He studies and I play
   etc.
   ```

## Requirements

- Use real words from the khmerwords.json vocabulary list
- Include a variety of sentence lengths (4-10 words)
- Use transition words to create compound and complex sentences
- Ensure sentences are grammatically correct in Khmer
- Do not include English in the scrambled questions, only in the answer key

---

# Fill in the Blanks Generator

Generate fill-in-the-blank exercises with 8-10 sentences entirely in Khmer.

## Instructions

1. **Create Khmer sentences** using words from khmerwords.json file
2. **Sentence types** - Create a mix of:
   - **Single clause sentences** (4-5 words): Remove 1 key word
   - **Two clause sentences** (6-8 words): Remove 1-2 key words, use transition words like hai-nung (and), bpon-dtae (but), bpee-bprooah (because)
   - **Multiple clause sentences** (9-10 words): Remove 2 key words, combine clauses with transition words
3. **Transition words available** in khmerwords.json:
   - and: hai-nung / nung
   - but: bpon-dtae / dtae
   - because: bpee-bprooah / bprooah / daoy-sa
   - also: gaw
   - if: baur / baur-sen
   - so: anh-jing / doj-ch'neh
   - then: bon-dtoab-mok
   - after: bon-dtoab-bpee / graowee
   - before: bpee-mun / mun-bpayl
4. **Remove 1-2 key words** from each sentence (replace with __________)
5. **Sentences must be entirely in Khmer** (no English in the sentences themselves)
6. **Provide a word bank** with all the missing words plus 3-5 distractor words
7. **Format**:

   ```
   Fill in the blanks with the correct Khmer words:

   **Word Bank:** sa-aik / sala / lan / kdaw / aan / tom / neang / rean / klean / cheu / dtrow / joub / tmey / ga-ngea / joal-jet / saj-moan / dtinh / la-or / cafe / bi-yea / twer / pteah / dtuk / bay / sok-sabay

   1. knyom dtow psa __________.
   2. neang rean nau __________.
   3. knyom __________ nau sala bpayl-pruk hai-nung twer __________ bpayl-l'ngeaj.
   ```

8. **Provide an answer key**:
   ```
   Answer Key:
   1. sa-aik
   2. sala
   3. rean, ga-ngea
   etc.
   ```

## Requirements

- Use real words from the khmerwords.json vocabulary list
- Sentences must be entirely in Khmer
- Include a variety of sentence lengths (4-10 words)
- Use transition words to create compound and complex sentences
- For longer sentences (9-10 words), use 2 blanks
- Provide a word bank with all answer words plus 3-5 distractor words
