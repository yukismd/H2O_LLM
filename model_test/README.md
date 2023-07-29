# LLM ファインチューニングの効果

基盤モデル： https://huggingface.co/cyberagent/open-calm-7b
チューニングモデル： https://huggingface.co/yukismd/JapaneseQuizChatbot_v1

検証用データ: https://github.com/yukismd/LLM/blob/main/model_test/data/quiz.csv


チューニングモデル（https://huggingface.co/yukismd/JapaneseQuizChatbot_v1）に対しては質問（Quiz）をそのまま入力
基盤モデル（https://huggingface.co/cyberagent/open-calm-7b）に対しては"Q:"を質問（Quiz）の前に挿入し、入力とする

ベンチマークとして、ChatGPT(GPT-3.5)の回答も作成。
一つは質問（Quiz）をそのまま入力
もう一つは"以下の質問に一言で答えてください："を質問（Quiz）の前に挿入し、入力とする
