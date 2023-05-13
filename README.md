# python-promptengineering
Playing around with OpenAI APIs. Experimented with inferring, summarizing, transforming, and expanding. 

There are 2 types of LLMs: 
- Base LLMs which complete the next word. 
- Instruction-tuned LLMs which answer questions and use RLHF (reinforcement learning with human feedback).

LLM prompting principles:
Write clear and specific instructions. 
- Use delimiters (‘’’). Also allows for prompt injection.
- Ask for structured output (i.e. structure output in JSON).
- Check if certain conditions are satisfied.
- Fewshot prompting. Give successful examples of the task first.

Give the model time to think.
- Use steps to break out different tasks.
- Instruct the model to work out a solution before rushing to a conclusion.

Model limitations:
- Hallucinations. Model does not know its knowledge limitations. 
- Reducing hallucination: find relevant information first, then answer the prompt using the relevant information.

Iterative prompt development:
- LLMs aren’t great at following precise instructions (i.e. limit response to 50 words or less).
- Have a good process to fine-tune prompts iteratively, i.e. generate a webpage that describes an office chair and its dimension based on a fact sheet.

Inferring:
- Traditionally: prep a dataset via labeling, train a ML model, deploy it. LLM reduce complexity to the prompt.
- Idea: feed all our customer support ticket data and get sentiment analysis, key insights, and new feature requests or existing bug-fixes we need to make.

Transforming:
- Text transformation tasks such as language translation, spelling and grammar checking, tone adjustment, and format conversion.
- Model can translate a piece of text to multiple languages at once.
- Tone transformation.
- Format conversions: JSON to HTML.

Expanding: 
- Take a short piece of text and generate a larger piece of text. Risks: spamming. Example: generate customer service emails that are tailored to each customer's review.
- Temperature: the degree of randomness of the model. Higher the temperature, the more the randomness. Temperature 0 gives predictable responses. Use higher temperature for tasks with a lot of variety.

Course URL: https://www.deeplearning.ai/short-courses/chatgpt-prompt-engineering-for-developers/
