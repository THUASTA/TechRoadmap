# Comp Dept.

Step by step guide for members of Comp Dept., THUASTA.

```mermaid
flowchart TB
  subgraph pre_knowledge[Premilinary Knowledge]
    markdown[Markdown]
  end

  subgraph prog_lang[Learn a Language]
    direction LR

    python[Python]
    csharp[C#]

    python --> csharp
  end

  subgraph vcs[Version Control System]
    git[Git]
  end

  subgraph repo[Repo Hosting Service]
    github[GitHub]
  end

  subgraph os[OS and General Knowledge]
    direction LR

    terminal[Terminal Usage]
    posix[POSIX Basics]
    commands[Basic Terminal Commands]

    terminal --> posix
    posix --> commands
  end

  subgraph testing[Testing]
    direction LR

    unit_testing[Unit Testing]
    integration_testing[Integration Testing]

    unit_testing --> integration_testing
  end

  subgraph ci_cd[CI/CD]
    github_actions[GitHub Actions]
  end

  subgraph container[Containerization]
    docker[Docker]
  end

  subgraph networking[Networking]
    direction LR

    http[HTTP]
    websockets[WebSockets]

    http --> websockets
  end

  unity[Unity]

  pre_knowledge --> prog_lang
  prog_lang --> vcs
  vcs --> repo
  repo --> os
  os --> testing
  testing --> ci_cd
  ci_cd --> container
  container --> networking
  networking --> unity
```