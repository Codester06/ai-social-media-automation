# AI Social Media Automation using n8n

An end-to-end automation workflow built with **n8n** that detects the latest video from **Google Drive**, generates an AI-powered caption using **Google Gemini**, uploads the media to **Cloudinary**, and automatically publishes it as an **Instagram Reel** through the **Instagram Graph API**.

---

## 🚀 Overview

This workflow eliminates the manual process of posting content to Instagram by automating the complete publishing pipeline. It continuously monitors a Google Drive folder, identifies newly added videos, generates relevant captions using AI, uploads the media to Cloudinary for public access, and publishes the content as an Instagram Reel after verifying that the media has been fully processed.

---

## ✨ Features

- ⏰ **Scheduled Execution** – Runs automatically every **2 hours**.
- 📂 **Smart File Detection** – Detects the latest media file from Google Drive.
- 📁 **Automatic File Management** – Moves processed files to keep folders organized.
- ⬇️ **Media Download** – Downloads videos directly from Google Drive.
- ☁️ **Cloud Upload** – Uploads videos securely to Cloudinary.
- 🤖 **AI Caption Generation** – Creates engaging captions using Google Gemini.
- 📱 **Instagram Reel Publishing** – Automatically creates and publishes Instagram Reels.
- 🔄 **Processing Status Check** – Waits and continuously checks Instagram processing status before publishing.
- ⚡ **Fully Automated Pipeline** – No manual intervention required after uploading a video to Google Drive.

---

## 🛠️ Tech Stack

### Automation
- n8n

### Programming Language
- JavaScript

### APIs & Services
- Google Drive API
- Google Gemini API
- Cloudinary API
- Instagram Graph API

---

## 🔄 Workflow

```text
Schedule Trigger
        │
        ▼
Search Google Drive
        │
        ▼
Select Latest File
        │
        ▼
Move Processed File
        │
        ▼
Download Video
        │
        ▼
Upload to Cloudinary
        │
        ▼
Generate AI Caption (Gemini)
        │
        ▼
Create Instagram Media Container
        │
        ▼
Poll Processing Status
        │
        ▼
Publish Instagram Reel
```

---

## 📋 Workflow Summary

1. The workflow starts automatically on a scheduled interval.
2. Searches a Google Drive folder for available media files.
3. Selects the newest uploaded video.
4. Moves the processed file to prevent duplicate uploads.
5. Downloads the video from Google Drive.
6. Uploads the media to Cloudinary and retrieves a public URL.
7. Uses Google Gemini to generate an AI-powered Instagram caption.
8. Creates an Instagram Reel media container using the Graph API.
9. Waits and periodically checks the media processing status.
10. Automatically publishes the Reel once processing is complete.

---

## 💡 Use Cases

- AI-powered Social Media Automation
- Instagram Content Scheduling
- Creator Workflow Automation
- Marketing Automation
- Content Distribution Pipeline
- No-Code / Low-Code Automation

---

## 📌 Future Improvements

- Support for Facebook Reels
- LinkedIn Post Automation
- YouTube Shorts Publishing
- TikTok Integration
- Multi-Account Posting
- Automatic Hashtag Generation
- AI Image & Video Analysis
- Analytics Dashboard
- Slack/Discord Notifications
- Error Monitoring & Retry System

---
