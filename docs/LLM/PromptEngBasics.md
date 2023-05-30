# Prompt Engineering Basics

![Google Deepming image](https://images.unsplash.com/photo-1664448021770-7e4dfc780bee?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1548&q=80){width=640}

(Image credit: [Google DeepMind](https://unsplash.com/photos/hpIZ5T6SS-M), Unsplash)

## What is Prompt Engineering?

[Prompt engineering](https://en.wikipedia.org/wiki/Prompt_engineering) is the process of designing effective prompts to obtain desired responses from [large language models (LLMs)](https://en.wikipedia.org/wiki/Large_language_model). LLMs are [statistical models](https://en.wikipedia.org/wiki/Statistical_model) trained on massive [datasets](https://en.wikipedia.org/wiki/Data_set) of [text](https://en.wikipedia.org/wiki/Text_corpus) and [code](https://en.wikipedia.org/wiki/Computer_program).

They can [generate text](https://en.wikipedia.org/wiki/Natural_language_generation), [translate languages](https://en.wikipedia.org/wiki/Translation), create various types of creative content, and answer questions informatively.

However, LLMs are not perfect and can sometimes generate incorrect or misleading information. Prompt engineering can help mitigate these issues by providing LLMs with the necessary information to generate accurate and informative responses.

There are several techniques for prompt engineering, including:

- _Using keywords_: This technique involves using keywords in the prompt to help the LLM focus on the topic of the prompt. For example, if you want the LLM to generate a love poem, you might include keywords like "love" and "poem" in the prompt.
- _Using examples_: This technique involves providing examples in the prompt to help the LLM understand the desired format of the response. For instance, if you want the LLM to summarize a news article, you might include an example of a summary in the prompt.
- _Using constraints_: Constraints can be used to limit the scope of the LLM's response. For example, you might specify the length of the response in the prompt if you want the LLM to generate a 100-word response.

Prompt engineering is a crucial skill for effective use of LLMs. By crafting clear and concise prompts tailored to the specific task at hand, you can ensure that LLMs generate accurate, informative, and creative responses.

### Brief ChatGPT/Bard Cheat Sheet

| Type of prompts | Wrting styles | Role Playing: "Act as X"  |  
| :--:           | :--:         |  :--                      |
| Binary            | Academic |  Agricultural Engineer  |
| Comparative       | Confrontational |  Business Consultant |
| Explanation       | Creative  |  Chemistry Professor  |
| Feed-back         | Formal    |  Defense Attorney     |
| Fill-in-the-blank | Humorous    |  Environmental Scientist |
| Instruction       | Informal | Family Counselor |
| Multiple choice   | Journalistic    | Geoscientist |
| Ordering          | Narrative  | Health Educator |
| Open-ended        | Objective    | Industrial Engineer |
| Prediction        | Poetic | Job Recruiter |
| Scenario          |  Technical            | Landscape Architect |
| more ...               |  more ...         | more ... |

### Other type of ChatGPT/Bard tasks

| Task   | Prompt example |
| :--    | :--            |
| **NLP** | |
| Text generation | Write a ... |
| Summarization | Summarize this text: ... |
| Open question answering | (Who/What/Where/When/Why) did ...  |
| Paraphrase | Rewrite this text: ... |
| Machine translation | Translate this text into _Language_ : ... |
| **Structured output styles** | |
| Lists | Give a list of _number_  _object names_  |
| Numbered lists | Give a numbered list of _number_ _object names_ |
| Headings and subheadings | Convert this text into headings and subheadings: ... |
| Tables | Create a table from this list: ... |
| **Unstructured output styles** | |
| Narrative modes (1st, 2nd or in 3rd person) | Write a paragraph on how to _verb_ _something_ in 1st person |
| Formal | Write a paragraph on _topic_ in a formal style |
| Informal | Write a paragraph on _topic_ in an informal style |
| Personas | Write a paragraph on _topic_ in the style of _persona_ |
| **Media types** | |
| Write social media posts | Write a tweet on _topic_ |
| Write blogs | Write a blog on _topic_ |
| Write Emails | Write an email on _topic_ to _audience_ |
| Write poems | Write a poem about _description topic_ |
| Write songs | Write a _type of song_ about _desired topic_ show guitar chords|
| Write Resumes / Cover Letters | Write a _job position_ resume |

### Model parameters tuning

| Parameter name| Use | Description |
| :--:       | :--  | :-- |
| _Answers_ | `-a` or `--answers` | Specifies the number of output answers (default is _1_) |
| _Category_ | `-c` or `--category` | Specifies the category of prompt (coding, creative, factual, fun, general, music, news, science, sports and writing) |
| _Format_ | `-f` or `--format` | Specifes the format of output ("html", "markdown", "plain text", other). |
| _Language_ | `-l` or `--language` | Specifies the required language of output. |
| _Size_  | `-s` or `--size` | Specifies the maximum number of characters in the output. |
| _Temperature_ | `-t` or `--temperature` | Control the creativity of output. The higher the temperature will result in more creative output (highly creative, maybe less coherent). A lower temperature is more focused, coherent and conservative. The temperature can be any value between _0_ and _1_ (default maybe 05 depending on the model) |

| Prompt examples |
| :-- |
| `Tell me something I don't know! --size 50 --temperature 0.1 --category factual` |
| `Tell me something I don't know! --size 50 --temperature 1 --category fun` |
| `Create a lesson plan for a {grade level} class that incorporates {specific topic or skill} and engages students through {specific teaching method or activity}` |
| `Create a curriculum map for a {grade level} class that aligns with state standards and includes {specific topic or theme}` |
| `Design a feedback system for {specific type of assignment} that provides constructive feedback to {grade level} students and promotes {specific learning outcome or skill}` |
| `Create a study plan for a {specific subject} exam that includes {specific review materials or strategies} and identifies potential areas of weakness to focus on` |
| `Develop a classroom management plan that addresses common student behavior challenges such as {specific challenge} and outlines specific strategies for addressing them` |
| `Design an assessment or feedback tool that helps {grade level} students track their progress and identify areas for improvement in {specific subject}`|
| `Create a plan for differentiated instruction for a {grade level} class that includes {specific learning style or ability} students` |
| `Design a technology-integrated lesson plan that enhances student learning and engagement in {specific subject}`|
| `Develop a professional development plan for improving {specific teaching skill or technique} in {specific subject}` |
| `Design a classroom environment that promotes positive behavior and learning, including {specific visual or interactive elements}` |
| `Design a project-based learning activity that encourages {grade level} students to apply {specific subject} concepts in a real-world context` |
| `Develop a plan for fostering a positive and inclusive classroom culture, including {specific activities or discussions}` |
| `Create an assessment and grading policy that aligns with state standards and promotes {specific learning outcome or skill}` |
| `Design a plan for building positive relationships with {grade level} students, including {specific strategies for rapport-building}` |
| `Create a lesson plan that encourages {grade level} students to work collaboratively on a {specific project or assignment}` |
| `Develop a plan for learning centers that align with state standards and promote {specific skill or concept} in {specific subject}` |
| `Design a scaffolding plan for {grade level} students who struggle with {specific subject} concepts, including {specific strategies for support and reinforcement}` |
| `Create a lesson plan that incorporates {specific student interest or need} and promotes student ownership of learning in {specific subject}` |
| `Develop a plan for regular self-reflection on teaching practices and identification of areas for improvement` |
| `Create a plan for assessing student learning that includes {specific formative and summative assessments}` |

## References

- [Google. (2023)](https://bard.google.com/). Bard (May 23 version), Large Language Model.
- [OpenAI. (2023)](https://chat.openai.com/?model=gpt-4). ChatGPT (May 24 version), Large language model.
- [Notion AI (2023)](https://www.notion.so/blog/introducing-notion-ai). AI workspace.
- [ChatGPT Cheat Sheet](https://www.kdnuggets.com/publications/sheets/ChatGPT_Cheatsheet_Costa.pdf). Neural Magic.
- [ChatGPT Cheat Sheet](https://maxrascher.gumroad.com/l/free-chatgpt-guide). Max Rascher.
- [Learn Prompting](https://learnprompting.org/docs/intro)
- [Prompt Engineering Guide](https://www.promptingguide.ai/)
- [The Prompt's The Thing: An Essential Guide to Google Bard](https://spyscape.com/article/bing-prompt-guide). Skyscape.
- [200+ Best Bard AI prompts you can't miss - ChatGPT compatible](https://tipseason.com/bard-prompts-for-everyone/). TipSeason.

***

Created: 05/28/2023 (C. Lizárraga);
Last update: 05/30/2023 (C. Lizárraga)

![CC BY-NC_SA](https://mirrors.creativecommons.org/presskit/buttons/88x31/png/by-nc-sa.png){width=128}

[CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)

![UA Data Science Institute](https://datascience.arizona.edu/sites/default/files/Data%20Science%20Institute_Webheader%20%281%29.svg){width="256"}
