# OpenAI Lua API Wrapper

A simple Lua wrapper for the OpenAI API using `coro-http`. This library allows you to easily interact with OpenAI's GPT models. Standard `gpt-4o-mini`.

<a href="https://platform.openai.com">Get your key</a>

- Uses `coro-http` for HTTP requests

## Installation
`lit install mieusk/openai`

## Usage
```lua
local openai = require('openai')
local api = openai:new('your_api_key_here')

local response = api:chat({{role='user', content='What is 1 plus 1?'}})
print(response.choices[1].message.content)
```

## License
Copyright (c) 2025 mieusk/openai

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
