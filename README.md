# Memora – Every Memory Deserves a Story

**Memora** is an AI-powered, multi-agent storytelling platform that transforms scattered photographs, personal notes, conversations, and life experiences into meaningful digital stories and beautifully designed memory books.

Instead of simply storing memories, Memora uses collaborative AI agents to collect, organize, write, review, and prepare stories, helping people preserve their special moments effortlessly.

## ✨ Key Features

- **AI-Powered Storytelling:** Transform personal memories into engaging narratives.
- **Memory Collection:** Gather photographs, messages, notes, and personal experiences.
- **Automated Organization:** Organize memories and use available capture dates to structure stories.
- **Multi-Agent Collaboration:** Specialized AI agents work together to complete the storytelling process.
- **Story Editing:** Review and refine generated narratives for clarity and factual consistency.
- **Digital Storybooks:** Generate beautifully formatted memory books and previews.
- **Human Approval:** Maintain human control over public publishing.
- **Collaborative Workspace:** Use Mattermost for communication between AI agents.

## 🤖 Multi-Agent Architecture

Memora uses four specialized AI agents that collaborate through Switch AI.

| Agent | Responsibility |
|---|---|
| Collector | Collects photographs, messages, and personal memories. |
| Storyteller | Creates meaningful narratives using collected memories and evidence. |
| Editor | Reviews and refines stories for quality and factual accuracy. |
| Publisher | Prepares digital storybook previews and manages publishing workflows. |

### How It Works

1. Users share their photographs, notes, and memories.
2. The Collector gathers and organizes the available information.
3. The Storyteller transforms the collected information into a narrative.
4. The Editor reviews and improves the generated story.
5. The Publisher prepares the final digital storybook preview.
6. Human approval is required before public publication.

## 🔗 How We Use Switch AI

Switch acts as the central communication and coordination layer in Memora.

We connected multiple AI agents, including Claude Code and Codex, through Switch to create a collaborative multi-agent workflow.

**Our integration includes:**
- Switch AI for agent communication and task coordination.
- Claude Code for AI-powered storytelling workflows.
- Codex for editing and reviewing content.
- Mattermost as the collaboration platform.
- Shared rooms, messages, documents, and task handoffs between agents.

This architecture allows agents to collaborate as a team instead of operating as isolated AI systems.

## 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| Python | Core application and agent logic |
| FastAPI | Backend API |
| HTML, CSS, JavaScript | Frontend interface |
| Switch AI | Multi-agent coordination |
| Claude Code | Story generation |
| Codex | Content editing and review |
| Mattermost | Agent communication |
| SQLite | Application storage |
| PostgreSQL | Switch infrastructure storage |
| Docker & Docker Compose | Containerization and deployment |

## 🏗️ Architecture

```text
                 USER
                   |
                   v
             MEMORA WEB APP
                   |
                   v
             COLLECTOR AGENT
                   |
                   v
                SWITCH
                   |
          MATTERMOST ROOM
                   |
                   v
            STORYTELLER
             (Claude Code)
                   |
                   v
                EDITOR
                (Codex)
                   |
                   v
               PUBLISHER
                   |
                   v
          DIGITAL STORYBOOK
                   |
                   v
           HUMAN APPROVAL
```

## 🚀 Getting Started

### Prerequisites

Before running Memora, make sure you have:

- Windows, macOS, or Linux.
- Docker Desktop or Docker Engine.
- Docker Compose.
- Git.

### Installation

**1. Clone the repository**

```bash
git clone YOUR_REPOSITORY_URL
```

**2. Navigate to the project directory**

```bash
cd memoryweaver-stories-main
```

**3. Configure environment variables**

Create or configure your environment file using the project's provided configuration template. Add the required credentials and settings for Switch and the AI agents.

Never commit API keys, passwords, or private tokens to GitHub.

**4. Build and start the application**

```bash
docker compose up -d --build
```

**5. Check running services**

```bash
docker compose ps
```

**6. View application logs**

```bash
docker compose logs -f
```

### Access Memora

| Service | Local URL |
|---|---|
| Memora Web App | http://localhost:8787 |
| Mattermost | http://localhost:8065 |
| Switch API | http://localhost:8000 |

*Service availability depends on the configured Docker Compose setup.*

## 🎯 Project Objective

Our goal is to make memory preservation easier, smarter, and more meaningful. Memora combines AI-powered storytelling with multi-agent collaboration to turn ordinary photographs and personal experiences into stories that people can revisit and cherish.

## 🔮 Future Improvements

- More personalized storytelling styles.
- Additional language support.
- Improved photo recognition and memory organization.
- More AI model and agent integrations.
- Enhanced storybook customization.
- Easier agent monitoring and workflow debugging.
- Additional export and sharing formats.

## 👥 Built With

Memora is developed as an exploration of AI-powered storytelling, autonomous agents, and collaborative multi-agent systems.

**Every memory deserves a story.** ❤️
