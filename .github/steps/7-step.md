## Step 7: Refine workflow output

The initial report is too basic. You need more useful insights.

### 📖 Theory: Better prompts produce better reports

Prompt quality determines output quality. Adding concrete constraints and expected sections increases consistency across runs.

Learn more:

- [GitHub Copilot documentation](https://docs.github.com/en/copilot)

### ⌨️ Activity: Improve the instruction list

1. Update the instruction content in `.github/workflows/repo-report.md` to include:

   ```markdown
   Include:
   - Top 3 most active pull requests
   - Any failing workflows
   - Suggested next steps
   ```

1. Run the workflow again from the **Actions** tab.
1. Confirm the output includes these richer insights.

<details>
<summary>Having trouble? 🤷</summary><br/>

- Replace the previous `Include:` list with this one.
- If output misses a section, rerun after saving and committing the latest prompt.

</details>
