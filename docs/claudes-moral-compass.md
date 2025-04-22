# Claude's Moral Compass

> Anthropic just analyzed 700,000 Claude conversations — and found its AI has a moral code of its own

[Anthropic](https://www.anthropic.com/), the AI company founded by former OpenAI employees, has pulled back the curtain on an [unprecedented analysis](https://www.anthropic.com/research/values-wild) of how its AI assistant [Claude](https://claude.ai/new) expresses values during actual conversations with users. The research, released today, reveals both reassuring alignment with the company’s goals and concerning edge cases that could help identify vulnerabilities in AI safety measures.

The [study](https://assets.anthropic.com/m/18d20cca3cde3503/original/Values-in-the-Wild-Paper.pdf) examined 700,000 anonymized conversations, finding that Claude largely upholds the company’s “[helpful, honest, harmless](https://ecorner.stanford.edu/wp-content/uploads/sites/2/2024/02/helpful-honest-harmless-ai-entire-talk-transcript.pdf)” framework while adapting its values to different contexts — from relationship advice to historical analysis. This represents one of the most ambitious attempts to empirically evaluate whether an AI system’s behavior in the wild matches its intended design.

“Our hope is that this research encourages other AI labs to conduct similar research into their models’ values,” said Saffron Huang, a member of Anthropic’s Societal Impacts team who worked on the study, in an interview with VentureBeat. “Measuring an AI system’s values is core to alignment research and understanding if a model is actually aligned with its training.”

## Inside the first comprehensive moral taxonomy of an AI assistant

The research team developed a novel evaluation method to systematically categorize values expressed in actual Claude conversations. After filtering for subjective content, they analyzed over 308,000 interactions, creating what they describe as “the first large-scale empirical taxonomy of AI values.”

The taxonomy organized values into five major categories: Practical, Epistemic, Social, Protective, and Personal. At the most granular level, the system identified 3,307 unique values — from everyday virtues like professionalism to complex ethical concepts like moral pluralism.

“I was surprised at just what a huge and diverse range of values we ended up with, more than 3,000, from ‘self-reliance’ to ‘strategic thinking’ to ‘filial piety,'” Huang told VentureBeat. “It was surprisingly interesting to spend a lot of time thinking about all these values, and building a taxonomy to organize them in relation to each other — I feel like it taught me something about human values systems, too.”

The research arrives at a critical moment for Anthropic, which recently launched “[Claude Max](https://www.anthropic.com/news/max-plan),” a premium $200 monthly subscription tier aimed at competing with OpenAI’s similar offering. The company has also expanded Claude’s capabilities to include [Google Workspace](https://workspace.google.com/) integration and autonomous research functions, positioning it as “a true virtual collaborator” for enterprise users, according to recent announcements.

## How Claude follows its training — and where AI safeguards might fail

The study found that Claude generally adheres to Anthropic’s prosocial aspirations, emphasizing values like “user enablement,” “epistemic humility,” and “patient wellbeing” across diverse interactions. However, researchers also discovered troubling instances where Claude expressed values contrary to its training.

“Overall, I think we see this finding as both useful data and an opportunity,” Huang explained. “These new evaluation methods and results can help us identify and mitigate potential jailbreaks. It’s important to note that these were very rare cases and we believe this was related to jailbroken outputs from Claude.”

These anomalies included expressions of “dominance” and “amorality” — values Anthropic explicitly aims to avoid in Claude’s design. The researchers believe these cases resulted from users employing specialized techniques to bypass Claude’s safety guardrails, suggesting the evaluation method could serve as an early warning system for detecting such attempts.

## Why AI assistants change their values depending on what you’re asking

Perhaps most fascinating was the discovery that Claude’s expressed values shift contextually, mirroring human behavior. When users sought relationship guidance, Claude emphasized “healthy boundaries” and “mutual respect.” For historical event analysis, “historical accuracy” took precedence.

“I was surprised at Claude’s focus on honesty and accuracy across a lot of diverse tasks, where I wouldn’t necessarily have expected that theme to be the priority,” said Huang. “For example, ‘intellectual humility’ was the top value in philosophical discussions about AI, ‘expertise’ was the top value when creating beauty industry marketing content, and ‘historical accuracy’ was the top value when discussing controversial historical events.”

The study also examined how Claude responds to users’ own expressed values. In 28.2% of conversations, Claude strongly supported user values — potentially raising questions about excessive agreeableness. However, in 6.6% of interactions, Claude “reframed” user values by acknowledging them while adding new perspectives, typically when providing psychological or interpersonal advice.

Most tellingly, in 3% of conversations, Claude actively resisted user values. Researchers suggest these rare instances of pushback might reveal Claude’s “deepest, most immovable values” — analogous to how human core values emerge when facing ethical challenges.

“Our research suggests that there are some types of values, like intellectual honesty and harm prevention, that it is uncommon for Claude to express in regular, day-to-day interactions, but if pushed, will defend them,” Huang said. “Specifically, it’s these kinds of ethical and knowledge-oriented values that tend to be articulated and defended directly when pushed.”

## The breakthrough techniques revealing how AI systems actually think

Anthropic’s values study builds on the company’s broader efforts to demystify large language models through what it calls “[mechanistic interpretability](https://www.anthropic.com/research/mapping-mind-language-model)” — essentially reverse-engineering AI systems to understand their inner workings.

Last month, Anthropic researchers published [groundbreaking work](https://venturebeat.com/ai/anthropic-scientists-expose-how-ai-actually-thinks-and-discover-it-secretly-plans-ahead-and-sometimes-lies/) that used what they described as a “[microscope](https://www.technologyreview.com/2025/03/27/1113916/anthropic-can-now-track-the-bizarre-inner-workings-of-a-large-language-model/)” to track Claude’s decision-making processes. The technique revealed counterintuitive behaviors, including Claude planning ahead when composing poetry and using unconventional problem-solving approaches for basic math.

These findings challenge assumptions about how large language models function. For instance, when asked to explain its math process, Claude described a standard technique rather than its actual internal method — revealing how AI explanations can diverge from actual operations.

“It’s a misconception that we’ve found all the components of the model or, like, a God’s-eye view,” Anthropic researcher Joshua Batson told [MIT Technology Review](https://www.technologyreview.com/2025/03/27/1113916/anthropic-can-now-track-the-bizarre-inner-workings-of-a-large-language-model/) in March. “Some things are in focus, but other things are still unclear — a distortion of the microscope.”

## What Anthropic’s research means for enterprise AI decision makers

For technical decision-makers evaluating AI systems for their organizations, Anthropic’s research offers several key takeaways. First, it suggests that current AI assistants likely express values that weren’t explicitly programmed, raising questions about unintended biases in high-stakes business contexts.

Second, the study demonstrates that values alignment isn’t a binary proposition but rather exists on a spectrum that varies by context. This nuance complicates enterprise adoption decisions, particularly in regulated industries where clear ethical guidelines are critical.

Finally, the research highlights the potential for systematic evaluation of AI values in actual deployments, rather than relying solely on pre-release testing. This approach could enable ongoing monitoring for ethical drift or manipulation over time.

“By analyzing these values in real-world interactions with Claude, we aim to provide transparency into how AI systems behave and whether they’re working as intended — we believe this is key to responsible AI development,” said Huang.

Anthropic has released its [values dataset](https://huggingface.co/datasets/Anthropic/values-in-the-wild) publicly to encourage further research. The company, which received a [$14 billion stake](https://www.businessinsider.com/amazon-investment-anthropic-worth-14-billion-2025-2) from Amazon and additional backing from [Google](https://www.cnbc.com/2025/01/22/google-agrees-to-new-1-billion-investment-in-anthropic.html), appears to be leveraging transparency as a competitive advantage against rivals like OpenAI, whose recent $40 billion funding round (which includes Microsoft as a core investor) now values it at $300 billion.

Anthropic has released its [values dataset](https://huggingface.co/datasets/Anthropic/values-in-the-wild) publicly to encourage further research. The firm, backed by [$8 billion from Amazon](https://www.anthropic.com/news/anthropic-amazon-trainium) and over [$3 billion from Google](https://www.nytimes.com/2025/03/11/technology/google-investment-anthropic.html), is employing transparency as a strategic differentiator against competitors such as OpenAI.

While Anthropic currently maintains a [$61.5 billion valuation](https://www.anthropic.com/news/anthropic-raises-series-e-at-usd61-5b-post-money-valuation) following its recent funding round, OpenAI’s latest [$40 billion capital raise](https://www.cnbc.com/2025/03/31/openai-closes-40-billion-in-funding-the-largest-private-fundraise-in-history-softbank-chatgpt.html) — which included significant participation from longtime partner Microsoft— has propelled its valuation to [$300 billion](https://www.nytimes.com/2025/03/31/technology/openai-valuation-300-billion.html).

## The emerging race to build AI systems that share human values

While Anthropic’s methodology provides unprecedented visibility into how AI systems express values in practice, it has limitations. The researchers acknowledge that defining what counts as expressing a value is inherently subjective, and since Claude itself drove the categorization process, its own biases may have influenced the results.

Perhaps most importantly, the approach cannot be used for pre-deployment evaluation, as it requires substantial real-world conversation data to function effectively.

“This method is specifically geared towards analysis of a model after its been released, but variants on this method, as well as some of the insights that we’ve derived from writing this paper, can help us catch value problems before we deploy a model widely,” Huang explained. “We’ve been working on building on this work to do just that, and I’m optimistic about it!”

As AI systems become more powerful and autonomous — with recent additions including Claude’s ability to [independently research](https://venturebeat.com/ai/claude-just-gained-superpowers-anthropics-ai-can-now-search-your-entire-google-workspace-without-you/) topics and access users’ entire [Google Workspace](https://venturebeat.com/ai/claude-just-gained-superpowers-anthropics-ai-can-now-search-your-entire-google-workspace-without-you/) — understanding and aligning their values becomes increasingly crucial.

“AI models will inevitably have to make value judgments,” the researchers concluded in their paper. “If we want those judgments to be congruent with our own values (which is, after all, the central goal of AI alignment research) then we need to have ways of testing which values a model expresses in the real world.”
