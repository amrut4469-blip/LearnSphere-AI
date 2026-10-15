# 🏗 Architecture

LearnSphere AI is a **document-grounded** study platform built with **Next.js** and **Google Gemini**.

```mermaid
flowchart TB
    subgraph Client[Client - Next.js]
        UI[Dashboard and Modes]
        CAM[Camera / Gallery]
        VOICE[Voice Tutor]
    end
    subgraph Server[Server - API Routes]
        RT[AI Route Handler]
        ENV[(GEMINI_API_KEY)]
    end
    subgraph AI[Google Gemini]
        TXT[Text]
        VIS[Vision]
        AUD[Voice]
    end
    UI --> RT
    CAM --> RT
    VOICE --> RT
    ENV -.-> RT
    RT --> TXT
    RT --> VIS
    RT --> AUD
```

## Principles
| Principle | Meaning |
|---|---|
| Grounded | Answers come from the student's own document. |
| Honest | No sample questions or invented progress stats. |
| Engaging | Quests and practice turn studying into a game. |
| Multimodal | Text, images and voice. |
| Secure | Secrets stay on the server. |

## Deployment
Hosted on **Vercel**. See [deployment.md](deployment.md).
