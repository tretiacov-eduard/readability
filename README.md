Text Analyzer

This C program analyzes a given text and calculates the Coleman-Liau index, a readability index designed to gauge the understandability of a text for the average reader. The program takes user input for the text and outputs the corresponding grade level.
How to Use

    Compile the Program

    Before running the program, ensure you have a C compiler installed. If not, you can install one such as GCC.

    bash

gcc text_analyzer.c -o text_analyzer

Run the Program

Execute the compiled program.

bash

./text_analyzer

Input Text

Enter the text when prompted.

plaintext

Text: This is an example text. It contains sentences, words, and letters. Enjoy analyzing it!

View Result

The program will output the calculated grade level based on the Coleman-Liau index.

plaintext

    Grade 8

How it Works

    The program calculates the number of letters, words, and sentences in the input text.
    It then computes the Coleman-Liau index using the formula: index = 0.0588 * L - 0.296 * S - 15.8, where L is the average number of letters per 100 words, and S is the average number of sentences per 100 words.
    The resulting index is used to determine the reading grade level of the text.

Functions

    count_letters(string text): Counts the number of letters in the input text.
    count_words(string text): Counts the number of words in the input text.
    count_sentences(string text): Counts the number of sentences in the input text.

Example

For the input text:

plaintext

This is an example text. It contains sentences, words, and letters. Enjoy analyzing it!

The program calculates:

    Letters: 81
    Words: 18
    Sentences: 3

The Coleman-Liau index is then computed, resulting in a grade level of 8.
Note

    The program assumes proper sentence structure with spaces after periods and appropriate word spacing.