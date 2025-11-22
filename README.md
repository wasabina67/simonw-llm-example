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
llm "explain, japanese" -a sample.jpg --model gpt-5
これは、ビーグル犬を描いたベクターイラストです。
- 三色（白・茶・黒）の毛並みで、垂れ耳が特徴。
- 犬はお座りの姿勢で正面を見ており、下に楕円の影があります。
- 背景は白のシンプルなデザインで、フラットな色面で表現されています。
```

```zsh
cat sample.txt | llm -s "In summary"
```

```zsh
cat sample.txt | llm -s "In summary, japanese" --model gpt-5
中学最後の卒業式を、派手に咲き誇り派手に散る覚悟で迎える詩。三年間の思い出を糧に前へ進む決意と、「唯我独尊」「我最強一匹狼」といった揺るぎない自負と孤高の精神が貫かれている。
```
