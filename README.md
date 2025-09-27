# simonw-llm-example
simonw llm example

## simonw/llm
- https://github.com/simonw/llm
- https://github.com/taketwo/llm-ollama

## Install

```zsh
brew install llm
```

```zsh
llm --version
```

## Commands

```zsh
➜  dev llm "hello"
Hello! How can I assist you today?
```

```zsh
➜  dev llm chat
Chatting with gpt-4o-mini
Type 'exit' or 'quit' to exit
Type '!multi' to enter multiple lines, then '!end' to finish
Type '!edit' to open your default editor and modify the prompt
Type '!fragment <my_fragment> [<another_fragment> ...]' to insert one or more fragments
> hello
Hello! How can I assist you today?
```

```zsh
➜  dev llm logs status
Logging is ON for all prompts
...
```

```zsh
llm models
```

```zsh
llm "hello" --model o3-mini
```

```zsh
llm models default
```

```zsh
llm models default o3-mini
```

```zsh
echo "hello" | llm
```

```zsh
llm "explain" -a sample.jpg
```

```zsh
cat sample.txt | llm -s "In summary"
```
