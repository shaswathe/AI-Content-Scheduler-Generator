# AI-Content-Scheduler-Generator
AI-powered social media automation platform using n8n, Google Gemini, LinkedIn API, Instagram Graph API, and Unsplash API to automate content generation, approval workflows, image retrieval, and multi-platform publishing.
# 🚀 AI-Powered Social Media Content Scheduler & Generator

An AI-powered social media automation platform built using **n8n, Google Gemini, Google Sheets, Unsplash API, LinkedIn API, and Instagram Graph API**.

This project automates the complete content lifecycle—from content generation and image retrieval to approval workflows and multi-platform publishing—helping businesses maintain a consistent social media presence while significantly reducing manual effort.

---

## 📌 Project Overview

Managing social media manually involves multiple repetitive tasks:

- Content creation
- Image searching
- Content approval
- Multi-platform publishing
- Status tracking

This project automates the entire process using AI and workflow automation, enabling businesses to publish content consistently across social media platforms with minimal human intervention.

---

## 🎯 Project Objectives

- Automate AI-powered content generation
- Retrieve relevant images automatically
- Implement approval-based publishing workflows
- Publish content to LinkedIn and Instagram
- Track publishing status in real-time
- Prevent duplicate posting
- Handle workflow failures automatically
- Reduce manual effort and improve efficiency

---

## 🏗️ System Architecture

```text
Schedule Trigger
       ↓
Google Sheets
       ↓
Filter Approved Content
       ↓
Generate Content (Gemini)
       ↓
Fetch Image (Unsplash)
       ↓
Approval Validation
       ↓
Switch Platform
 ├── LinkedIn Branch
 └── Instagram Branch
       ↓
Publish Content
       ↓
Update Google Sheets
       ↓
Notifications & Logging
```

---

## ⚙️ Technology Stack

| Technology | Purpose |
|------------|----------|
| n8n | Workflow Automation |
| Google Gemini API | AI Content Generation |
| Google Sheets API | Content Management |
| Unsplash API | Image Retrieval |
| LinkedIn API | LinkedIn Publishing |
| Instagram Graph API | Instagram Publishing |
| Gmail API | Email Notifications |
| WhatsApp/SMS API | Mobile Alerts |

---

## 🔄 Workflow Execution

### Step 1: Schedule Trigger

The workflow starts automatically at predefined intervals.

Example:

- Daily at 9:00 AM
- Weekly Campaign Posts
- Custom Marketing Schedules

---

### Step 2: Read Content Topics

The workflow retrieves content topics from Google Sheets.

Example:

| Topic | Approval Status |
|---------|---------|
| AI Automation | Approved |
| Data Analytics | Pending |
| Business Intelligence | Approved |

Google Sheets acts as a content calendar and tracking system.

---

### Step 3: Filter Approved Content

Only content marked as:

```text
Approved
```

proceeds to the next stage.

This prevents accidental publishing and maintains content quality.

---

### Step 4: Generate Content Using Google Gemini

Google Gemini generates:

- Social media captions
- Marketing messages
- Relevant hashtags
- Calls-to-action

Example Prompt:

```text
Generate a professional LinkedIn post about AI Automation.

Tone: Professional
Length: 150 words
Include relevant hashtags and CTA.
```

---

### Step 5: Retrieve Relevant Images

The Unsplash API automatically searches and retrieves relevant images based on the content topic.

Example:

Topic:

```text
Artificial Intelligence
```

Output:

- High-quality image URL
- Attribution information

---

### Step 6: Store Generated Content

Generated content and image URLs are automatically written back into Google Sheets.

Example:

| Topic | Content | Image URL | Status |
|---------|---------|---------|---------|
| AI Automation | Generated | Available | Pending Review |

---

### Step 7: Notifications

Once content generation is completed:

#### Email Notification

Reviewer receives:

```text
New content generated and ready for approval.
```

#### Mobile Notification

WhatsApp/SMS alerts provide instant updates.

---

### Step 8: Publish Content

Using an n8n Switch Node, content is routed to the correct platform.

#### LinkedIn Publishing

- Text Post
- Image Post
- Automated Publishing

#### Instagram Publishing

- Create Media Container
- Wait for Processing
- Publish Media

---

## 🛡️ Error Handling

A dedicated error workflow captures and manages failures.

### Error Workflow

```text
Error Trigger
      ↓
Capture Error
      ↓
Log Details
      ↓
Notify Administrator
```

Handled scenarios:

- API Failures
- Authentication Errors
- Network Issues
- Missing Media Assets
- Publishing Failures

---

## 🔒 Duplicate Protection

To prevent reposting the same content:

The workflow validates:

```text
Posting_Status
```

Example:

```text
Published
```

If already published:

```text
Skip Post
```

This ensures content is never posted twice.

---

## 📊 Results & Business Impact

| Activity | Manual Process | Automated Process |
|-----------|-----------|-----------|
| Content Creation | 30 Minutes | < 1 Minute |
| Image Search | 15 Minutes | Automatic |
| Publishing | 10 Minutes | Automatic |
| Total Time | ~55 Minutes | < 2 Minutes |

### Achievements

✅ Reduced manual effort by over 90%

✅ Automated content creation and publishing

✅ Enabled multi-platform social media management

✅ Improved posting consistency

✅ Implemented approval-based workflow

✅ Added automated error handling and monitoring

---

## 🌟 Key Features

### 🤖 AI Content Generation
- Google Gemini Integration
- Automated Captions
- Marketing Content Creation
- Hashtag Generation

### 🖼️ Automated Image Selection
- Unsplash API Integration
- Topic-Based Image Retrieval

### ✅ Approval Workflow
- Human Review Process
- Controlled Publishing

### 📱 Multi-Platform Publishing
- LinkedIn
- Instagram

### 📈 Status Tracking
- Publishing Status Updates
- Workflow Monitoring

### ⚠️ Error Management
- Failure Notifications
- Error Logging
- Recovery Tracking

---

## 📷 Demo Screenshots

### n8n Workflow

![Workflow Architecture](screenshots/workflow.png)

### Generated Content

![Generated Content](screenshots/content-generation.png)

### LinkedIn Publishing

![LinkedIn Post](screenshots/linkedin-post.png)

### Instagram Publishing

![Instagram Post](screenshots/instagram-post.png)

---

## 🚀 Future Enhancements

- X (Twitter) Integration
- Facebook Integration
- Analytics Dashboard
- Auto Retry Mechanism
- AI Performance Insights
- Content Performance Tracking
- RAG-Based Content Generation
- Vector Database Integration
- Knowledge Base Driven Content Creation

---

## 🧠 Skills Demonstrated

- Workflow Automation (n8n)
- AI Integration
- Prompt Engineering
- REST API Integration
- Google Gemini
- Social Media Automation
- Business Process Automation
- Google Sheets Automation
- LinkedIn API
- Instagram Graph API
- Error Handling & Monitoring

---

## 📈 Business Value

This project transforms a time-consuming manual social media process into a fully automated AI-powered workflow, enabling businesses to:

- Maintain a consistent online presence
- Improve marketing efficiency
- Reduce operational effort
- Scale content production
- Accelerate content publishing

---

## 👨‍💻 Author

**Shaswathe R**

- LinkedIn: https://linkedin.com/in/shaswathe
- GitHub: https://github.com/shaswathe

---

⭐ If you found this project useful, consider giving it a star on GitHub.
