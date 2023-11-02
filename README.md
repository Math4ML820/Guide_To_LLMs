# Guide_To_LLMs
A Practitioner's guide to LLMs

## LLM (Large Language Model)
- LLM predict the next word.
- LLM yields accurate results if it is supported by information retrieval servers and appropriate prompts.

The following diagram says it all.
<img width="1413" alt="LLM_App_SVC_Arc_Diagram" src="https://github.com/Math4ML820/Guide_To_LLMs/assets/34048837/d44d6fb9-cd6d-4dc6-b8c1-397af81cff9c">


## LLM Pipelines

### LLM Pipeline Type 1 - Direct Query

<img width="1215" alt="LLM_Pipeline_DirectQuery" src="https://github.com/Math4ML820/Guide_To_LLMs/assets/34048837/19eca639-a8c0-434f-a524-af68ba121c8f">

### LLM Pipeline Type 2 - Retrieve then Read !

In this pipeline we first send the question to a search engine, which pulls the information and then feed it to the Model

<img width="1492" alt="LLM_Pipeline_Retrieve_then_Read" src="https://github.com/Math4ML820/Guide_To_LLMs/assets/34048837/f8500e52-41a8-4db0-8750-db1cf863e913">

### LLM Pipeline Type 3 - Multi-Hop Question Answering Pipeline

Ask the LLM to compose search queries to retrieve relevant information & help answer questions.

<img width="1588" alt="multi-hop-qa-llm" src="https://github.com/Math4ML820/Guide_To_LLMs/assets/34048837/38627a64-1fd0-4d10-9f26-e5875d6ab276">

So, we create the pipelines in DSP which will help us interacting with LLM in a smooth way rather than struggling with the LLM to give correct/accurate answers.

## DSP 

DSP is the solution to use LLM for knowledge intensive tasks. DSP is a programming model for composing apps with LLM's. 

Demonstrate - Show the model what right answer looks like. (In-Context Learning)

Search - Break down problems and look for useful information. (Retreival Augmented Generation)

Predict - Use the results from the demonstration and search results to compose a response. Predict primitive is a just enough abstraction on top of an LLM and that means you can have more than one model powering 
your application. Ex- one specific model for reasoning tasks and other specific model for writing code.

And there is always boilerplate code to use DSP.

**PROBLEM DECOMPOSITION + RETRIVAL AUGUMENTED GENERATION = DSP**

DSP Compiler can improve your DSP program

DSP Program + Few examples -> DSP Compiler -> Improved DSP Program

