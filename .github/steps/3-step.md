## Step 3: Enable tools for the agent

The agent needs access to repository data to perform analysis.

### 📖 Theory: Tools define what the agent can reach

Agentic workflows use a `tools` block to declare integrations. Adding `github` allows repository-aware actions within the boundaries you set.

Learn more:

- [GitHub Copilot documentation](https://docs.github.com/en/copilot)

### ⌨️ Activity: Add the GitHub tool

1. Open `.github/workflows/repo-report.md`.
1. Extend the frontmatter:

   ```yaml
   ---
   on:
     workflow_dispatch:

   permissions:
     contents: read

   tools:
     github:
   ---
   ```

1. Commit the change.

<details>
<summary>Having trouble? 🤷</summary><br/>

- Keep `tools` at the same level as `on` and `permissions`.
- `github:` is present with no extra value under it.

</details>
