# LLM-based qualitative and quantitative analysis of social media comments

## Overview

A pipeline that retrieves comments of videos to a specified hashtag, translates them into English, and analyses them for topics, needs, and experiences using BERTopic and Llama. Combines quantitative with qualitative analysis.

## Prompts used with the Llama Model

| Prompt | Purpose |
| -------|-------- |
| The main topic is {hashtag}. Please give a not too general but concise subtheme that unifies these words: {topic_words}. Only state the topic. | to give a unifying theme for topic clusters identified by BERTopic |
| Please identify some needs of people interacting with {hashtag} videos in the following list of comments: {list_of_comments}.  | to identify needs expressed in comments |
| Please summarise the summaries in the following text and identify 5 needs: {list_of_needs_per_video}. | to summarise the needs across all videos |
| Please identify some experiences of people interacting with {hashtag} videos in the following list of comments: {list_of_comments}.  | to identify experiences expressed in comments |
| Please summarise the summaries in the following text and identify 5 experiences: {list_of_experiences_per_video}. | to summarise the experiences across all videos |

## Workflow

![Overview of the Workflow](workflow.png?raw=true "Overview of the Workflow")

## How to cite

If you find this useful please cite Tumescheit C, Sou D, Nißen M, Kowatsch T, Hastings J. Large Language Models Reveal Menstruation Experiences and Needs on Social Media. Stud Health Technol Inform. 2025 Aug 7;329:748-752. doi: 10.3233/SHTI250940. PMID: 40775958.
https://doi.org/10.3233/shti250940