# Comp Dept.

Step by step guide for members of Comp Dept., THUASTA.

```mermaid
flowchart TB
  %% Hide lines for styling
  prog_lang --- os
  testing --- networking
  linkStyle 0,1 stroke:transparent;

  subgraph pre_knowledge[Premilinary Knowledge]
    markdown[Markdown]
    vscode[VSCode]
    code_styling[Code Styling]

    click markdown "../pre_knowledge/markdown"
    click vscode "../pre_knowledge/vscode"
  end

  subgraph prog_lang[Learn a Language]
    c_cpp[C/C++]
    python[Python]
    csharp[C#]
    go{{Go}}

    click python "../prog_lang/python"
    click csharp "../prog_lang/csharp"
  end

  subgraph vcs[Version Control System]
    git[Git]

    click git "../vcs/git"
  end

  subgraph repo[Repo Hosting Service]
    github[GitHub]

    click github "../repo/github"
  end

  subgraph os[OS and General Knowledge]
    terminal[Terminal Usage]
    commands[Basic Terminal Commands]

    terminal --> commands

    click terminal "../os/terminal"
    click commands "../os/commands"
  end

  subgraph testing[Testing]
    unit_testing[Unit Testing]
    integration_testing[Integration Testing]

    click unit_testing "../testing/unit_testing"
    click integration_testing "../testing/int_testing"
  end

  subgraph ci_cd[CI/CD]
    github_actions[GitHub Actions]

    click github_actions "../ci_cd/github_actions"
  end

  subgraph container[Containerization]
    docker[Docker]
    k8s{{Kubernetes}}

    docker -.-> k8s

    click docker "../container/docker"
  end

  subgraph networking[Networking]
    internet[Internet]
    http[HTTP]
    websockets[WebSockets]

    internet --> http
    internet --> websockets

    click internet "../networking/internet"
    click http "../networking/http"
    click websockets "../networking/websockets"
  end

  subgraph rel_db[Relational Database]
    postgres{{PostgreSQL}}
  end

  unity{{Unity}}

  vscode --> prog_lang
  commands --> git
  git --> github
  github --> github_actions
  commands --> docker
  commands --> testing

  internet -.-> postgres
  csharp -.-> unity
```
