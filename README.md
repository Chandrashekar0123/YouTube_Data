# 📺 YouTube Playlist Data Extraction and Visualization

## 🧩 Problem Statement

YouTube provides vast amounts of content, but analyzing channel or playlist performance manually is inefficient. Content creators and analysts need an automated way to extract key metrics (views, likes, comments, durations) and visualize them for insights into audience engagement and video performance.

---

## 📌 Project Description

This project utilizes the **YouTube Data API v3** to extract detailed video data from one or more YouTube playlists. The extracted data is then processed using Python and visualized using **Power BI**. The result is a structured Excel file and interactive dashboards that offer clear insights into the performance of videos within a playlist or channel.

---
🎬 Demo Video

To showcase the workflow and final dashboards, a demonstration video is included:

📁 Path: [Demo_Video.mp4](./Demo_Video.mp4)

✅ The video walkthrough includes:
- API setup and authentication
- Data extraction process
- Excel output preview
- Power BI dashboard demonstration

---

## 🧠 Approach

### 1. 🔑 API Setup
- Enable **YouTube Data API v3** from [Google Cloud Console](https://console.cloud.google.com/)
- Generate an API Key for access

### 2. 🧪 Data Extraction
- Input: List of YouTube Playlist IDs or URLs
- Output: Video-level data including:
  - `Video Title`
  - `Video ID`
  - `Published Date`
  - `Duration` (parsed from ISO 8601)
  - `View Count`
  - `Like Count`
  - `Comment Count`
  - `Video URL`

### 3. 🧹 Data Processing
- Clean and normalize the API responses
- Convert duration from ISO 8601 to readable format (hh:mm:ss)
- Export to `.xlsx` using `pandas`

### 4. 📊 Data Visualization
- Use Power BI to create dashboards:
  - **Top videos by views**
  - **Likes vs. Comments scatter plot**
  - **Engagement per minute**
  - **Monthly performance trends**

---

## 🛠️ Tech Stack

| Category       | Tools Used                                      |
|----------------|--------------------------------------------------|
| API            | YouTube Data API v3                              |
| Programming    | Python (Pandas, Requests, JSON)                  |
| Output Format  | Excel (XLSX)                                     |
| Visualization  | Power BI                                         |

---


## 🚀 Features

- 🎥 Fetch video details from YouTube playlists
- 📊 Analyze metrics like views, likes, comments, and durations
- 📁 Export structured data to Excel (CSV/XLSX)
- 📈 Visualize trends with Power BI dashboards
- 🔍 Identify top-performing videos & viewer engagement

---

## 🧠 Workflow

1. **API Key Setup**
   - Enable the **YouTube Data API** in [Google Cloud Console](https://console.cloud.google.com/)
   - Generate an API key

2. **Data Extraction**
   - Use `playlistItems` and `videos` endpoints to extract:
     - `title`, `videoId`, `description`, `publishedAt`
     - `viewCount`, `likeCount`, `commentCount`, `duration`

3. **Data Cleaning & Export**
   - Clean JSON responses
   - Parse durations and convert ISO 8601 format
   - Save output to Excel using `pandas`

4. **Visualization in Power BI**
   - Import Excel into Power BI
   - Create dashboards:
     - Top videos by views
     - Likes vs. comments scatter plots
     - Video durations vs. engagement bar charts

---

## 📂 Output Example

| Title               | Views   | Likes   | Comments | Duration | URL                         |
|---------------------|---------|---------|----------|----------|------------------------------|
| AI Tools Overview   | 120,000 | 4,500   | 230      | 12:15    | https://youtu.be/xxxxx       |
| ML Tutorial Basics  | 98,000  | 3,200   | 190      | 10:03    | https://youtu.be/yyyyy       |


---

## 📌 Applications

- **Content Strategy**: Understand audience engagement
- **Trend Monitoring**: Track top-performing content
- **Channel Optimization**: Data-driven video planning

---


