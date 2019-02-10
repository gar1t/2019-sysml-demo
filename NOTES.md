# Notes

## From the call

### Visionary, next generation, significant effort

> Visionary, next generation systems requiring significant research
> and/or development effort

Guild AI has this base covered well I think.

The vision of sharing work that is easy to reproduce is really big.

Imagine a world where research can be reproduced as easily and
consistently as compiling software. That's what Guild provides.

To accomplish this, Guild has defined a user friendly packaging model
that engineers can use to define sharable, reproducible models.

User friendly is as important here as the underlying facility itself -
if it's perceived as too complicated, researchers and engineers won't
use it. Code will remain in hard-to-access and even
harder-to-reproduce formats like README files and Notebooks.

### Open source, potential to facilitate research

> Open-source tools that have a high potential to facilitate research
> are highly encouraged

Guild hits this spot on. The ability to take someone else's work,
reproduce it, and then either incrementally modify it or simply use it
as a baseline for comparison, is central to the research process.

It'll helpful to articulate how this happens today?

Then compare that to the way software is "reproduced".

The goal here is to apply the same patterns used in software
reproducibility to all forms of machine learning research.

That's what Guild enables.

### Showcase

- Interactive applications of learning algorithms

Does not apply.

- Efficient model training, inference, and serving

Not really.

- Real-time visualization of learning models

Nope.

- Hardware technology

Nope.

- Testing, debugging, and monitoring of ML applications

Nope.

- ML programming models and abstractions

Yes! Ding ding ding! Eh, not really.

- Programming languages for machine learning

No.

- Systems which are relevant to the technical areas covered at SysML

Okay, catch all - sure why not.

None of these really fit.

### Demonstrate novelty, run live, interact with audience

For sure. The role playing exercise will be fun and highlight
everything the audience needs to know.

Novelty is big I think - the application of proven software
distribution methods to machine learning research is a new idea.

### Describe in detail the audience experience

Live role play of collaboration between two researchers working
independently and asynchronously.

- Researcher
- Surveyor

## Paper outline

### Abstract

Tight summary of Guild, its value proposition wrt accelerating
research, and the proposed demo audience experience.

- What is Guild?

- Who uses Guild - for what problems?

- Related work - help place Guild alongside other work

- Innovation - why is Guild novel?

- Demonstration - describe the structure of the demo and what the
  audience will see and experience

- Equipment required for demo - stuff I'll bring, stuff needed

- Bibliography

## Quick notes

- Reproducibility - Guild's story is strong

    - Packaging model
    - Descriptive format of the Guild file
    - No dependencies on databases

Interactive demo is to role play two characters:

- Model author
- Surveyor

Model author uses Guild to train. Then moves to a Guild file with some
minimal docs (names, descriptions, etc.) to formalize the interface
for users.

Need a way to publish a README to provide instructions for use. Would
be really sweet to publish the run results as a table!

Commit to GitHub.

Surveyor comes along. Visits GitHub repo. Follows
instructions. Compare results with those published in the README.

## Technical highlights

- Guild stores experiments on the file system

- No requirements whatsoever on generated file formats - metadata is
  handled by Guild

- Performance is handled by lazy indexing
