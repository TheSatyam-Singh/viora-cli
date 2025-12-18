<p align="center"><code>npm i -g @universelabs/viora</code><br />or <code>brew install --cask viora</code></p>

<p align="center"><strong>UniVerse Viora CLI</strong> is a coding agent from UniVerse Labs that runs locally on your computer.
</br>
</br>If you want Viora in your code editor (VS Code, Cursor, Windsurf), <a href="https://developers.universelabs.tech/viora/ide">install in your IDE</a>
</br>If you are looking for the <em>cloud-based agent</em> from UniVerse, <strong>Viora Web</strong>, go to <a href="https://viora.universelabs.tech">viora.universelabs.tech</a></p>

<p align="center">
  <img src="./.github/codex-cli-splash.png" alt="Viora CLI splash" width="80%" />
  </p>

---

## Quickstart

### Installing and running UniVerse Viora CLI

Install globally with your preferred package manager. If you use npm:

```shell
npm install -g @universelabs/viora
```

Alternatively, if you use Homebrew:

```shell
brew install --cask viora
```

Then simply run `viora` to get started:

```shell
viora
```

If you're running into upgrade issues with Homebrew, see the [FAQ entry on brew upgrade viora](./docs/faq.md#brew-upgrade-viora-isnt-upgrading-me).

<details>
<summary>You can also go to the <a href="https://github.com/TheSatyam-Singh/viora-cli/releases/latest">latest GitHub Release</a> and download the appropriate binary for your platform.</summary>

Each GitHub Release contains many executables, but in practice, you likely want one of these:

- macOS
  - Apple Silicon/arm64: `viora-aarch64-apple-darwin.tar.gz`
  - x86_64 (older Mac hardware): `viora-x86_64-apple-darwin.tar.gz`
- Linux
  - x86_64: `viora-x86_64-unknown-linux-musl.tar.gz`
  - arm64: `viora-aarch64-unknown-linux-musl.tar.gz`

Each archive contains a single entry with the platform baked into the name (e.g., `viora-x86_64-unknown-linux-musl`), so you likely want to rename it to `viora` after extracting it.

</details>

### Using Viora with your UniVerse account

<p align="center">
  <img src="./.github/codex-cli-login.png" alt="Viora CLI login" width="80%" />
  </p>

Run `viora` and select **Sign in with UniVerse**. We recommend signing into your UniVerse account to use Viora as part of your Plus, Pro, Team, Edu, or Enterprise plan. [Learn more about what's included in your UniVerse plan](https://help.universelabs.tech/en/articles/viora-plans).

You can also use Viora with an API key, but this requires [additional setup](./docs/authentication.md#usage-based-billing-alternative-use-a-universe-api-key). If you previously used an API key for usage-based billing, see the [migration steps](./docs/authentication.md#migrating-from-usage-based-billing-api-key). If you're having trouble with login, please comment on [this issue](https://github.com/TheSatyam-Singh/viora-cli/issues/1).

### Model Context Protocol (MCP)

Viora can access MCP servers. To configure them, refer to the [config docs](./docs/config.md#mcp_servers).

### Configuration

UniVerse Viora CLI supports a rich set of configuration options, with preferences stored in `~/.viora/config.toml`. For full configuration options, see [Configuration](./docs/config.md).

### Execpolicy

See the [Execpolicy quickstart](./docs/execpolicy.md) to set up rules that govern what commands Viora can execute.

### Docs & FAQ

- [**Getting started**](./docs/getting-started.md)
  - [CLI usage](./docs/getting-started.md#cli-usage)
  - [Slash Commands](./docs/slash_commands.md)
  - [Running with a prompt as input](./docs/getting-started.md#running-with-a-prompt-as-input)
  - [Example prompts](./docs/getting-started.md#example-prompts)
  - [Custom prompts](./docs/prompts.md)
  - [Memory with AGENTS.md](./docs/getting-started.md#memory-with-agentsmd)
- [**Configuration**](./docs/config.md)
  - [Example config](./docs/example-config.md)
- [**Sandbox & approvals**](./docs/sandbox.md)
- [**Execpolicy quickstart**](./docs/execpolicy.md)
- [**Authentication**](./docs/authentication.md)
  - [Auth methods](./docs/authentication.md#forcing-a-specific-auth-method-advanced)
  - [Login on a "Headless" machine](./docs/authentication.md#connecting-on-a-headless-machine)
- **Automating Codex**
  - [GitHub Action](https://github.com/openai/codex-action)
  - [TypeScript SDK](./sdk/typescript/README.md)
  - [Non-interactive mode (`codex exec`)](./docs/exec.md)
- [**Advanced**](./docs/advanced.md)
  - [Tracing / verbose logging](./docs/advanced.md#tracing--verbose-logging)
  - [Model Context Protocol (MCP)](./docs/advanced.md#model-context-protocol-mcp)
- [**Zero data retention (ZDR)**](./docs/zdr.md)
- [**Contributing**](./docs/contributing.md)
- [**Install & build**](./docs/install.md)
  - [System Requirements](./docs/install.md#system-requirements)
  - [DotSlash](./docs/install.md#dotslash)
  - [Build from source](./docs/install.md#build-from-source)
- [**FAQ**](./docs/faq.md)
- [**Open source fund**](./docs/open-source-fund.md)

---

## License

This repository is licensed under the [Apache-2.0 License](LICENSE).
