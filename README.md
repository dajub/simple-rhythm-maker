# simple-rhythm-maker

This is a straight forward neural net for generating rhythms. Beats were transcribed using alphabetical representation (e.g. h = hi-hat, hb = hi-hat and base, r = rest) ahd broken into 16th notes. These were then converted into one-hot encoded arrays  upon which the LSTM neural net trained to learn which notes follow which others. It then outputted sequences of notes which were converted back into drum notes. This is basically the same type of character neural net one would use to learn speech, just instead of a spoken language it is musical notes. 

This was primarily a chance to get acquanted with neural networks and to investigate whether or not people would be able to or thought they would be able to pick out which rhythms were made by the machine and which by me. From the NN side, much more data is needed. There are large data bases of transcirbed drum files which would just need some manipulating to get into the desired format. Here I myself transcribed some simeple rhythms but that should not be done. Further, 48th notes allows for a lot more variety of rudiemtns, combinging duple and triplet based possibilities which I would do in a subsequent iteration. Lastly, for actually testing these outloud, the stiff sound of a machine reading the notes to produce audio makes any rhythm sound robotic and therefore I would ddvice adding in some small randomness into the note sounds. You can make produce the drum noises fairly easily with randomness using [Chuck](https://chuck.cs.princeton.edu/) or [Max_MSP](https://cycling74.com/). 
