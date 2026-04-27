## Step 5: Add guardrails with safe outputs

Your team wants the agent to propose actions safely instead of making direct changes.

### 📖 Theory: Safe outputs reduce automation risk

`safe-outputs` defines constrained actions that can be validated before execution. This helps teams move faster without granting broad mutation access.

Learn more:

- [Automate repository tasks with GitHub agentic workflows](https://github.blog/ai-and-ml/automate-repository-tasks-with-github-agentic-workflows/)

### ⌨️ Activity: Configure safe outputs

1. Update frontmatter in `.github/workflows/repo-report.md` to include:

   ```yaml
   ---
   on:
     workflow_dispatch:

   permissions:
     contents: read

   tools:
     github:

   safe-outputs:
     create-issue:
       title-prefix: "[repo-report] "
       labels: ["report"]
   ---
   ```

1. Commit your changes.

<details>
<summary>Having trouble? 🤷</summary><br/>

- Use `safe-outputs` exactly (with the hyphen).
- Keep the label list as `report`.

</details>
