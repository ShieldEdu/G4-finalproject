# 📚 Group 4 Final project 
+ Last updated (0602 by Gyeong-hoon)
+ Presentation is scheduled on June 11 (Tuesday)
+ Overview of the project: This project aims to teach middle school students using the story "The Guardian's Secret," focusing on enhancing listening and writing skills through interactive activities created with Gradio and Python coding.

## Useful Links
|💠[Emoji](https://gist.github.com/rxaviers/7360908) | 💠[ProjectGuide](https://github.com/MK316/Spring2024/blob/main/DLTESOL/project/README.md) | 💠[Reading material](https://raw.githubusercontent.com/MK316/Spring2024/main/DLTESOL/project/story02.txt) | 💠[CodePage](https://github.com/ShieldEdu/G4-finalproject/blob/main/FPG04.ipynb) | 💠 [APP#1] | 💠 [APP#2] | 💠 [APP#3] |

## Lesson Plan

### 1. Introduction
**Main Presenter:**
- Introduce the project and the story "The Guardian's Secret."
- Explain the language objectives: enhancing listening and writing skills.

### 2. Teaching Procedure

#### Listening Activity

**(1) Pre-Listening Activity: Learning New Words**
- **Gradio Wordcloud App**: Create a word cloud highlighting frequent words from the story. Use the word cloud to introduce and discuss new vocabulary.

```python
import gradio as gr
from wordcloud import WordCloud
import matplotlib.pyplot as plt

def create_wordcloud(text):
    wordcloud = WordCloud(width=800, height=400, background_color='white').generate(text)
    plt.figure(figsize=(10, 5))
    plt.imshow(wordcloud, interpolation='bilinear')
    plt.axis('off')
    plt.show()

text = "The Guardian's Secret text goes here..."
gr.Interface(create_wordcloud, text, "plot").launch()


## Lesson Materials

### Story Title: The Guardian's Secret 
+ [text link](https://raw.githubusercontent.com/MK316/Spring2024/main/DLTESOL/project/story02.txt)
+ [image link](https://github.com/MK316/Spring2024/blob/main/DLTESOL/project/Story02.png)

**<Synopsis>**
In Echo Ridge, a mountain village enriched with legends of the "Guardian of the Glen" eagle, adventurous Alex discovers an ancient map in a library book that hints at a hidden treasure in Whispering Hollow cave. Along with friends Mia and Sam, Alex embarks on a challenging expedition through dense forests and rugged terrain. Upon reaching the cave, they find not gold, but historical artifacts including a statuette of the Guardian eagle, which they donate to the local museum. This discovery not only cements their status as local heroes but revitalizes the village's interest in its own lore and history, continuing the legend of the Guardian as a symbol of adventure and cultural heritage.


## Huggingface

