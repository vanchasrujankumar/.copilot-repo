# Global Copilot Repository

Professional multi-agent, self-learning system for GitHub Copilot with TDD, 100% test coverage, and zero lint issues.

## Features

### 🏗️ Professional Standards
- **Scalable Design**: Modular, stateless agents
- **TDD Approach**: Red-Green-Refactor cycle
- **100% Test Coverage**: All code paths tested
- **Zero Lint Issues**: Strict code quality standards
- **Clean Code**: SOLID principles, DRY, KISS

### 🤖 Multi-Agent System
- **Orchestrator**: Coordinates multiple agents
- **Specialist Agents**: Full Stack, Java, DevOps, Security, Data, QA
- **Self-Learning**: Continuous improvement from interactions
- **Knowledge Base**: Pattern storage and reuse

### 🔌 MCP Integration
- **GitHub, PostgreSQL, Slack, Jira, Notion**
- **Kafka, Grafana, BigQuery**
- **Extensible**: Add custom MCP servers
- **Secure**: Environment variables, no secrets in code

### 🛡️ Security
- **No secrets in repository**
- **Protected configs** (application*.local.*, .env)
- **Pre-commit hooks** for security checks
- **git-crypt** for sensitive files

## Quick Start

### 1. Clone Repository
```bash
git clone https://github.com/your-username/copilot-repo.git
cd copilot-repo
```

### 2. Install Dependencies
```bash
npm install
npm run prepare  # Setup git hooks
```

### 3. Configure Environment
```bash
cp .env.example .env
# Edit .env with your credentials
```

### 4. Setup MCP Servers
```bash
# Install MCP servers
npm install -g @modelcontextprotocol/server-github
npm install -g @modelcontextprotocol/server-postgres
# ... other servers

# Start MCP
npm run mcp:start
```

### 5. Clone Your Projects
```bash
cd workspace
git clone <your-project-url>
```

## Usage

### With GitHub Copilot
1. Open your project in `workspace/`
2. Copilot will use skills and agents
3. Multi-agent orchestration for complex tasks
4. Self-learning improves over time

### Development Workflow
```bash
# Write tests first (TDD)
npm test

# Check code quality
npm run lint:check
npm run format:check
npm run type-check

# Commit with conventional commits
git commit -m "feat: add new agent"
```

## Architecture

### Skills Directory
- **event-driven-systems.md**: Kafka, EventBridge
- **java-microservices.md**: Spring Boot, patterns
- **mongodb.md**: Database design, queries
- **kafka.md**: Streaming, producers, consumers
- **grafana.md**: Monitoring, dashboards
- **vela.md**: Open Application Model
- **spark-scala-hive-bigquery.md**: Big data processing
- **shell-python-nodejs.md**: Scripting, development
- **playwright.md**: E2E testing

### Agents Directory
- **multi-agent-orchestrator.md**: Coordinates agents
- **self-learning-agent.md**: Continuous improvement
- **full-stack-engineer.md**: Web development
- **java-architect.md**: Enterprise architecture
- **devops-engineer.md**: CI/CD, infrastructure
- **security-engineer.md**: Security practices
- **data-engineer.md**: Data pipelines
- **qa-tester.md**: Testing strategies
- **professional-agent-standards.md**: Quality standards

## Security

### Never Commit
- `.env` files
- `application*.local.*` files
- Certificate files (`.pem`, `.crt`, `.key`)
- Database files (`.db`, `.sqlite`)
- API keys, tokens, passwords

### Use
- Environment variables
- `.env.example` template
- git-crypt for sensitive files
- Pre-commit hooks

## Testing

### Requirements
- 100% test coverage
- Fast test execution
- Independent tests
- Realistic test data

### Commands
```bash
# Run all tests
npm test

# Run specific tests
npm run agent:test
npm run skill:test

# Watch mode
npm run test:watch

# CI mode
npm run test:ci
```

## Contributing

1. Fork repository
2. Create feature branch
3. Write tests first (TDD)
4. Implement feature
5. Run all checks
6. Submit pull request

## Support

- **Issues**: GitHub Issues
- **Security**: security@example.com
- **Documentation**: README files

## License

MIT License - see LICENSE file
