# Roadmap for Members of Comp Dept.

Step by step guide for members of Comp Dept., THUASTA.

```mermaid
flowchart TB
  %% Hide lines for styling
  %% os --- prog_lang
  %% testing --- networking
  %% linkStyle 0,1 stroke:transparent;

  subgraph apis[Learn about APIs]
    rest[REST]
    grpc{{gRPC}}
    graphql{{GraphQL}}
  end

  subgraph build_sys[Build Systems]
    cmake[CMake]
    make{{Make}}
  end

  subgraph ci_cd[CI/CD]
    github_actions[GitHub Actions]
  end

  subgraph container[Containerization]
    docker[Docker]
    k8s{{Kubernetes}}
  end

  subgraph docs[Documentation]
    doxygen{{Doxygen}}
    mkdocs{{MkDocs}}
    docfx{{DocFX}}
  end

  subgraph format_lint[Formatting and Linting]
    clang_format{{Clang-Format}}
    clang_tidy{{Clang-Tidy}}
    black{{Black}}
    pylint{{Pylint}}
  end

  subgraph networking[Networking]
    internet[Internet]
    http[HTTP]
    websockets[WebSockets]
  end

  subgraph os[OS and General Knowledge]
    terminal[Terminal Usage]
    commands[Basic Terminal Commands]
  end

  subgraph packages[Package Management]
    conda[Conda]
    poetry[Poetry]
  end

  subgraph prog_lang[Learn a Language]
    c_cpp[C/C++]
    python[Python]
    csharp[C#]
    go{{Go}}
  end

  subgraph rel_db[Relational Database]
    postgres{{PostgreSQL}}
    mysql{{MySQL}}
    sqlite{{SQLite}}
  end

  subgraph testing[Testing]
    unit_testing[Unit Testing]
    integration_testing[Integration Testing]
  end

  subgraph vcs[VCS and Repo Hosting]
    git[Git]
    github[GitHub]
    gitlab{{GitLab}}
  end

  markdown[Markdown]
  unity{{Unity}}
  

  markdown --> terminal
  terminal --> commands
  commands --> c_cpp
  c_cpp --> python
  python --> csharp
  csharp --> cmake
  cmake --> conda
  conda --> poetry
  poetry --> git
  git --> github
  github --> github_actions
  github_actions --> unit_testing
  unit_testing --> integration_testing
  integration_testing --> docker
  docker --> internet
  internet --> http
  http --> websockets
  websockets --> rest


  csharp -.-> go
  csharp -.-> unity
  cmake -.-> make
  github -.-> gitlab
  github_actions -.-> doxygen
  doxygen -.-> mkdocs
  mkdocs -.-> docfx
  docfx -.-> clang_format
  clang_format -.-> clang_tidy
  clang_tidy -.-> black
  black -.-> pylint
  docker -.-> k8s
  internet -.-> postgres
  postgres -.-> sqlite
  sqlite -.-> mysql
  rest -.-> grpc
  grpc -.-> graphql


  click cmake "../../topics/build_sys/cmake"
  click commands "../../topics/os/commands"
  click conda "../../topics/packages/conda"
  click csharp "../../topics/prog_lang/csharp"
  click c_cpp "../../topics/prog_lang/c_cpp"
  click docker "../../topics/container/docker"
  click git "../../topics/vcs/git"
  click github "../../topics/repo/github"
  click github_actions "../../topics/ci_cd/github_actions"
  click http "../../topics/networking/http"
  click integration_testing "../../topics/testing/int_testing"
  click internet "../../topics/networking/internet"
  click markdown "../../topics/markdown"
  click poetry "../../topics/packages/poetry"
  click python "../../topics/prog_lang/python"
  click rest "../../topics/apis/rest"
  click terminal "../../topics/os/terminal"
  click unit_testing "../../topics/testing/unit_testing"
  click vscode "../../topics/vscode"
  click websockets "../../topics/networking/websockets"
```
