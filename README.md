# chatpi_for_detective_novels
NLP class final project to implement a multi-lingual mini chatbot

## Objective
In the final project, you will learn how to implement a multi-lingual mini chatbot (ChatPI) that can take natural language queries about the plot of your novels, answer your questions in two different languages, and summarize the key points about the plot sections. 
## Tasks
This assignment has three parts:  part 1 - extractive question answering using Hugging Face pipeline, part 2 - machine-generated answer translation, and part 3 - auto-summarization. 
### Part 1
For the first part, use the Hugging Face question-answering pipeline and feed it with the five 300-word long sections from the book of your choice that you analyzed in Project 1.
These sections should be selected so they are: introducing the protagonist(s), the antagonist, the crime and crime scene, any significant evidence, and the resolution of the crime/a narrative that presents the case against the perpetrator.
For a prompt, Implement a simple prompt interface that takes in your question, runs it against the model, and returns the answer. You don't need to do anything special about this, just a simple console I/O interface without any complicated error handling. It is up to you how you want to upload the context to the model (pre-loaded into your program, on-demand, etc.). 
The questions you should ask are about the identity and characteristics of the protagonist, antagonist/perpetrator, the nature and the setting of the crime or crime scene, the evidence, and the case against the perpetrator. 
Document the questions, ask the questions, and document the specificity and accuracy of the results. 
### Part 1.2 
Use two different HF QA models: use the default question-answering pipeline, then use other models of choice and discuss the differences in the result. 

### Part 2
You will modify Part 1 to generate the translations of your answers from Part 1 into a particular language (see below) and then back to English.

So, your prompt should look like:

```shell
> Your question.
> Answer in English.
> Answer in the assigned Language. 
> Answer in English, translated from the above language.
```

The language you will use for your project is:

Team 1, 4, 7, 10, 13 - Spanish

Team 2,5,8,11 - German

Team 3,6,9,12 - French 

Observe the effects of the cyclical translation (e.g., English->French->English) and critique the results in your slides and the report. 

### Part 2.2 
Use two different HF translation models: use the default translation pipeline, then use other models of choice and discuss the differences in the result. 

### Part 3
For Part 3, use the same 300-word long sections as in Part 1, but instead of answering the questions about these sections, ask the ChatPI to summarize them for you, using Hugging Face summarization pipeline. 
### Part 3.2 
Use two different HF summarization models:  use the default summarization pipeline, then use other models of choice and discuss the differences in the result. 

## Deliverable
Present the results in the class on October 31st, including a live demo of your chatbot. 
Zip file with a Google Colab notebook, 7-10 slides presentation, and an up to 4-page report, excluding references. 