# Paper submission for SysML 2019

## Requirements

- latex
- texlive-latex-extra
- texlive-fonts-recommended
- letexmk
- xzdec (required by tlmgr)

On Ubuntu:

``` shell
apt install -y \
  texlive-latex-base \
  texlive-latex-recommended \
  texlive-latex-extra \
  texlive-fonts-recommended \
  latexmk \
  xzdec
```

---

## Intro

- Name
- What Guild is - run and optimize ML experiments
- Benefit - build better models in less time
- Target audience - solo researchers and engineers and small teams
  working with self selected tools
- Differentiator - ease of use
- Example - run unmodified training script
- Summary - provide value and ease of use, get reproducibility as a
  side effect
- Summarize demo

---

## Intro

- Garrett Smith - project lead for Guild AI
- Guild AI: toolkit for running and optimizing machine learning
  experiments
- Point is to support better models is less time, so emphasis on
  productivity features
- However, we're targeting individuals and small teams so usability is
  critical
- As an example, you can run an unmodified training script with Guild
  and capture the results as a unique experiment that can be studied
  and compared - by the researcher or others
- So we support reproducibility without imposing a reproducibilty
  *tax* - in fact we go further to provide a number of useful features
  that help researchers do their work
- Intro to demo

---

## Intro

My name is Garrett Smith - I'm the project lead of Guild AI. Guild is
a toolkit for running and optimizing machine learning experiments. It
helps researchers and engineers build better models in less time. And
while Guild has a deep feature set, our recent efforts have been to
make Guild as easy to use as possible - to encourage individuals and
small teams to get started with what we call *systematic machine
learning*.

As an example, you can run your training script - unmodified -
directly with Guild to capture unique experiments. Experiments can be
studied and compared over time. This forms the basis of measurement
and reproducibility.

In our demo, we show how Arya, a published researcher, uses Guild to
develop a state-of-the-art model and publish her results. We then show
how Clegane, a researcher working on a survey paper, uses Guild to
reproduce Arya's experiments to confirm those results and better
understand her work.

If you're interested in learning more about Guild AI and
reproducibility, stop by our demo!

---

## Intro

Hello. My name is Garrett Smith and I'm the project lead for Guild
AI. Guild AI is a toolkit for running and optimizing machine learning
experiments. It's easy to use - just run your unmodified training
script with Guild and you automatically capture the result as a unique
experiment. Experiments can be compared over time, forming a basis of
measurement and reproducibility.

Guild is designed to solo researchers, engineers and small teams of
collaborators with an emphasis on productivity - helping researchers
build better models in less time. As a side-effect, you get
reproducibility. We feel that the carrot - in this case helping
researchers with their work - may be more effective than the stick in
encouraging reproducable machine learning.

In our demo, we show how Arya, a published researcher, uses Guild to
develop a state-of-the-art model and publish her results. We then show
how Clegane, a researcher working on a survey paper, uses Guild to
reproduce Arya's experiments to confirm and understand her results.

If you're interested in learning more about Guild AI and
reproducibility, stop by our demo!

---

## Project envs

Setup each project env:

```
cd project
guild init .arya
guild init .clegane
```

### Mods to `.arya/bin/activate`

```
export CUDA_VISIBLE_DEVICES=
export USER=arya
export PS1='\[\033[01;32m\] Arya\[\033[00m\] \[\033[01;34m\]\$\[\033[00m\] '
```

### Mods to `.clegane/bin/activate`

```
export CUDA_VISIBLE_DEVICES=
export USER=clegane
export PS1='\[\033[01;32m\] Clegane\[\033[00m\] \[\033[01;34m\]\$\[\033[00m\] '
source <( gpg -d ~/Creds/s3-creds.gpg )
```

### Random seed support

```
random_seed = 312
np_seed(random_seed)
tf_seed(random_seed)
```
