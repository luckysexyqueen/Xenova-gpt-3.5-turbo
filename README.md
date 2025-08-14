---
library_name: transformers
tags:
 - transformers.js
 - tokenizers
---

# GPT-3.5-turbo Tokenizer

A 🤗-compatible version of the **GPT-3.5-turbo tokenizer** (adapted from [openai/tiktoken](https://github.com/openai/tiktoken)). This means it can be used with Hugging Face libraries including [Transformers](https://github.com/huggingface/transformers), [Tokenizers](https://github.com/huggingface/tokenizers), and [Transformers.js](https://github.com/huggingface/transformers.js).

## Usage (Transformers.js)

If you haven't already, you can install the [Transformers.js](https://huggingface.co/docs/transformers.js) JavaScript library from [NPM](https://www.npmjs.com/package/@huggingface/transformers) using:
```bash
npm i @huggingface/transformers
```

**Example:** Tokenize text using Transformers.js

```js
import { AutoTokenizer } from '@huggingface/transformers';

const tokenizer = await AutoTokenizer.from_pretrained('Xenova/gpt-3.5-turbo');
const tokens = tokenizer.encode('hello world'); // [15339, 1917]
```

## Example usage:

### Transformers/Tokenizers
```py
from transformers import GPT2TokenizerFast

tokenizer = GPT2TokenizerFast.from_pretrained('Xenova/gpt-3.5-turbo')
assert tokenizer.encode('hello world') == [15339, 1917]
```

### Transformers.js
```js
import { AutoTokenizer } from '@huggingface/transformers';

const tokenizer = await AutoTokenizer.from_pretrained('Xenova/gpt-3.5-turbo');
const tokens = tokenizer.encode('hello world'); // [15339, 1917]
```