# Readability

to run the code type

```terminal
python readability.py
```

## background

According to Scholastic, E.B. White’s Charlotte’s Web is between a second- and fourth-grade reading level, and Lois Lowry’s The Giver is between an eighth- and twelfth-grade reading level. What does it mean, though, for a book to be at a particular reading level?

Well, in many cases, a human expert might read a book and make a decision on the grade (i.e., year in school) for which they think the book is most appropriate. But an algorithm could likely figure that out too!

So what sorts of traits are characteristic of higher reading levels? Well, longer words probably correlate with higher reading levels. Likewise, longer sentences probably correlate with higher reading levels, too.

A number of *“readability tests”* have been developed over the years that define formulas for computing the reading level of a text. One such readability test is the **Coleman-Liau index.** The Coleman-Liau index of a text is designed to output that (U.S.) grade level that is needed to understand some text. The formula is `index = 0.0588 * L - 0.296 * S - 15.8` where *_L_* is the average number of letters per 100 words in the text, and *_S_* is the average number of sentences per 100 words in the text.

Let’s write a program called readability that takes a text and determines its reading level. For example, if user types in a line of text from Dr. Seuss, the program should behave as follows:

```python
$ ./readability
Text: Congratulations! Today is your day. You're off to Great Places! You're off and away!
Grade 3
```

The text the user inputted has *_**65** letters_*, *_**4** sentences_*, and *_**14** words_*.
>**65** letters per **14** words is an average of about **464.29** letters per 100 words (because 65 / 14 * 100 = 464.29).
>

>And 4 sentences per 14 words is an average of about 28.57 sentences per 100 words (because 4 / 14 * 100 = 28.57).
>

>Plugged into the [**Coleman-Liau formula**](https://en.wikipedia.org/wiki/Coleman%E2%80%93Liau_index), and rounded to the nearest integer, we get an answer of 3 (because 0.0588 * 464.29 - 0.296 * 28.57 - 15.8 = 3): so this passage is at a third-grade reading level.
>

### little disclaimer

the check50 resulted in errors. def sum wrong with my code, somebody go fix that please!!!

#### smaller disclaimer
[Academic Honesty](https://cs50.harvard.edu/x/2020/honesty/)
Written by myself!!!