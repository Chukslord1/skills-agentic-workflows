## Step 1: Create the workflow skeleton

Your team needs a workflow that can be triggered on demand.

### 📖 Theory: Agentic workflows use Markdown and frontmatter

Agentic workflows focus on intent instead of scripting every command. You define the trigger and boundaries in frontmatter, then describe the outcome in natural language.

Learn more:

- [GitHub Actions overview](https://docs.github.com/en/actions)
- [Automate repository tasks with GitHub agentic workflows](https://github.blog/ai-and-ml/automate-repository-tasks-with-github-agentic-workflows/)

### ⌨️ Activity: Create the workflow file

1. Create a file named `.github/workflows/repo-report.md`.
1. Add this frontmatter:

   ```yaml
   ---
   on:
     workflow_dispatch:
   ---
   ```

1. Commit your change to the `main` branch.

<details>
<summary>Having trouble? 🤷</summary><br/>

- Make sure the file extension is `.md`, not `.yml`.
- Confirm `workflow_dispatch` is indented under `on`.

</details>
