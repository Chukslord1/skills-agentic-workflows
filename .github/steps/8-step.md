## Step 8: Automate execution with a schedule

Your team wants this report generated daily without manual intervention.

### 📖 Theory: Schedule triggers support continuous reporting

The `schedule` trigger runs workflows using cron syntax. Combining manual and scheduled triggers gives you both control and automation.

Learn more:

- [Events that trigger workflows: schedule](https://docs.github.com/en/actions/reference/events-that-trigger-workflows#schedule)

### ⌨️ Activity: Add a schedule trigger

1. Open `.github/workflows/repo-report.md`.
1. Update the `on` block to:

   ```yaml
   on:
     workflow_dispatch:
     schedule:
       - cron: '0 9 * * *'
   ```

1. Commit your changes.

<details>
<summary>Having trouble? 🤷</summary><br/>

- Keep the cron expression wrapped in single quotes.
- Ensure `schedule` is under the same `on` block as `workflow_dispatch`.

</details>
