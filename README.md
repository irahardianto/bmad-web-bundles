<div align="center">
  <!-- <a href="https://github.com/irahardianto/bmad-web-bundles">
    <img src="assets/logo.png" alt="Logo" width="80" height="80">
  </a> -->

<h3 align="center">BMad Web Bundles</h3>

  <p align="center">
    <strong>Self-contained AI Agent & Team Environments based on the BMad Methodology.</strong>
    <br />
    Load entire software development teams into your LLM context with a single file.
    <br />
  </p>
</div>

<!-- ABOUT THE PROJECT -->
## About The Project

**BMad Web Bundles** is a repository of AI-ready "Web Bundles" designed to implement the **BMad Methodology (BMM)**. 

The repository is a mirror of web bundles in the [BMad Method Repo](https://github.com/bmad-code-org/BMAD-METHOD/tree/main), I used to easily find the package in v4, but since upgraded to v6, its not so easy to find, as such I decided to create this mirror, so I can easily discover it.

These bundles are not traditional software you install on your OS. Instead, they are self-contained **XML environments** that you load into a Large Language Model (LLM) context (like Gemini, ChatGPT, or Claude). 

Once loaded, these bundles provide the LLM with:
*   **Specialized Personas:** Experts like Architects, Product Managers, and Developers.
*   **Core OS:** A lightweight execution engine for running complex workflows.
*   **Embedded Knowledge:** Guidelines, templates, and best practices (e.g., how to write a Professional grade PRD).

This allows you to instantly spin up a virtual software development team inside a chat window, capable of following structured SDLC processes from ideation to code.

### Key Components

*   **`agents/`**: Individual specialist bundles (e.g., `architect.xml`, `dev.xml`, `pm.xml`). Each contains the specific persona, commands, and knowledge for that role.
*   **`teams/`**: Multi-agent bundles (e.g., `team-fullstack.xml`). These include an "Orchestrator" that can dynamically switch between different specialist roles to handle complex, multi-stage projects.

### Built With

*   **XML**: The container format for all bundles.
*   **YAML**: Used for defining workflows and task structures.
*   **Markdown**: Used for documentation and templates.
*   **BMad Methodology**: The underlying theoretical framework for the agent interactions.

<!-- GETTING STARTED -->
## Getting Started

To use these bundles, you don't need a compiler or a package manager. You just need an AI interface.

### Prerequisites

*   Access to an advanced LLM (e.g., Google Gemini, OpenAI ChatGPT, Anthropic Claude).
*   Ability to upload files or paste large amounts of text into the chat context.

### Installation

1.  **Clone the repo** to your local machine (to access the files).
    ```sh
    git clone https://github.com/irahardianto/bmad-web-bundles.git
    ```
2.  **Locate the bundle** you want to use (e.g., `teams/team-fullstack.xml`).
3.  **Upload the XML file** to your LLM chat session.
    *   *Alternatively, open the file in a text editor, copy the entire content, and paste it into the chat.*

#### Gemini Gems Example

1. **Select the Agent** pick the agent directive you want to use e.g. `agents/analyst.xml`
2. **Create a new Gem** go to gem manager, and create New Gem
3. **Add instructions option A** copy paste the agent directive and add to the Gem instructions
4. **Add instructions option B** add the agent directive file as the knowledge (change the extension .txt if its not supporting xml) of the Gem and put the following in the instruction box
```
All of your operating instructions and resources are contained in the XML file attached. Read in the initial agent block and instructions to understand it. You will not deviate from the character and rules outlined in the attached!
```

<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE` for more information.

---
<p align="center">
  Built with ❤️ for the Developer Community
</p>