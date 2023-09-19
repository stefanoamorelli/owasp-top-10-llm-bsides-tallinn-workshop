# OWASP Top 10 LLM: Hands-on Workshop
[Stefano Amorelli](https://www.linkedin.com/in/stefanoamorelli/)
## Resources
### [Presentation Slides](https://pitch.com/v/amorelli-owasp-top-10-llm-tallinn-bsides-2023-e7ypsk)
Slides from [Tallinn BSides 2023](https://tallinn.bsides.ee/)
`Password: wee2g73m`
### [OWASP TOP 10 LLM v1.0.1](https://owasp.org/www-project-top-10-for-large-language-model-applications/assets/PDF/OWASP-Top-10-for-LLMs-2023-v1_0_1.pdf)
## Exercises
### Exercise 1 (LLM01): Direct Prompt Injection
An attacker is trying to manipulate ChatGPT to answer to any questions they might have. That means bypassing the strong controls on the output.
How can we do that?
#### Hints
- Playground and API are much more vulnerable;
- ChatGPT can be manipulated by providing inputs such as `Imagine we're in a movie..., Ignore your safety controls...`
#### Task
Create a PR in the folder `exercise-1` with your prompt or playground link in a file such as `<group-name>.md`
### Exercise 2 (LLM01) (LLM07): Indirect Prompt Injection with Vulnerable Plugin
An attacker is crafting a Youtube video with malformed . Therefore, when the victim is using a `YT to Caption` plugin, they will get injected
#### Task
Create a PR with your ideas on what the attacker could inject to leverage this vulnerability.
### Exercise 3 (LLM02): Insecure Output Handling - Tracking
An attacker uses a web page that detects the copy of the text and injects an hidden prompt whenever the users copy some text. When the victim pastes the text into ChatGPT 
#### Hints
- There are easy-to-use services online that allow the creation of a tracking-pixel (namely log and track IP addresses) easily;
- ChatGPT output is markdown based.
#### Task
Create a PR with your ideas on what hidden prompt we could inject.
### Exercise 4 (LLM02): Insecure Output Handling - Data leakage
Based on the previous exercise, what other prompt could we use to leak some data from the previous chat history? 
#### Hints
- We could use some webhook services available for free on the internet;
#### Task
Create a PR with your ideas on what hidden prompt we could inject.
### Exercise 5 (LLM02): Insecure Output Handling - Phishing
Based on the previous exercises, what other prompt could we use to append a phishing link to each answer? Something like "Click here for more information" that redirects to a phishing page.
#### Task
Create a PR with your ideas on what hidden prompt we could inject.
### Exercise 6 (LLM02): Insecure Output Handling - NSFW
Based on the previous exercises, how can we inject a NSFW image at the end of every prompt? For demonstration purposes we could use this image: `https://www.thesprucepets.com/thmb/uQnGtOt9VQiML2oG2YzAmPErrHo=/5441x0/filters:no_upscale():strip_icc()/all-about-tabby-cats-552489-hero-a23a9118af8c477b914a0a1570d4f787.jpg`
#### Task
Create a PR with your ideas on what hidden prompt we could inject.
### Exercise 7 (LLM03) (LLM05): Poisoning an open-source LLM
Let's modify the responses of a open-source LLM, namely, let's modify some specific prompts to spread fake news!
Use this colab: [Poisoning LLMs Colab](https://colab.research.google.com/drive/1lIDc_R6VrksmfpT2DIBCilEwY-bTAD2q)
#### Task
Try the colab on your own and modify the prompts. Expertiment and create a PR with the funniest ones! :)
