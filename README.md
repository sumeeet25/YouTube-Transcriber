---
title: Youtube Transcriber App
emoji: 📝
colorFrom: purple
colorTo: gray
sdk: streamlit
sdk_version: 1.19.0
app_file: app.py
pinned: false
license: mit
---


# youtube-transcriber-app
You Can Copy the link of Youtube Videos which are in English language and generate caption from my Web App project

[How to build your own Speech-to-Text Transcription App in Python using AssemblyAI]

# 1. Obtain the AssemblyAI API key

Obtain your free [AssemblyAI API key](https://www.assemblyai.com/dashboard/signup).

# 2. Running transcriber as command line tool

Firstly, copy and paste the AssemblyAI API key into the `api.txt` file (you can replace the text `replace_with_your_AssemblyAI_API_key` with your own API key).

Secondly, install prerequisite `pytube` library by typing the following:
```
pip3 install pytube
```

Thirdly, run the transcriber by typing the following (note that you can replace the URL with a YouTube video of your choice):
```
python3 transcriber.py -i "https://www.youtube.com/watch?v=ry9SYnV3svc"
```

# 3. Running transcriber as a Streamlit app
To recreate this web app on your own computer, do the following.

### Create conda environment (Optional)
Firstly, we will create a conda environment called *transcriber*
```
conda create -n transcriber python=3.7.9
```
Secondly, we will login to the *transcriber* environment
```
conda activate transcriber
```

###  Download GitHub repo

```
git clone https://github.com/patil1001/youtube-transcriber-app.git
```

###  Pip install libraries
```
pip install -r requirements.txt
```

###  Launch the app

```
streamlit run app.py
```

