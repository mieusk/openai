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
MIT License.
