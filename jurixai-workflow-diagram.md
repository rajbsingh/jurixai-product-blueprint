# JurixAI Workflow Diagram

This diagram shows a high-level JurixAI legal document review workflow.

```mermaid
flowchart TD
    A[User Uploads Legal Document] --> B[Document Type Identification]
    B --> C[Key Information Extraction]
    C --> D[Clause Extraction]
    D --> E[Risk Flagging]
    E --> F[Plain-Language Summary]
    F --> G[Questions for Legal Review]
    G --> H{Risk Level}

    H -->|Low| I[User Review]
    H -->|Medium| J[Legal Professional Review Recommended]
    H -->|High| K[Qualified Legal Review Required]

    I --> L[Structured Output]
    J --> L
    K --> L

    L --> M[Disclaimer and Final Review Note]
```

## Design Principle

JurixAI should assist legal professionals and businesses, but it should not replace qualified legal advice.

High-risk legal outputs should always include human professional review.
