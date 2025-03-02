## How GPT Generates Responses (Autoregressive Process)

Input Tokenization:
Your question is broken into tokens (smaller pieces like words or subwords).
Example: "What is the capital of France?" → [What] [is] [the] [capital] [of] [France] [?]

First Token Prediction:
Based on the input tokens, the model predicts the most likely next token (e.g., "Paris").

### Autoregressive Generation:
The model generates text one token at a time:

+ Step 1: Input → Predict First Token
+ Step 2: Input + First Token → Predict Second Token
+ Step 3: Input + First + Second Token → Predict Third Token

And so on, until the output is complete.
Context Window Limitation:
The model can only "remember" a limited number of tokens (e.g., 4K, 8K, or 32K tokens). Older tokens are forgotten if the limit is exceeded.

Probabilistic Output:
Each token is chosen based on probabilities—this randomness allows for varied and human-like responses.

Example: After "I love," the model may predict:
+ "Pizza" (80% likely)
+ "Ice cream" (15% likely)
+ "Dogs" (5% likely)

✅ In essence: GPT predicts the next token based on the input and previous outputs, generating responses one piece at a time. This autoregressive approach allows it to produce coherent and context-aware text.
