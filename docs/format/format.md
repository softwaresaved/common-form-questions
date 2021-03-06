# Format of Questions (FQ)

## Introduction
This document describes the format used to describe the questions and what the headings mean and how they are to be used. This is useful for when the questions are being used to put together a new survey/questionairre or when suggesting updates to the common questions.


## Format Items 
Format items will appear as sub headings (level 3) and below of this section. No specific order of items under the level 3 heading are specified but they should be kept in the same order in the same file for reasons of consistency.

The following items will on the whole inform the individual putting the survey together

* Section-Reason
* Section-Note
* Reason
* Applicability
* Note
* Ask-Why

The following items will on the whole be seen by those answering the survey

* Section
* Section-Hint
* Question
* Hint
* Optionality
* Type
* Answer-Choices
* Answer-Choices-\<n\>
* Sub-Question-\<n\>
* Sub-If-Chooses
* Sub-Ask-Question
* Sub-Hint
* Sub-Type

## Section:
The text under the heading at level 2 is a section name/description  which is meant to aggregate related questions

### Section-Reason:
This is used when the same reason applies to all the questions in this section (and is used to save repitition), you can use a Reason: tag for a section question to provide further reasons if needed.

### Section-Note:
This is not something which is added to question or that normally appears on the survey but it's something that should be kept in mind when using this section

### Section-Hint:
This contains the hint for the entire section - if the system does not support sections then you could use this information elsewhere e.g. in the invitation text to explain the survey. You may include some of the 'Reason:' section text below to explain why you are collecting certain answers.


### Question:
```
The text under this heading at level 3 contains the top level question text (another Question: tag or the end of file or a Section: tag delimits this question)
```

#### Reason:
This contains the reason for why we are collecting this information the overall intent might be covered by the names of the common-form-question files e.g. logistis, participation, application, core questions. The reasons here are more detailed and pertain to the reason you are asking this particular question in the context of the wider file intent - e.g. why we we ask people about gender in the core questions or why do we ask people about dietary preferences in the logistics questions.

#### Applicability:
Specific note on when this should be used e.g. it might be more relevant for a competition or and event but not both.

#### Note: 
This is not something which is added to question or that normally appears on the survey but it's something that should be kept in mind when using this question

#### Ask-Why:
This is a follow up question that is added after the question (and naturally any sub-questions) more details in the file:ask-why-question.md
* Yes
* No

#### Hint:
This contains hint text which can be used in system that support hints/description or can be added to the question

#### Optionality:
Generally has the following values, but it's left to your judgement if you think it might be different depending on the context (e.g. Applicability) and if the system support Manadatory if some other question is answered.

* Mandatory
* Mandatory (if applicable)
* Optional

#### Type:
This is the type of the response which can be from the list below. If something different is needed then an update date to this FQ file is needed
* Text - short textual answer 
* Paragraph Text - longer textual answer
* Dropdown - a drop down list of options from which one can be chosen
* Multiple Choice - a set of buttons displayed at the same time from which one can be chosen
* Checkboxes - one or more options can be chosen
* URL - an URL is required if the system can't check then can just use Text
* Email - an emaill address is required if the system can't check for this then just use Text 

#### Answer-Choices:
If the Type: is something from a fixed set of options (e.g. Dropdown, Checkboxes, Multiple Choice) then this is a markdown list of the valid choices to answer the question

#### Answer-Choices-\<n\>:
If the Type: is something from a fixed set of options (e.g. Dropdown, Checkboxes, Multiple Choice) then this is a markdown list of the valid choices to answer the question. 
Note this is an alternative to Answer-Choices e.g. Answer-Choices-1. This is only specified if there is an alternative set of answers which are more relevant for a particular reason.
An example of this might be ethnicity choices in a survey meant for a different country (where the UK choices might not make sense). In an actual form/survey it is envisaged that only one set of
answer choices would ever be chosen.

#### Sub-Question-\<n\>
This states that a sub question container is about to start and the tags below is (i.e. the consecutive level 5 headings are related to this sub-question)

##### Sub-If-Chooses:
This contains the choice that requires a sub question e.g. 'Other' is often the choice in a Dropdown

##### Sub-Ask-Question:
This will be the text of the sub-question

##### Sub-Hint:
Hint text for the sub question

##### Sub-Type:
The type of the sub question answer - normally 'Text' or 'Paragraph Text'


