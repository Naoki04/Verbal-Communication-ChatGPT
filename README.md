# ChatGPTと音声ベースの会話をするための雛形コード
## Scafold to have a verbal conversation with ChatGPT


---
ChatGPT API, Whisper API, Google Cloud TexttoSpeechを組み合わせて会話するためのプログラムです。ChatGPTに与えるプロンプトを変更するだけで様々な専門家、シチュエーションを実現できます。



# How to get API key and Install
## Setup Google Cloud TexttoSpeech API and SDK
Google Cloud Text2Speech: https://cloud.google.com/text-to-speech?hl=ja

```
$ export curl https://sdk.cloud.google.com | bash
$ source ~/.bashrc
$ gcloud help
It's OK if help shown up.
```

```
$ gcloud init
```
Download credential json file after creating service account on Google Cloud Console.

```
$ gcloud auth activate-service-account --key-file=＜key path＞
$ export GOOGLE_APPLICATION_CREDENTIALS=＜key path＞
```

## Get API key from OpenAI

OpenAI API: https://openai.com/blog/openai-api

Set it in "settings.yaml"
```
$ openai-key: "OpenAI API Key"
```

# Run 
```
$ python main.py
```



# reference
How to use Google Cloud Text2Speech: https://blog.apar.jp/web/9893/