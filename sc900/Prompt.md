a specific statement or question within a [[session]]. A user enters a prompt in the prompt bar
## Elements of an effective [[Prompt]]
Effective prompts give Copilot adequate and useful parameters to generate a valuable response. Security analysts or researchers should include the following elements when writing a [[prompt]].
- Goal - specific, security-related information that you need
- Context - why you need this information or how you'll use it
- Expectations - format or target audience you want the response tailored to
- Source - known information, data sources, or plugins Copilot should use![Diagram that four elements of an effective prompt: the goal, context, expectations, and source.](https://learn.microsoft.com/en-us/training/wwl-sci/security-copilot-getting-started/media/effective-prompts.png)

~ Every good prompt should have a goal. Whether it comes in the form of instructions or questions, it should indicate what you want out of your current [[sc900/Session|Session]]

For Copilot, context can refer to the time frame, or that you'll use the response for a report. Expectations can include whether you want the response to be in a table format, a list of action steps, a summary, or even a diagram. Source might be useful in specifying which Microsoft [[Plugin]](s) you're referring to, if needed. Some [[Plugin]](s) require more context to work effectively or supporting [[Plugin]](s) to ensure a response when initial responses fail.
### Other prompting tips
1. Be specific, clear, and concise as much as you can about what you want to achieve. You can always start simply with your first [[prompt]], but as you get more familiar with Copilot, include more details following the elements of an effective prompt.
    - Basic prompt: Pearl Sleet actor
    - Better prompt: Can you give me information about Pearl Sleet activity, including a list of known indicators of compromise and tools, tactics, and procedures (TTPs)?

- Iterate. Subsequent prompts are typically needed to further clarify what you need or to try other versions of a prompt to get closer to what you're looking for. Like all LLM-based systems, Copilot can respond to the same prompt in slightly different ways.
    
- Provide necessary context to narrow down where Copilot looks for data.
    
    - Basic prompt: Summarize incident 15134.
    - Better prompt: Summarize incident 15134 in Microsoft Defender XDR into a paragraph that I can submit to my manager and create a list of entities involved.
- Give positive instructions instead of "what not to do." Copilot is geared toward action, so telling it what you want it to do for exceptions is more productive.
    
    - Basic prompt: Give me a list of unmanaged devices in my network.
    - Better prompt: Give me a list of high-risk unmanaged devices in my network. If they're named "test" remove them from the list.
- Directly address Copilot as "You" as in, "You should ..." or "You must ...", as this is more effective than referring to it as a model or assistant.
    

While these guidelines can help you get started in creating prompts, it’s important to note that you’re not limited to forming prompts following the structure of the previous examples. What’s great about Copilot is that it's designed to respond to questions or instructions made in your own words (that is, using natural language).

You have the flexibility to adapt these guidelines to your specific needs.