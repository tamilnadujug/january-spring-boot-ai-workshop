# Spring Boot AI Workshop - January 2026

Welcome! This repository serves as a comprehensive reference guide for learning Spring Boot AI development, featuring materials from two excellent workshops covering different aspects of AI application development.

## 📚 Workshop References

This repository consolidates reference materials from two distinct talks, each focusing on different aspects of Spring AI development:

### 🚀 Talk 1: Spring AI Fundamentals
**Presenter**: Thamarai P  
**Focus**: Core Spring AI Concepts & Implementation  
**Repository**: [spring-ai-workshop](https://github.com/ThamaraiP/spring-ai-workshop)  
**Documentation**: [docs folder](https://github.com/ThamaraiP/spring-ai-workshop/tree/main/docs)

#### What You'll Learn
- Setting up Spring AI applications from scratch
- Connecting to Large Language Models (LLMs)
- Working with prompt templates and prompt engineering
- Implementing chat memory for conversational AI
- Using vector stores for semantic search and RAG (Retrieval-Augmented Generation)
- Function/Tool calling capabilities

#### Workshop Topics
This workshop covers **fundamental Spring AI concepts** through practical examples:

| Topic | Document | Focus Area |
|-------|----------|------------|
| **Setup** | [00.Create Spring AI Application.md](https://github.com/ThamaraiP/spring-ai-workshop/blob/main/docs/00.Create%20Spring%20AI%20Application.md) | Project initialization, dependencies |
| **LLM Integration** | [01.Create REST Controller and Connect to LLM.md](https://github.com/ThamaraiP/spring-ai-workshop/blob/main/docs/01.Create%20REST%20Controller%20and%20Connect%20to%20LLM.md) | REST APIs, model connections |
| **Prompts** | [02-Prompt Template.md](https://github.com/ThamaraiP/spring-ai-workshop/blob/main/docs/02-Prompt%20Template.md) | Dynamic prompt creation |
| **Memory (In-Memory)** | [03-Chat Memory.md](https://github.com/ThamaraiP/spring-ai-workshop/blob/main/docs/03-Chat%20Memory.md) | Conversation history management |
| **Memory (Database)** | [03-Chat Memory - Database.md](https://github.com/ThamaraiP/spring-ai-workshop/blob/main/docs/03-Chat%20Memory%20-%20Database.md) | Persistent conversation storage |
| **Vector Store (Basic)** | [04-Vector Store.md](https://github.com/ThamaraiP/spring-ai-workshop/blob/main/docs/04-Vector%20Store.md) | Semantic search foundations |
| **Vector Store (Database)** | [04-Vector Store - Database.md](https://github.com/ThamaraiP/spring-ai-workshop/blob/main/docs/04-Vector%20Store%20-%20Database.md) | Production vector storage |
| **Tool Calling** | [05-Tool Calling.md](https://github.com/ThamaraiP/spring-ai-workshop/blob/main/docs/05-Tool%20Calling.md) | Function calling with LLMs |

#### Tech Stack
- Spring Boot
- Spring AI
- Vector Databases
- LLM APIs (OpenAI, Azure OpenAI, etc.)

#### Getting Started
```bash
# Clone the repository
git clone https://github.com/ThamaraiP/spring-ai-workshop.git
cd spring-ai-workshop

# Follow the documentation in order, starting with 00.Create Spring AI Application.md
```

#### Who Should Follow This?
- Developers new to Spring AI
- Those building conversational AI applications
- Anyone implementing RAG (Retrieval-Augmented Generation) patterns
- Developers working with vector databases and semantic search

---

### 🔐 Talk 2: MCP Internals, Security & Cloud Deployments
**Presenters**: Shaama M & Muthukumaran  
**Focus**: Building Production-Ready MCP Servers  
**Repository**: [javafest-mcp-internals-security-cd](https://github.com/Shaamam/javafest-mcp-internals-security-cd)

#### What You'll Learn
- Building Model Context Protocol (MCP) servers with Spring Boot
- Multi-protocol support (STDIO, SSE, Stateless communication)
- Firebase authentication and JWT validation
- OAuth2 resource server implementation
- Production deployment strategies (AWS Fargate, Google Cloud Run, Azure Container Apps)
- Security best practices for AI applications

#### Workshop Structure
This is a **progressive 4-chapter tutorial** where each chapter builds on the previous:

| Chapter | Topic | Key Technologies |
|---------|-------|------------------|
| **Chapter 1** | Basic MCP Server with Multi-Protocol Support | Spring AI MCP, H2 Database, Multiple communication protocols |
| **Chapter 2** | Firebase Authentication & User Context | Firebase Admin SDK, Spring Security, JWT validation |
| **Chapter 3** | OAuth2 Resource Metadata & Enhanced Security | OAuth2 standards (RFC 6750/8707), MCP Security Framework |
| **Chapter 4** | Production Deployment & Cloud Configuration | Docker, AWS Fargate, Google Cloud Run, Azure Container Apps |

#### Tech Stack
- Spring Boot 3.5.7
- Spring AI 1.1.0-M4
- Java 21
- Firebase Authentication
- Docker & Container Orchestration

#### Getting Started
```bash
# Clone the repository
git clone https://github.com/Shaamam/javafest-mcp-internals-security-cd.git
cd javafest-mcp-internals-security-cd

# Start with Chapter 1
cd chapter-1
./gradlew bootRun --args='--spring.profiles.active=sse'
```

#### Who Should Follow This?
- Developers building production-ready MCP servers
- Those interested in AI security and authentication patterns
- Teams planning to deploy AI applications to cloud platforms
- Anyone wanting to understand MCP protocol internals

---

## 🎯 Recommended Learning Path

### For Complete Beginners
Start with **Talk 1: Thamarai's Spring AI Fundamentals** to understand core concepts, then move to **Talk 2: Shaama & Muthukumaran's MCP workshop** for production deployment.

```
1. Spring AI Setup & LLM Connection (Talk 1)
2. Prompt Templates & Engineering (Talk 1)
3. Chat Memory & Conversation Management (Talk 1)
4. Vector Stores & RAG (Talk 1)
5. Tool Calling (Talk 1)
→ Then move to Talk 2: MCP Internals for production patterns
```

### For Experienced Developers
If you're already familiar with Spring AI basics, jump directly to **Talk 2: Shaama & Muthukumaran's MCP workshop** to learn production-ready patterns, security, and deployment.

### For Specific Use Cases

| Use Case | Recommended Workshop | Key Chapters/Topics |
|----------|---------------------|---------------------|
| Building chatbots | Talk 1: Thamarai's Workshop | Chat Memory, Prompt Templates |
| Implementing RAG | Talk 1: Thamarai's Workshop | Vector Store, Tool Calling |
| Production deployment | Talk 2: Shaama & Muthukumaran's Workshop | Chapters 3-4 |
| Security & Authentication | Talk 2: Shaama & Muthukumaran's Workshop | Chapters 2-3 |
| MCP Protocol | Talk 2: Shaama & Muthukumaran's Workshop | All Chapters |

---

## 🛠️ Prerequisites

### Common Requirements
- Java 17+ (Java 21 recommended for MCP workshop)
- Gradle or Maven
- IDE (IntelliJ IDEA, VS Code, Eclipse)
- Git
- Basic understanding of Spring Boot

### For Talk 1: Spring AI Workshop
- OpenAI API key or other LLM provider credentials
- Vector database (for Vector Store chapters)

### For Talk 2: MCP Workshop (Chapters 2+)
- Firebase account
- Docker (for Chapter 4)
- Cloud platform account (AWS/GCP/Azure for deployment)

---

## 📖 Additional Resources

### Official Documentation
- [Spring AI Reference](https://docs.spring.io/spring-ai/reference/)
- [Model Context Protocol Specification](https://modelcontextprotocol.io/)
- [Spring Boot Documentation](https://spring.io/projects/spring-boot)

### Community & Support
- [Spring AI GitHub](https://github.com/spring-projects/spring-ai)
- [Spring Community Forums](https://spring.io/community)

### Testing Tools
- [Firebase JWT Testing Tool](https://firebasejwt.muthuishere.site/)
- [MCP Firebase Auth Proxy](https://mcpfirebaseauthserver.muthuishere.site/)

---

## 🤝 Contributors & Acknowledgments

### Workshop Presenters
- **Shaama M** - [LinkedIn](https://www.linkedin.com/in/shaama-m-030115237)
- **Muthukumaran** - [LinkedIn](https://www.linkedin.com/in/muthuishere/)
- **Thamarai P** - [GitHub](https://github.com/ThamaraiP)

### Special Thanks
- Spring AI Team
- Firebase Team
- Spring Boot Community

---

## 📝 Notes

These are **independent workshops** covering different aspects of Spring AI development:

- **Talk 1 (Thamarai's workshop)** focuses on fundamental Spring AI concepts and getting started
- **Talk 2 (Shaama & Muthukumaran's workshop)** focuses on production-ready MCP servers with advanced security and deployment

Choose your learning path based on your current skill level and project requirements!

---

## 📧 Questions or Issues?

Refer to the individual repository's issue tracker:
- [Talk 1: Spring AI Workshop Issues](https://github.com/ThamaraiP/spring-ai-workshop/issues)
- [Talk 2: MCP Workshop Issues](https://github.com/Shaamam/javafest-mcp-internals-security-cd/issues)

Happy Learning! 🚀
