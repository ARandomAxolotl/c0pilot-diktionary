# c0pilot++

yes, copilot but dumber

## Controls

- Green flag: regenerate

- `space`: switch views:

    - history

    - "copy this"

    - nothing

- `t`: toggle text-to-speech (might randomly not work, idk why)

- `x`: clear history

- `d`: toggle debug mode:

- pauses after every word

- press `enter` to generate the next word




## About

For those advanced, this is basically a bigram model.

Inside there's the old c0pilot code.

It is:

- much slower (around 2x slower than c0pilot++)

- less efficient

- no longer receives vocab updates

c0pilot++ uses the updated system.



## Adding vocabulary

Add new words using the format:

word{

nextword:weight

}

Higher weight = more likely to appear.

Example:

hello{

friend:5

world:2

}

You can also use multi-word tokens:

hello{

good morning:5

}

## Known issues

- This is a bigram model.

- c0pilot means:

    - "Microsoft Copilot" = stupid

    - "0" = "0 guaranteed meaning"
- c0pilot++ vocab parser has "bugs":

   `This is a feature, not a bug`

Example:

word{

word2{

word1:67

}

This is valid.

`word` and `word2` can both lead to `word1`.


## Changelogs : 

c0pilot 1.0 : existed and abandoned

c0pilot 1.1 : forked to c0pilot++ 1.0

c0pilot++ 1.0 : remake parser, no bug fixed as those are `features`

c0pilot++ 1.1 : added LOTS of vocab

c0pilot++ 1.2 : using the bugs, made the vocab file much smaller and efficient

c0pilot++ 1.3 : added bakanohana so it can sing

c0pilot 1.2 : minor updates to fit the new system

c0pilot++ 1.4 and c0pilot 1.3 : added vocab files to github

c0pilot++ 1.5 : more words!
