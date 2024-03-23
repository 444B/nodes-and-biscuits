# Nodes and Biscuits Forum
## Welcome

This repo serves to automatically capture and process a transcript of the podcast, which would be useful to   
- provide a community feedback loop to the [Godot Engine](https://github.com/godotengine/godot) project  
- Improvement proposals,   
- context to the issues discussed on the podcast  

## Proposed workflow   
### 1. Getting Media   
- [Spotify API](https://developer.spotify.com/documentation/web-api/tutorials/getting-started): Get podcast episode and serves as trigger for workflow  
- [Youtube-dl](https://github.com/ytdl-org/youtube-dl) on a VM   
 
### 2. Getting transcript  
[Google Cloud Speech to Text API](https://cloud.google.com/speech-to-text?hl=en) - processing the audio from youtube-dl (if a direct transcript isn't available)  
OR - using [Streamlabs podcast](https://podcasteditor.streamlabs.com/) studio to get transcript   
OR - [Youtube API](https://developers.google.com/youtube/v3): get auto generated captions - less desired since lower quality  
 
### 3. Processing
3. [GPT-4 API](https://platform.openai.com/docs/guides/speech-to-text):  process the transcript file and to capture topics discussed, etc  
 
### 4. Posting ### 
4. [Githubs API](https://docs.github.com/en/rest): publish it to the repo as a discussion and opening issues for anything discussed  
