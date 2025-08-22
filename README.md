# 🤖 AI-Agent - Intelligent Research & Web Scraping Platform

A cutting-edge AI-powered research and web scraping platform featuring two sophisticated agents built with LangChain, LangGraph, and advanced AI technologies. Discover developer tools, analyze companies, and extract web data with intelligent automation.

![Python](https://img.shields.io/badge/Python-3.12+-blue.svg)
![LangChain](https://img.shields.io/badge/LangChain-0.3.25+-green.svg)
![LangGraph](https://img.shields.io/badge/LangGraph-0.4.8+-purple.svg)
![OpenAI](https://img.shields.io/badge/OpenAI-GPT--4-orange.svg)
![Firecrawl](https://img.shields.io/badge/Firecrawl-2.7.1+-red.svg)

## 🚀 Features

### 🧠 Advanced Research Agent
- **🔍 Intelligent Tool Discovery** - Automatically finds and analyzes developer tools
- **�� Company Analysis** - Comprehensive research on tech companies and their offerings
- **📊 Structured Data Extraction** - Extracts pricing, tech stack, API availability, and more
- **🔄 Multi-Step Workflow** - Advanced LangGraph-powered research pipeline
- **📈 Comparative Analysis** - Side-by-side tool comparisons with recommendations
- **🎯 Developer-Focused Insights** - Language support, integration capabilities, DX ratings

### 🌐 Simple Web Scraping Agent
- **🕷️ Intelligent Web Crawling** - Advanced web scraping with Firecrawl integration
- **�� Content Extraction** - Extract structured data from any website
- **🔗 MCP Protocol Support** - Model Context Protocol for tool integration
- **💬 Conversational Interface** - Natural language interaction for web scraping tasks
- **⚡ Real-time Processing** - Instant data extraction and analysis

### ��️ Core Capabilities
- **🤖 AI-Powered Analysis** - GPT-4 integration for intelligent insights
- **📋 Structured Output** - Pydantic models for reliable data structures
- **🔐 Environment Management** - Secure API key handling
- **📦 Modern Python** - Type hints, async/await, and best practices
- **🎯 Task Automation** - Streamlined workflows for research tasks

## ��️ Architecture

### Advanced Agent Structure
📂 advanced-agent/

├── 📁 src/

│   ├── 🔄 workflow.py        # LangGraph workflow orchestration

│   ├── 📊 models.py          # Pydantic data models  

│   ├── 💭 prompts.py         # AI prompt engineering

│   ├── 🕷️ firecrawl.py       # Web scraping service

│   └── 📦 __init__.py

├── 🖥️ main.py               # CLI interface

└── ⚙️ pyproject.toml         # Dependencies & config

### Simple Agent Structure
📂 simple-agent/

├── 🖥️ main.py               # MCP-based web scraping agent

└── ⚙️ pyproject.toml         # Dependencies & config


## 🛠️ Tech Stack

### 🤖 AI & Machine Learning
- **OpenAI GPT-4** - Advanced language model for analysis
- **LangChain** - AI application framework
- **LangGraph** - Stateful AI workflows
- **Pydantic** - Data validation and serialization

### 🌐 Web Scraping & Data
- **Firecrawl** - Advanced web scraping and crawling
- **MCP Protocol** - Model Context Protocol for tool integration
- **Async/Await** - High-performance concurrent operations

### �� Python Ecosystem
- **Python 3.12+** - Modern Python with type hints
- **uv** - Fast Python package manager
- **python-dotenv** - Environment variable management

## 🚀 Getting Started

### 🌟 What You Need

- **Python 3.12+** 🐍
- **uv package manager** ��
- **OpenAI API key** 🤖
- **Firecrawl API key** 🕷️

### 🛠️ Installation

1. **Clone the repo**
   
   git clone https://github.com/yourusername/ai-agent.git
   cd ai-agent
   

3. **Set up environment variables**
   
   Create `.env` files in both `advanced-agent/` and `simple-agent/` directories:
   # OpenAI API Key
   OPENAI_API_KEY=your_openai_api_key_here
   
   # Firecrawl API Key
   FIRECRAWL_API_KEY=your_firecrawl_api_key_here
  

4. **Install dependencies**
   
   # For Advanced Agent
   cd advanced-agent
   uv sync
   
   # For Simple Agent
   cd ../simple-agent
   uv sync


5. **Start the agents**
   
   # Advanced Research Agent
   cd advanced-agent
   python main.py
   
   # Simple Web Scraping Agent
   cd ../simple-agent
   python main.py


## 🎯 Usage Examples

### Advanced Research Agent
**Example queries:**
- "Find the best code review tools"
- "Compare CI/CD platforms"
- "Research database monitoring solutions"
- "Analyze project management tools for developers"

### Simple Web Scraping Agent
**Example commands:**
- "Scrape the pricing page of company X"
- "Extract all blog posts from this website"
- "Get the tech stack information from this page"
- "Crawl and analyze this documentation site"



## �� Features in Detail

### 🔍 Advanced Research Agent Features

#### Intelligent Tool Discovery
- **Article Analysis** - Scans tech articles and comparison posts
- **Tool Extraction** - Identifies relevant tools from content
- **Smart Filtering** - Focuses on developer-relevant solutions

#### Comprehensive Company Analysis
- **Pricing Models** - Free, Freemium, Paid, Enterprise analysis
- **Tech Stack Detection** - Identifies technologies used
- **API Availability** - Checks for developer APIs
- **Language Support** - Programming language compatibility
- **Integration Capabilities** - Third-party integrations
- **Developer Experience** - DX ratings and insights

#### Structured Data Output

class CompanyInfo(BaseModel):
    name: str
    website: str
    pricing_model: str
    tech_stack: List[str]
    api_available: bool
    language_support: List[str]
    integration_capabilities: List[str]
    developer_experience_rating: str


### 🌐 Simple Web Scraping Agent Features

#### MCP Protocol Integration
- **Tool Discovery** - Automatic tool loading via MCP
- **Standardized Interface** - Consistent tool interaction
- **Extensible Architecture** - Easy to add new tools

#### Conversational Interface
- **Natural Language** - Ask for data in plain English
- **Context Awareness** - Maintains conversation context
- **Error Handling** - Graceful error recovery

## �� Configuration

### Environment Variables

#### Advanced Agent

OPENAI_API_KEY=sk-...          # OpenAI API key
FIRECRAWL_API_KEY=fc_...       # Firecrawl API key


#### Simple Agent

OPENAI_API_KEY=sk-...          # OpenAI API key
FIRECRAWL_API_KEY=fc_...       # Firecrawl API key


### Model Configuration
- **GPT-4o-mini** - Fast and cost-effective for research
- **Temperature: 0.1** - Consistent, focused responses
- **Structured Output** - Pydantic models for reliability

## 📈 Example Output

### Advanced Agent Research Results

🔍 Developer Tools Query: code review tools
📊 Results for: code review tools
============================================================
🏢 GitHub
🌐 Website: https://github.com
�� Pricing: Freemium
�� Open Source: False
��️ Tech Stack: Git, REST API, GraphQL
💻 Language Support: All languages
🔌 API: ✅ Available
🔗 Integrations: CI/CD, IDEs, Slack
📝 Description: Comprehensive code review with inline comments...
🏢 GitLab
🌐 Website: https://gitlab.com
�� Pricing: Freemium
�� Open Source: True
��️ Tech Stack: Git, Ruby, Go
💻 Language Support: All languages
🔌 API: ✅ Available
🔗 Integrations: Kubernetes, Docker, AWS
📝 Description: Complete DevOps platform with advanced code review...
Developer Recommendations:
For small teams: GitHub provides excellent integration...
For enterprise: GitLab offers comprehensive DevOps...


## 🔒 Security

- **Environment Variables** - Secure API key management
- **Type Safety** - Pydantic validation for all data
- **Error Handling** - Graceful failure recovery
- **Rate Limiting** - Respectful API usage

## 🚀 Deployment

### Local Development

# Advanced Agent
cd advanced-agent
uv run python main.py

# Simple Agent
cd simple-agent
uv run python main.py


### Production Considerations
- **API Key Rotation** - Regular key updates
- **Rate Limiting** - Monitor API usage
- **Logging** - Comprehensive error tracking
- **Monitoring** - Performance metrics

## 🤝 Contributing

1. **Fork the repository** 🍴
2. **Create a feature branch** `git checkout -b feature/AmazingFeature`
3. **Commit your changes** `git commit -m 'Add AmazingFeature'`
4. **Push to the branch** `git push origin feature/AmazingFeature`
5. **Open a Pull Request** 🚀

### Development Setup

# Install development dependencies
uv sync --dev

# Run tests (when implemented)
uv run pytest

# Format code
uv run black .
uv run isort .

# Type checking
uv run mypy .


**Ready to revolutionize your research workflow? Dive into AI-Agent today! 🚀**

That's all





