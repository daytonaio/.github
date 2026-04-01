# Welcome to Daytona

![Daytona Header](https://github.com/daytonaio/.github/blob/main/profile/readme_img.png)

Daytona is a **secure, scalable runtime for AI-generated code execution and agent workflows**. Our open-source platform provides lightning-fast infrastructure (200ms startup) with complete isolation, giving developers and AI systems a safe sandbox for running generated code without risk. The comprehensive **Daytona SDK** offers programmatic control over workspace creation, file operations, and process execution—essential components for building robust AI agents with dynamic lifecycles.

For organizations building AI applications, **Daytona Enterprise** delivers production-ready infrastructure with enterprise-grade security, compliance tools, and flexible deployment options. Our stateful environment snapshots enable persistent agent operations across sessions, making Daytona the ideal foundation for Fortune 500 companies and startups implementing AI agent architectures.

Ready to transform your AI agent infrastructure? [Schedule a demo](https://cal.com/radisic)!

## Articles about Daytona

- [AI Agents Need a Runtime With a Dynamic Lifecycle](https://www.daytona.io/dotfiles/ai-agents-need-a-runtime-with-a-dynamic-lifecycle-here-s-why)
- [Securing AI Code: Building Safe Sandboxes with Daytona SDK](https://www.daytona.io/dotfiles/securing-ai-code-building-safe-sandboxes-with-daytona-sdk)
- [Run AI-Generated Code Safely with Daytona Sandboxes](https://www.daytona.io/dotfiles/run-ai-generated-code-safely-with-daytona-sandboxes-part-1)
- [Building Better AI Agents with Daytona SDK](https://www.daytona.io/dotfiles/building-better-ai-agents-the-ai-enablement-stack)
- [Sandboxing AI Development with Agent-Agnostic Infrastructure](https://www.daytona.io/dotfiles/sandboxing-ai-development-with-agent-agnostic-infrastructure)

> Read more on our blog, the [Dotfiles Insider](https://www.daytona.io/dotfiles/).

## Quick Start

1. Create an account at [app.daytona.io](https://app.daytona.io)
2. Generate a [new API key](https://app.daytona.io/dashboard/keys)
3. Follow [documentation](https://www.daytona.io/docs/) to start using Daytona

> Daytona provides a comprehensive set of [guides](https://www.daytona.io/docs/en/guides) and [examples](https://www.daytona.io/docs/en/getting-started#examples) to help you get started.

## Creating your first Sandbox

### Python SDK

```py
from daytona import Daytona, DaytonaConfig

config = DaytonaConfig(api_key="YOUR_API_KEY")
daytona = Daytona(config)
sandbox = daytona.create()
response = sandbox.process.code_run('print("Hello World!")')
print(response.result)
```

### Typescript SDK

```jsx
import { Daytona } from "@daytonaio/sdk";

const daytona = new Daytona({apiKey: "YOUR_API_KEY"});
const sandbox = await daytona.create();
const response = await sandbox.process.codeRun('print("Hello World!")');
console.log(response.result);
```

### Ruby SDK

```ruby
require 'daytona'

config = Daytona::Config.new(api_key: 'YOUR_API_KEY')
daytona = Daytona::Daytona.new(config)
sandbox = daytona.create
response = sandbox.process.code_run(code: 'print("Hello World!")')
puts response.result
```

### Go SDK

```go
package main

import (
  "context"
  "fmt"
  "github.com/daytonaio/daytona/libs/sdk-go/pkg/daytona"
  "github.com/daytonaio/daytona/libs/sdk-go/pkg/types"
)

func main() {
  config := &types.DaytonaConfig{APIKey: "YOUR_API_KEY"}
  client, _ := daytona.NewClientWithConfig(config)
  ctx := context.Background()
  sandbox, _ := client.Create(ctx, nil)
  response, _ := sandbox.Process.ExecuteCommand(ctx, "echo 'Hello World!'")
  fmt.Println(response.Result)
}
```
