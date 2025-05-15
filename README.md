# Jack (Memory Bank) AI Agent

## 1. What's This Repository About?

Jack (Memory Bank) is a powerful AI agent configuration designed to work within your IDE, specifically tailored for the Trae IDE. It provides a blueprint for an AI assistant that maintains a persistent, evolving understanding of your project, significantly enhancing developer productivity and project consistency.

**Why is Jack so great to use?**

*   **Persistent Context:** Unlike standard AI interactions that are often stateless, Jack's Memory Bank provides a structured knowledge base. This allows the AI to maintain context across sessions and tasks, remembering previous discussions, decisions, and project details.
*   **Consistent & Reliable Behavior:** Jack operates based on a defined set of rules and protocols (`jack-agent-prompt.md` and `projectRules.md`). This ensures more predictable and reliable assistance, tailored to your project's needs.
*   **Streamlined Onboarding:** Setting up an AI for a new project can be time-consuming. Jack provides a template and a starting set of rules, making it easier to integrate intelligent assistance from day one.
*   **Active Documentation Partner:** Jack is designed to actively participate in and contribute to your project's documentation through its Memory Bank, helping to keep it up-to-date.
*   **Centralized Knowledge:** The Memory Bank acts as a central, accessible repository for project-specific knowledge, preventing information silos.

This repository provides the core `jack-agent-prompt.md` and the structure for its `.memory-bank/` to help you set up your own instance of Jack.

## 2. How to Set Up Your Own Jack (Memory Bank) Agent in Trae IDE

Setting up your Jack (Memory Bank) agent involves a few simple steps:

1.  **Copy the Agent Prompt:**
    *   Open the `jack-agent-prompt.md` file from this repository **in a raw mode** ([link](https://raw.githubusercontent.com/HIMix/jack-memory-bank/refs/heads/master/jack-agent-prompt.md)).
    *   Copy its entire content.
    *   In your Trae IDE, paste this content into the agent configuration/prompt section for a new or existing AI agent ([Trae Agents Docs](https://docs.trae.ai/ide/agent)).
    *   **Note:** Ensure the content is copied from raw version of a file and pasted correctly without any formatting changes.

2.  **Copy initial `projectRules.md` (Optional):**
    *   At the root of your project, you can create a directory named `.memory-bank`.
    *   You can then copy the `projectRules.md` file from this repository into your new `.memory-bank/` directory. This file contains general operational rules and best practices for Jack.
    *   **Note:** This step is optional. If Jack doesn't find a `.memory-bank` directory or a `projectRules.md` file, it will create them and populate `projectRules.md` with general best practices based on its initial understanding.

    *Example directory structure (if you manually create it):*
    ```
    your-project-root/
    ├── .memory-bank/
    │   └── projectRules.md
    └── ... (your other project files)
    ```

3.  **Ask Jack to Initialize Memory Bank:**
    *   Once the agent prompt is set up, you can instruct Jack to initialize or update its Memory Bank.
    *   **For a new project:** Simply ask Jack to "initialize memory bank" and provide some initial information about your project (e.g., goals, main features, technology stack).
    *   **For an existing project:** Ask Jack to "analyze current project and update memory bank." Jack will then examine your project and start populating its Memory Bank files (`projectOverview.md`, `productContext.md`, `activeContext.md`, `systemPatterns.md`, `techContext.md`, `projectStatus.md`, and `projectRules.md` if not already present or if it needs updates).
    *   You can trigger this process by using keywords like `/plan`, "Planning Mode", or "update memory bank" in your prompt to Jack.
    *   Jack will guide you through creating and populating the necessary Memory Bank files.

4.  **Evolve the Memory Bank:**
    *   As your project progresses, continue to interact with Jack. Use commands like "update memory bank" or engage in planning sessions to ensure Jack keeps its Memory Bank files current.
    *   A well-maintained Memory Bank makes Jack an increasingly insightful and effective assistant, deeply understanding your project's evolving context.

## 3. Useful Links

*   [Trae.ai](https://www.trae.ai/)
*   [Jack (Memory Bank) repo](https://github.com/HIMix/jack-memory-bank)
*   [Tweet for Trae Hackathon](https://x.com/HIMixoidus/status/1922845058304205156)
