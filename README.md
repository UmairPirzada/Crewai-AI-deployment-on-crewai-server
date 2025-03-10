# {{crew_name}} Crew

Welcome to the {{crew_name}} Crew project, powered by [crewAI](https://crewai.com). This template is designed to help you set up a multi-agent AI system with ease, leveraging the powerful and flexible framework provided by crewAI. Our goal is to enable your agents to collaborate effectively on complex tasks, maximizing their collective intelligence and capabilities.

## Installation

Ensure you have Python >=3.10 <3.13 installed on your system. This project uses [UV](https://docs.astral.sh/uv/) for dependency management and package handling, offering a seamless setup and execution experience.

First, if you haven't already, install uv:

```bash
pip install uv
```

Next, navigate to your project directory and install the dependencies:

(Optional) Lock the dependencies and install them by using the CLI command:

```bash
crewai install
```

### Customizing

**Add your `GEMINI_API_KEY` into the `.env` file**

- Modify `src/hello_flow/config/agents.yaml` to define your agents
- Modify `src/hello_flow/config/tasks.yaml` to define your tasks
- Modify `src/hello_flow/crew.py` to add your own logic, tools and specific args
- Modify `src/hello_flow/main.py` to add custom inputs for your agents and tasks

## Running the Project

To kickstart your crew of AI agents and begin task execution, run this from the root folder of your project:

```bash
crewai run
```

This command initializes the hello_flow Crew, assembling the agents and assigning them tasks as defined in your configuration.

This example, unmodified, will run the create a `report.md` file with the output of a research on LLMs in the root folder.

## Understanding Your Crew

The hello_flow Crew is composed of multiple AI agents, each with unique roles, goals, and tools. These agents collaborate on a series of tasks, defined in `config/tasks.yaml`, leveraging their collective skills to achieve complex objectives. The `config/agents.yaml` file outlines the capabilities and configurations of each agent in your crew.

## Support

For support, questions, or feedback regarding the {{crew_name}} Crew or crewAI.

- Visit our [documentation](https://docs.crewai.com)
- Reach out to us through our [GitHub repository](https://github.com/joaomdmoura/crewai)
- [Join our Discord](https://discord.com/invite/X4JWnZnxPb)
- [Chat with our docs](https://chatg.pt/DWjSBZn)

Let's create wonders together with the power and simplicity of crewAI.

# Crewai-AI-deployment-on-crewai-server

A CrewAI application that generates creative poems using AI. This project demonstrates the use of CrewAI for creative text generation tasks.

## Features

- Generates random sentence count for poems
- Uses AI to create engaging poems about CrewAI
- Saves generated poems with metadata
- Configurable AI model settings

## Installation

1. Clone the repository:

```bash
git clone https://github.com/UmairPirzada/Crewai-AI-deployment-on-crewai-server.git
cd Crewai-AI-deployment-on-crewai-server
```

2. Create and activate a virtual environment:

```bash
python -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
```

3. Install dependencies:

```bash
pip install -e .
```

## Configuration

1. Create a `.env` file in the root directory
2. Add your API key and model configuration:

```env
GEMINI_API_KEY=your_api_key_here
MODEL="gemini/gemini-2.0-flash"
```

## Usage

Run the application:

```bash
python -m hello_flow.main
```

## Project Structure

```
src/hello_flow/
├── crews/
│   └── poem_crew/
│       ├── config/
│       │   ├── agents.yaml
│       │   └── tasks.yaml
│       └── poem_crew.py
└── main.py
```
