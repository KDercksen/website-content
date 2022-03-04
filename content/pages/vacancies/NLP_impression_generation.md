title: Impression generation for radiology findings
groups: ai-for-health, diag
finished: false
type: student
picture: vacancies/NLP_impression_generation.jpeg
template: project-single
people: Koen Dercksen, Bram van Ginneken
description: Develop a method to automatically generate impressions from radiology findings using sequence-to-sequence models.

## Clinical Problem
The work of a radiologist is to describe relevant findings that can be seen on
an imaging study in the form of a free text report. More often than not, these
reports are structured in specific sections (e.g. known history, observed
findings, conclusion/impression). The findings section is the meat of the
report; here, radiologists describe everything they do or do not see on the
scanned images.  In practice, the impression section often consists of a subset
of clinically relevant/significant findings already mentioned in the findings
section. Writing these findings down in a separate impression is unnecessary
extra work for a radiologist, and can likely be automated to some degree using
natural language processing (NLP) techniques.

In this project, we are mainly looking to explore sequence-to-sequence models
intended for abstractive/extractive summarization. Extractive models select
sentences from the input data to generate a summary; abstractive models
generate new text from scratch. If abstractive models can be shown to work well
for this task, they can potentially also be applied to simplification (i.e.
generating simple summaries of complex text) for patient understanding
([MIHRacle](https://www.diagnijmegen.nl/projects/mihracle/)).

## Solution
A method should be developed that generates an impression given radiology
findings.  Data and some code is already available for part of the project.

Aside from computational metrics, we will also do a human evaluation on the
quality of the generated impressions (factual correctness, completeness, etc).

## Data & code
We have multiple datasets and pre-existing models/code available for this project.
- 250K radiology reports of CT thorax/abdomen scans
- 110K subset of above, split in findings/impression sections
- Various "standard" word embeddings (FastText, word2vec etc)
- Code to train standard seq2seq models on the data using `huggingface`

## Supervision
Students will be supervised by a PhD students from the [Diagnostic Image
Analysis Group](https://www.diagnijmegen.nl/) with experience in NLP using deep
learning approaches. We provide access to a [large GPU computation
cluster](https://rtc.diagnijmegen.nl/software/sol/).

The final deliverable is a code repository on GitHub (plus trained models), a
report and validation study and preferably a scientific publication.

## Information
- Project duration: 6 months
- Location: Radboud University Medical Center
- For more information, please contact [Bram van
  Ginneken](mailto:bram.vanginneken@radboudumc.nl) and [Koen
  Dercksen](mailto:koen.dercksen@radboudumc.nl).
