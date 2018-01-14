# RNN-TV-Script-Generation
Applyting Recurrent Neural Network to generate TV scripts. Developed as coursework in the "Deep Learning Fundamentals" Nanodegree @ Udacity. This project passed all specifications as shown in the project information section

## Project Information
- The function create_lookup_tables create two dictionaries: vocab_to_int and int_to_vocab
- The function token_lookup returns a dict that can correctly tokenizes the provided symbols.
- Implemented the get_inputs function to create TF Placeholders for the Neural Network with Input, Target and Learning Rate placeholders.
- Enough epochs to get near a minimum in the training loss, no real upper limit on this. Just need to make sure the training loss is low and not improving much with more training.
- Batch size is large enough to train efficiently, but small enough to fit the data in memory. No real “best” value here, depends on GPU memory usually.
- Size of the RNN cells (number of units in the hidden layers) is large enough to fit the data well. Again, no real “best” value.
- The sequence length (seq_length) here should be about the size of the length of sentences you want to generate. Should match the structure of the data.

## Results

The TV Script generated and have similar characteristics to the original tv scripts, the results are pretty fun! The following TV script was generated:

homer_simpson:(beligerent) oh, you'd like that wouldn't you, ya...

carl_carlson: hey, i'm worried.

homer_simpson: i've had just about enough of you.

moe_szyslak: so we, uh... homer's been gone a drunk.

moe_szyslak:(covering nervous laughing) i got hooked on this stuff in the service.

homer_simpson:(quietly) hi, moe. this is why... that's all right.

moe_szyslak:(sighs) what's the point?... same ol' stinkin' world... ah, i'm gonna be sick tonight.

barney_gumble: hey moe, you wanna smell my flower?

moe_szyslak:(genuinely enthused) do i?!

moe_szyslak:(laughs) usually people that tease me get thrown out on their ass. but, uh, your sayin' it made me feel good. jeez, i can't less of my blood and sweat are in this drink.

moe_szyslak: anyway, you got it, moe.(shuts off) so goodbye...

chief_wiggum:(singing) so you better make that call to the plow king.

homer_simpson: how could you, barney? after all you,(tearfully) you get that car?

moe_szyslak: oh, what? i suppose you've seen a bigger star?

homer_simpson:(coy) i might have.

lenny_leonard: come on, there's sexy bald like...

moe_szyslak:(while poking, friendly) so, hey, did you see the game last night?

...

seymour_skinner: homer, still not private?

moe_szyslak: sure, we're



