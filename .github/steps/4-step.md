## Step 4: Define the agent task

Now you need to tell the agent what to do.

### 📖 Theory: Natural language drives agent behavior

Instead of procedural steps, you provide a clear outcome and required sections. Specific prompts make output more predictable and useful.

Learn more:

- [Automate repository tasks with GitHub agentic workflows](https://github.blog/ai-and-ml/automate-repository-tasks-with-github-agentic-workflows/)

### ⌨️ Activity: Add instructions below frontmatter

1. In `.github/workflows/repo-report.md`, add this content below frontmatter:

   ```markdown
   # Repository Report

   Generate a report about this repository.

   Include:
   - Recent commits
   - Open pull requests
   ```

1. Commit your update.

<details>
<summary>Having trouble? 🤷</summary><br/>

- Ensure this content is outside frontmatter, below the closing `---`.
- Keep both list items exactly as written for this step.

</details>
