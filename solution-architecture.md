# 🧩 Solution Architecture

## Idea
**LearnSphere AI** converts a student's own document into personalised study experiences using Google Gemini.

## Components

```mermaid
flowchart TB
    S[Student] --> UI[Web UI - Next.js]
    UI --> UP[Document Upload + Exam Setup]
    UI --> SCN[Question Scanner]
    UI --> TUT[AI Tutor / Voice Tutor]
    UP --> API[Server API Route]
    SCN --> API
    TUT --> API
    API --> GEM[Google Gemini API]
    GEM --> API
    API --> OUT[Notes - Answers - Questions - Revision]
    OUT --> GAME[Quests - Practice Arena - Revision Centre]
    GAME --> PROG[Progress Analytics]
```

## Design decisions
| Decision | Reason |
|---|---|
| Document-grounded generation | Keeps content relevant to the student's syllabus. |
| Server-side API route | Protects the Gemini API key. |
| Multimodal input (text, image, voice) | Students ask doubts in different ways. |
| Gamified layer | Improves engagement and consistency. |
| Honest analytics | Builds trust; no invented stats. |
| Vercel hosting | Fast deployment and easy sharing. |
