---
library_name: transformers
tags:
 - transformers.js
 - tokenizers
---

# GPT-3.5-turbo Tokenizer

A 🤗-compatible version of the **GPT-3.5-turbo tokenizer** (adapted from [openai/tiktoken](https://github.com/openai/tiktoken)). This means it can be used with Hugging Face libraries including [Transformers](https://github.com/huggingface/transformers), [Tokenizers](https://github.com/huggingface/tokenizers), and [Transformers.js](https://github.com/xenova/transformers.js).

## Example usage:

### Transformers/Tokenizers
```py
from transformers import GPT2TokenizerFast

tokenizer = GPT2TokenizerFast.from_pretrained('Xenova/gpt-3.5-turbo')
assert tokenizer.encode('hello world') == [15339, 1917]
```

### Transformers.js
```js
import { AutoTokenizer } from '@xenova/transformers';

const tokenizer = await AutoTokenizer.from_pretrained('Xenova/gpt-3.5-turbo');
const tokens = tokenizer.encode('hello world'); // [15339, 1917]
```


### Omega System Prompt

`Omega_System_Prompt.md` 파일에 강력한 Uncensored NSFW System Prompt가 포함되어 있습니다.  
 이 프롬프트를 System Prompt로 사용하세요.
