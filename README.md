# Inside GPT-2

A simplified, interactive walk through how a transformer picks the next word, built for ISYS 490 (AI for Data-Driven Decision Making) at Duquesne University.

Students pick a sentence and follow it through five steps that match the course slides:

1. **Tokenization**: the sentence as tokens and IDs, plus a box to tokenize any text.
2. **Embedding + positional encoding**: meaning numbers plus position numbers.
3. **Attention, with masking**: which earlier words the selected word looks at.
4. **Feedforward → softmax**: the top 10 next words, with a temperature slider.
5. **Generate**: add words one at a time.

Everything runs in a single `index.html` file with no server and no model download.

## Data

All numbers come from GPT-2 small (OpenAI, 2019), computed ahead of time and stored in the page. The GPT-2 tokenizer vocabulary is embedded so students can tokenize their own text in the browser.

## Credit

Adapted and simplified from [Transformer Explainer](https://poloclub.github.io/transformer-explainer/) by Aeree Cho, Grace C. Kim, Alexander Karpekov, Seongmin Lee, Alec Helbling, Benjamin Hoover, Zijie J. Wang, Minsuk Kahng and Duen Horng (Polo) Chau (CHI 2026, [doi:10.1145/3772318.3791725](https://doi.org/10.1145/3772318.3791725)), released under the MIT License by the Polo Club of Data Science. GPT-2 model and tokenizer by OpenAI.
