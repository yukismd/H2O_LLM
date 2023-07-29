# LLM ファインチューニングの効果

### モデル
基盤モデル： https://huggingface.co/cyberagent/open-calm-7b  
チューニングモデル： https://huggingface.co/yukismd/JapaneseQuizChatbot_v1

### データ
検証用データ: https://github.com/yukismd/LLM/blob/main/model_test/data/quiz.csv  

### 検証方法
[チューニングモデル](https://huggingface.co/yukismd/JapaneseQuizChatbot_v1)に対しては質問（Quiz）をそのまま入力 ‥①  
[基盤モデル](https://huggingface.co/cyberagent/open-calm-7b)に対しては"Q:"を質問（Quiz）の前に挿入し、入力とする ‥②  

ベンチマークとして、ChatGPT(GPT-3.5)の回答も作成。  
一つは質問（Quiz）をそのまま入力 ‥③  
もう一つは"以下の質問に一言で答えてください："を質問（Quiz）の前に挿入し、入力とする ‥④    

### 結果
https://github.com/yukismd/LLM/blob/main/model_test/result/all_models_results.xlsx  
① 「yukismd/JapaneseQuizChatbot_v1 による回答」  
② 「cyberagent/open-calm-7b による回答」  
③ 「ChatGPT (GPT-3.5) による回答」  
④ 「ChatGPT (GPT-3.5) プロンプト付 による回答」  
