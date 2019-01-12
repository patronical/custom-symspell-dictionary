# custom-symspell-dictionary
customized frequency dictionary and spell-check

Special words need special care with spell-checking.
A standard dictionary may correct them into something else.
The SymSpell Frequency dictionary is update to include special words.
Common examples of special words may include acronyms and names.

"new_dictionary.ipynb"
A Jupyter Notebook is used to import a corpus containing known-good special words.
As an example, the Bhagavad Gita is used:
https://www.holybooks.com/wp-content/uploads/The-Bhagavad-Gita-Translation-by-Shri-Purohit-Swami.pdf
The text is tokenized, and frequency checked.
The text frequencies are scaled to the standard dictionary frequencies.
The most common word "the" is used for scaling.
The special words are added to the standard dictionary.
The existing words have their dictionary frequencies updated.
A custom frequency dictionary is then generated.

"symspell_worksheet.ipynb"
A separate Jupyter Notebook is used for spell checking.
The SymSpell package is used that utilizes the custom dictionary.
This package supports two-word compound concatenations.
Spell check functions are implemented along with simple custom word tests.
