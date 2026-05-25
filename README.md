# Global Copilot Repository

This repository contains skills and agents for AI-assisted development with GitHub Copilot.

## Multi-Agent & Self-Learning Approach

### Multi-Agent System
- **Orchestrator**: Coordinates multiple specialized agents
- **Specialist Agents**: Domain experts (Full Stack, Java, DevOps, Security, Data, QA)
- **Aggregator**: Combines results from multiple agents
- **Self-Learning**: Continuously improves from interactions

### Self-Learning Model
- **Experience Learning**: Learn from successful patterns
- **Context Learning**: Adapt to project context
- **Performance Learning**: Optimize responses
- **Feedback Loop**: Improve based on user feedback

## Structure

- **skills/** - Reusable skills for different technologies
- **agents/** - Multi-agent system with self-learning capabilities
- **workspace/** - Clone your repos here to use these skills

## Available Skills

### Core Technologies
- Event-driven systems
- Java microservices
- MongoDB
- Kafka
- Grafana
- Vela
- Spark, Scala, Hive, BigQuery
- Shell, Python, Node.js, npm, JavaScript
- Playwright (testing)

## Available Agents

### Multi-Agent System
- **multi-agent-orchestrator** - Coordinates multiple agents
- **self-learning-agent** - Continuously learns and improves

### Role-Specific Agents
- Full Stack Engineer
- Java Architect
- DevOps Engineer
- Security Engineer
- Data Engineer
- QA Tester

## Usage

1. Clone your repos to the `workspace/` directory
2. Configure Copilot to use skills from this repo
3. Use multi-agent approach for complex tasks
4. Enable self-learning for continuous improvement

## Data-Driven & Test-Driven Approach

All skills and agents follow:
- **Data-driven**: Based on real-world patterns and best practices
- **Test-driven**: Emphasize TDD/BDD with comprehensive test coverage

## Configuration

See `.copilot-config.json` for multi-agent and self-learning settings.
