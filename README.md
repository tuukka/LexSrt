# LexSrt
The purpose of this script is to get all the senses for all the words in a SRT-file from Wikidata

It uses SpaCy to tokenize each subtitle in the srt and looks up the corresponding lexeme in 
Wikidata based on the detected position of speech and token representation.

# Limitaitons
* Hard-coded to English
* No API

# Installation
Clone the repository.

# Use
`python main.py -i path-to-srt.srt`

You can fiddle with the configuration options in `config.py`

# Example subtitle Ice Age
![image](https://github.com/dpriskorn/LexSrt/assets/68460690/f07d14a4-45cb-45cb-a617-889604652639)

The script encourages the user to contribute to Wikidata if 
senses are completely missing.

# License
GPLv3+ with the exeption of the code borrowed from Ordia, see the licens in the file.

# Thanks
Big thanks to Finn Nielsen for writing the spaCy->lexeme function. 
I improved it a bit for my purposes to get what I wanted.

# What I learned
* Having your own classes is nice. 
* Reusing easy to read quality code from others is nice
* Reusing classes from other projects is nice
* WBI is still lacking convenince methods I want so I'll
propose them to be included upstream to make life easier for others.
* Pydantic and black goes a long way, I don't really need all the other linting mypy stuff for whipping up working code like this in a few hours. Stability is good enough for me with those two and the inspection in PyCharm.
