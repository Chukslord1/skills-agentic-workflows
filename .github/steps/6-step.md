## Step 6: Run the workflow

Now it is time to execute the workflow and observe the agent in action.

### 📖 Theory: Workflow runs provide execution evidence

Each run captures status and logs. Reviewing logs helps you verify whether the prompt produced the intended result.

Learn more:

- [Monitoring and troubleshooting workflows](https://docs.github.com/en/actions/monitoring-and-troubleshooting-workflows)

### ⌨️ Activity: Run and inspect

1. Open the **Actions** tab in your repository.
1. Select the workflow from `.github/workflows/repo-report.md`.
1. Click **Run workflow**.
1. Open the latest run and inspect logs and output.

<details>
<summary>Having trouble? 🤷</summary><br/>

- If the workflow does not appear, verify the frontmatter syntax first.
- If the run fails, review indentation in the frontmatter and rerun.

</details>
