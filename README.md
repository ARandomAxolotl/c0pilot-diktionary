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
