# Language

[Csound](https://csound.com/)

# Domain

Audio synthesis with real-time inputs

# Computational model

Csound code contains an instrument section and a score section.
The instrument section defines parameters of each different instrument used (constant throughout the program runtime), and the score section defines when different events occur after initial execution.
Thus, Csound can be used as a sequencer to synthesize audio patterns.
However, the program can also read real-time inputs from devices such as MIDI keyboards to play sounds and apply effects at times defined during the program runtime.

# DSL-ness

I would say this is more on the domain-specific side of the spectrum even edging a bit past since it has very limited functionality (I don't think you can even create a "hello world" program since there are no strings).
The code is mostly definitions with limited freedom on functions that can be applied.

# Internal or external?

Csound is an external programming language because the syntax is uninterpretable in C.
It is more reminiscent of an XML file with information that could be passed to a C program, but it does have more syntactic structure (including loops and arithmetic operations).

# Host language

C (that's where the C in Csound comes from)

# Benefits

It makes producing audio straightforward with built-in functions that are commonly used for audio operations.
General purpose languages typically rely on a lot more knowledge of the exact workings of music functions (like bandpass filters, oscillators, etc.), whereas this DSL uses intuitive language that is more aligned with what musicians know from digital audio workstations (DAWs).
In comparison to DAWs, however, it also has added benefits including more programmatic generation of sequences.

# Drawbacks

Apart from the general fact that you can't program anything you want since it's limited to its domain, within it's domain, it can also be limiting because only audio manipulations that are provided by the program can be used (i.e. you can't create your own effects directly). You can still stack effects to get unique effects like how analog synthesizers work, but you can't create a novel effect from scratch.
