
# Video Automation System

A fully automated **AI video generation workflow** built with **n8n**, **LangChain**, and **Google Gemini**.
This system generates, edits, and uploads short-form ranking videos to YouTube — all without manual work.

---

<img width="1433" height="694" alt="Image" src="https://github.com/user-attachments/assets/30cb68d4-08dd-4a62-8782-d95007020377" />


## Sample Output
Note: This was generated using free models/alternatives.


https://github.com/user-attachments/assets/25ebef1d-2061-4c94-9c39-a7e95d3c73ed





## Overview

Manually creating short-form videos is time-consuming — researching topics, writing scripts, finding visuals, recording voiceovers, and editing each clip.
The goal of this project was to **automate the entire process** using AI tools and workflow automation.

This system combines AI-generated content creation with video rendering and publishing, producing complete YouTube-ready videos in just a few minutes.

---

## How It Works

1. **Topic & Script Generation:**
   Uses **LangChain** and **Google Gemini** to automatically generate trending topics, detailed scripts, and visual prompts.

2. **Video Creation:**
   Sends structured data (script, images, voiceovers) to **Json2Video API**, which automatically compiles and renders a short-form video.

3. **Data Logging:**
   Updates **Google Sheets** to keep track of video topics, upload status, and timestamps.

4. **YouTube Upload:**
   The final rendered video is uploaded directly to **YouTube** using the YouTube Data API.

---

## Results

* Reduced manual video creation time from **hours to under 3 minutes**
* Fully automated **daily content generation and publishing**
* Achieved a **100% hands-free YouTube video production pipeline**
* Ideal for creators, marketers, or automation developers scaling content workflows

---

## Tech Stack

* **Automation:** n8n
* **AI Models:** LangChain + Google Gemini
* **Video Rendering:** Json2Video API
* **Database:** Google Sheets
* **Publishing:** YouTube Data API

---

## Workflow Components

| Component          | Description                            |
| ------------------ | -------------------------------------- |
| LangChain + Gemini | Generate topics, scripts, and prompts  |
| Json2Video API     | Create short-form videos automatically |
| Google Sheets      | Log video data and scheduling info     |
| YouTube Node       | Upload videos directly to YouTube      |
| n8n                | Orchestrates the complete process      |

---

## Setup Instructions

1. **Clone the Repository**

   ```bash
   git clone https://github.com/yourusername/video-automation-system.git
   cd video-automation-system
   ```

2. **Import the Workflow**

   * Open your **n8n dashboard**
   * Click **“Import from File”**
   * Upload the workflow JSON file (`VideoAutomationSystem.json`)

3. **Set Up Credentials**

   * **Google Gemini API** — for topic and script generation
   * **Json2Video API** — for automatic video rendering
   * **Google Sheets OAuth2** — for video tracking
   * **YouTube OAuth2** — for video uploading

4. **Configure Parameters**

   * Update API keys and spreadsheet IDs
   * Customize prompt style or content category
   * Define upload metadata (title, tags, description)

5. **Activate Workflow**

   * Turn on the workflow in n8n
   * The system will automatically generate and upload a new video based on your set schedule

---



## Business Impact

This automation enables effortless AI-driven content creation — ideal for scaling **YouTube automation channels**, media agencies, or educational platforms.
It removes the need for manual editing or creative input while maintaining consistent posting frequency.

---

## Files Included

* `VideoAutomationSystem.json` — Full n8n workflow export
* Optional setup guide for API credentials and scheduling configuration

---

## Future Enhancements

* Integration with **Sora** or **Runway** for advanced video generation
* AI-based voiceover creation using **ElevenLabs**
* Social media repurposing (TikTok, Instagram Reels, Shorts)


