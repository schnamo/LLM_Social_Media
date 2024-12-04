# LLM-based qualitative and quantitative analysis of social media comments

## Overview

A pipeline that retrieves comments of videos to a specified hashtag, translates them into English, and analyses them for topics, needs, and experiences using BERTopic and Llama. 

## Prompts used with the Llama Model

| Prompt | Purpose |
| -------|-------- |
| The main topic is {hashtag}. Please give a not too general but conscience subtheme that unifies these words: {topic_words}. Only state the topic. | to give a unifying theme for topic clusters identified by BERTopic |
| Please identify some needs of people interacting with {hashtag} videos in the following list of comments: {list_of_comments}.  | identifying needs expressed in comments |
| Please summarise the summaries in the following text and identify 5 needs: {concatenated_needs_per_video}. | summarise the needs across all videos |
| Please identify some experiences of people interacting with {hashtag} videos in the following list of comments: {list_of_comments}.  | identifying experiences expressed in comments |
| Please summarise the summaries in the following text and identify 5 experiences: {concatenated_needs_per_video}. | summarise the experiences across all videos |

## Workflow

![Overview of the Workflow](workflow.png?raw=true "Overview of the Workflow")

## How to cite

tbc
