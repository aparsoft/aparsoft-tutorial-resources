# Aparsoft Tutorial Resources
*Code Scripts, Notebooks & Learning Materials for Developers*

[![YouTube](https://img.shields.io/badge/YouTube-Subscribe-red?style=flat&logo=youtube)](https://youtube.com/@aparsoft)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Follow-blue?style=flat&logo=linkedin)](https://linkedin.com/company/aparsoft)
[![Website](https://img.shields.io/badge/Website-aparsoft.com-green?style=flat)](https://aparsoft.com)

![Python](https://img.shields.io/badge/Python-3.12-blue?logo=python)
![LangChain](https://img.shields.io/badge/LangChain-Latest-green)
![LangGraph](https://img.shields.io/badge/LangGraph-Latest-purple)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebooks-orange?logo=jupyter)

> **Tutorial Resources Hub for the Developer Community**
>
> A comprehensive collection of code scripts, Jupyter notebooks, documentation, and learning materials covering LangChain, LangGraph, PostgreSQL integration, and AI application development. All resources are designed to support our YouTube tutorials and developer community.

## What Is This Repository?

This is a **centralized resource hub** containing all the code, scripts, notebooks, and documentation for our Aparsoft tutorial series. It's designed to be a companion repository for developers following our YouTube tutorials and learning AI development.

**What You'll Find:**
- Jupyter notebooks (.ipynb) with hands-on examples
- Code scripts for various AI/ML tasks
- Documentation and guides (Markdown & PDF)
- LangChain and LangGraph implementations
- PostgreSQL integration examples
- Production-ready code patterns
- Assets and resources for tutorials

---

## What You Can Learn

### LangGraph & LangChain
- **Workflows vs Agents** - Understanding the differences and when to use each
- **Workflow Patterns** - Building sequential and conditional workflows
- **Agent Implementation** - Creating intelligent agents with tools
- **Persistence & State Management** - Using PostgreSQL for conversation memory
- **Production Patterns** - Best practices for deploying AI applications

### Database Integration
- **PostgreSQL with LangChain** - Vector storage and retrieval
- **Chat History Management** - Storing and retrieving conversations
- **Auto Summarization** - Implementing conversation summarization
- **Production Setup** - Database configuration for production

### Development Workflows
- **Jupyter Notebooks** - Interactive development and learning
- **Code Scripts** - Reusable patterns and implementations
- **Documentation** - Comprehensive guides and explanations
- **Asset Management** - Commands and utilities for development

---

## Quick Start

### Prerequisites

**Required:**
- Python 3.10+ (we recommend 3.12)
- Jupyter Notebook or JupyterLab
- PostgreSQL (for database examples)
- OpenAI API key (for LangChain/LangGraph examples)

**Optional:**
- Docker (for containerized PostgreSQL)
- VS Code with Jupyter extension

### Getting Started

**1. Clone the Repository**
```bash
git clone https://github.com/aparsoft/aparsoft-tutorial-resources.git
cd aparsoft-tutorial-resources
```

**2. Set Up Your Environment**
```bash
# Create virtual environment
python -m venv venv

# Activate virtual environment
# On macOS/Linux:
source venv/bin/activate
# On Windows:
venv\Scripts\activate

# Install dependencies
pip install jupyter langchain langgraph openai psycopg2-binary
```

**3. Configure Environment Variables**
```bash
# Create .env file
touch .env

# Add your API keys
echo "OPENAI_API_KEY=your_key_here" >> .env
echo "DATABASE_URL=postgresql://user:pass@localhost:5432/dbname" >> .env
```

**4. Start Jupyter Notebook**
```bash
# Launch Jupyter
jupyter notebook

# Or JupyterLab
jupyter lab
```

**5. Explore the Tutorials**
- Start with `langgraph/00_langgraph_workflow_vs_agents.ipynb`
- Follow the numbered sequence for progressive learning

---

## Available Resources

### Jupyter Notebooks (.ipynb)
Interactive notebooks with executable code, explanations, and visualizations:
- Workflows and agents implementation
- Step-by-step tutorials
- Visualization outputs
- Hands-on exercises

### Documentation Files (.md / .pdf)
Comprehensive guides and references:
- Conceptual explanations
- Architecture diagrams
- Best practices
- Production guidelines

### Code Scripts
Reusable code patterns and utilities:
- Helper functions
- Common patterns
- Integration examples
- Deployment scripts

### Assets & Resources
- Command references
- Setup guides
- Conversion utilities
- Logos and branding

---

## About Aparsoft

We're an AI solutions company based in **Bengaluru, India**, dedicated to making AI development accessible to developers worldwide.

**Our Mission:**
- Share practical AI development knowledge
- Build a supportive developer community
- Create high-quality educational content
- Demonstrate production-ready patterns
- Help developers build real AI applications

### Learn With Us

**Main Channels:**
- **Website:** [aparsoft.com](https://aparsoft.com) - Services and contact
- **YouTube:** [@aparsoft-ai](https://youtube.com/@aparsoft-ai) - Weekly tutorials and live coding
- **LinkedIn:** [/company/aparsoft](https://linkedin.com/company/aparsoft) - Articles and insights
- **GitHub:** [@aparsoft](https://github.com/aparsoft) - Open-source projects
- **Twitter/X:** [@aparsoft](https://x.com/AparsoftPvtLtd) - Quick tips and updates

**Subscribe to our YouTube channel** - New content every week!

---

## How to Use This Repository

### For Beginners
1. **Start with notebooks** - Interactive learning is easiest
2. **Follow the sequence** - Numbered tutorials build on each other
3. **Watch YouTube videos** - Companion videos explain concepts
4. **Run the code** - Learn by doing, not just reading
5. **Ask questions** - Use GitHub Discussions or Discord

### For Experienced Developers
1. **Check documentation** - Quick reference for concepts
2. **Review code patterns** - Production-ready implementations
3. **Adapt examples** - Use as templates for your projects
4. **Contribute improvements** - Share your expertise
5. **Explore advanced topics** - Production and scaling guides

### For Content Creators
- Use our diagrams and assets
- Link to our tutorials
- Reference our documentation
- Share your adaptations

---

## Contributing

We welcome contributions from developers at all levels!

**Ways to Contribute:**
- **Add new notebooks** - Share your learning materials
- **Improve documentation** - Make guides clearer
- **Fix issues** - Help improve code quality
- **Share use cases** - Real-world implementations
- **Translate content** - Help non-English speakers
- **Report bugs** - Help us improve

**How to Contribute:**
```bash
# Fork the repo
# Create a branch
git checkout -b feature/your-feature-name

# Make your changes
# Commit with clear messages
git commit -m "Add: description of changes"

# Push and create PR
git push origin feature/your-feature-name
```

---

## Documentation Standards

This repository follows these standards:

### Notebook Formatting
- Clear markdown explanations
- Commented code cells
- Output visualization included
- Requirements at the top
- Summary at the end

### Code Style
- PEP 8 for Python
- Type hints where applicable
- Docstrings for functions
- Comprehensive comments
- Error handling

### Documentation
- Markdown for text docs
- PDF for printable guides
- Images in `*_files/` folders
- Clear naming conventions
- Table of contents for long docs

---

## Useful Commands

### Notebook Management
```bash
# Convert notebook to markdown
jupyter nbconvert --to markdown notebook.ipynb

# Convert notebook to PDF
jupyter nbconvert --to pdf notebook.ipynb

# Convert notebook to HTML
jupyter nbconvert --to html notebook.ipynb

# Run notebook from command line
jupyter nbconvert --to notebook --execute notebook.ipynb
```

### Environment Setup
```bash
# Export requirements
pip freeze > requirements.txt

# Install from requirements
pip install -r requirements.txt

# Update packages
pip install --upgrade langchain langgraph openai
```

### Database Commands
```bash
# Start PostgreSQL with Docker
docker run -d -p 5432:5432 -e POSTGRES_PASSWORD=password postgres

# Connect to database
psql -h localhost -U postgres -d dbname

# Backup database
pg_dump dbname > backup.sql
```

---

## Get Help & Support

### Learning Resources
- **YouTube Tutorials:** [@aparsoft-ai](https://youtube.com/@aparsoft-ai)
- **GitHub Discussions:** Ask questions about code

### Issues & Bugs
- **GitHub Issues:** [Report here](https://github.com/aparsoft/aparsoft-tutorial-resources/issues)
- **Email Support:** support@aparsoft.com

### Professional Services
Need custom AI solutions?
- **Website:** [aparsoft.com](https://aparsoft.com)
- **Email:** contact@aparsoft.com
- **Phone:** +91 8904064878

---

## License

Copyright © 2024 Aparsoft Private Limited. All rights reserved.

This repository is provided for **educational purposes**. You are free to:
- Learn from the code and documentation
- Use the patterns in your own projects
- Modify and adapt for personal/commercial use
- Share with attribution to Aparsoft

**Please attribute when sharing:**
```
Based on tutorials from Aparsoft (https://github.com/aparsoft)
```

---

## Support This Project

**If these resources helped you:**
- Star this repository - Helps others discover it
- Subscribe on YouTube - [@aparsoft-ai](https://youtube.com/@aparsoft-ai)
- Share with community - Help others learn
- Contribute - Add your own tutorials
- Sponsor - Support our educational mission

---

## What's Next?

### Coming Soon
- **Advanced RAG Patterns** - Retrieval-augmented generation tutorials
- **Multi-Agent Systems** - Complex agent orchestration
- **Vector Databases** - Pinecone, Weaviate, Qdrant integration
- **Deployment Guides** - AWS, GCP, Azure deployment
- **Testing Strategies** - Testing LLM applications
- **Cost Optimization** - Reducing API costs

### Stay Updated
- Watch our YouTube channel for announcements
- Follow on LinkedIn for updates
- Check GitHub for new releases
- Join Discord for early access

---

## Related Projects

### Our Other Repositories
- **[django-nextjs-chatbot](https://github.com/aparsoft/django-nextjs-chatbot)** - Full-stack AI chatbot tutorial
- **[langchain-tutorials](https://github.com/aparsoft/langchain-tutorials)** - LangChain deep dives
- **[ai-deployment-guide](https://github.com/aparsoft/ai-deployment-guide)** - Production deployment

### Recommended Learning
- [LangChain Documentation](https://python.langchain.com/)
- [LangGraph Documentation](https://langchain-ai.github.io/langgraph/)
- [OpenAI Cookbook](https://github.com/openai/openai-cookbook)

---

## Repository Stats

- **Total Notebooks:** 8+
- **Documentation Files:** 15+
- **Topics Covered:** LangGraph, LangChain, PostgreSQL, Production
- **Languages:** Python, Markdown
- **Difficulty:** Beginner to Advanced

---

*"Building AI Knowledge Together, One Tutorial at a Time"*

**Built with love by the Aparsoft Team in Bengaluru, India**

**Ready to learn?** [Start with our YouTube tutorials](https://youtube.com/@aparsoft-ai) and code along with these resources!

---

## Acknowledgments

Special thanks to:
- Our YouTube community for feedback and support
- Contributors who improve our tutorials
- Open-source projects we build upon (LangChain, LangGraph)
- Developers worldwide sharing their knowledge

**Together, we're making AI development accessible to everyone!**
