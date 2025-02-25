# Welcome to Daytona
![Daytona Header](https://github.com/daytonaio/.github/blob/main/profile/readme_img.png)

Daytona is a **secure, scalable runtime for AI-generated code execution and agent workflows**. Our open-source platform provides lightning-fast infrastructure (200ms startup) with complete isolation, giving developers and AI systems a safe sandbox for running generated code without risk. The comprehensive **Daytona SDK** offers programmatic control over workspace creation, file operations, and process execution—essential components for building robust AI agents with dynamic lifecycles.

For organizations building AI applications, **Daytona Enterprise** delivers production-ready infrastructure with enterprise-grade security, compliance tools, and flexible deployment options. Our stateful environment snapshots enable persistent agent operations across sessions, making Daytona the ideal foundation for Fortune 500 companies and startups implementing AI agent architectures.

## Here are some articles about Daytona:
- [AI Agents Need a Runtime With a Dynamic Lifecycle](https://www.daytona.io/dotfiles/ai-agents-need-a-runtime-with-a-dynamic-lifecycle-here-s-why)
- [Securing AI Code: Building Safe Sandboxes with Daytona SDK](https://www.daytona.io/dotfiles/securing-ai-code-building-safe-sandboxes-with-daytona-sdk)
- [Run AI-Generated Code Safely with Daytona Sandboxes](https://www.daytona.io/dotfiles/run-ai-generated-code-safely-with-daytona-sandboxes-part-1)
- [Building Better AI Agents with Daytona SDK](https://www.daytona.io/dotfiles/building-better-ai-agents-the-ai-enablement-stack)
- [Sandboxing AI Development](https://www.daytona.io/dotfiles/sandboxing-ai-development-with-agent-agnostic-infrastructure)

Read more on our blog, the [Dotfiles Insider](https://www.daytona.io/dotfiles/), or explore our open source [Documentation](https://www.daytona.io/docs/).

Ready to transform your AI agent infrastructure? [Schedule an Enterprise Demo](https://daytona.zapier.app/)

Get started with Daytona in seconds:
```python
from daytona_sdk import Daytona

daytona = Daytona()
workspace = daytona.create()

# Run AI-generated code securely inside isolated sandbox
response = workspace.process.code_run('print("Hello from AI sandbox!")')
print(response.result)
```
