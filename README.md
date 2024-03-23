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

# Sample
Process using streamlabs to capture transcript and ChatGPT4 to create .md 
<details>
 <summary>Prompt used</summary>
I have an audio transcript.
Please process it and provide it back to me as an .md file with the following sections
# Title, date
## TLDR
## Topics discussed
## Issues or proposals mentioned which are relevant to Godot
## Other points
</details>


# Nodes and Biscuits: A Dive into Godot Plugins and Game Development Insights
**Date:** [Insert Date of Podcast Here]

## TL;DR
- Christoph Klestil and Big Brain discuss the intricacies of developing plugins for the Godot Engine.
- Topics include the creation of Behave and Pandora plugins, game development processes, and insights into Godot's community and future directions.
- Focus on issues and proposals relevant to Godot, including plugin development challenges and strategies for effective community engagement.

## Topics Discussed
- **Plugin Development in Godot:** Big Brain shares his journey into Godot plugin development, highlighting the Behave and Pandora plugins. Behave allows designing behavior trees in the editor, while Pandora simplifies handling RPG data at scale.
- **Community Engagement and Support:** The challenges of maintaining popular plugins, such as Behave, which has garnered significant attention and use within the Godot community.
- **Game Development Processes:** Insights into Big Brain's current game project and his approach to game development, including naming conventions, storytelling, and creating immersive worlds.
- **Future Directions for Godot:** Discussion on the evolution of Godot, addressing both its strengths and areas for improvement, particularly in terms of UI/UX design and plugin support.

## Issues or Proposals Mentioned Relevant to Godot
- **Enhancing Plugin Support:** The conversation touches on the need for better support and documentation for plugin developers in Godot to foster a more vibrant ecosystem.
- **Godot Version Compatibility:** Big Brain mentions the importance of ensuring plugins remain compatible with new versions of Godot, suggesting more streamlined processes or tools for plugin developers to manage version transitions.

## Other Points
- **The Power of Community:** Both speakers emphasize the importance of community feedback in the development of plugins and games. They discuss how engaging with the community can lead to better software solutions and more enjoyable game experiences.
- **Challenges of Indie Game Development:** Insights into the balancing act of indie game development, including time management, prioritizing features, and dealing with the uncertainties of creative endeavors.
"""
