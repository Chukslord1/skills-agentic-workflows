## Step 2: Define execution boundaries with permissions

Your organization requires strict control over what automation can access.

### 📖 Theory: Start with least privilege

The `permissions` block limits what the workflow token can do. For this reporting workflow, read access to repository contents is enough.

Learn more:

- [Automatic token authentication](https://docs.github.com/en/actions/security-guides/automatic-token-authentication)

### ⌨️ Activity: Add permissions

1. Open `.github/workflows/repo-report.md`.
1. Update frontmatter to include:

   ```yaml
   ---
   on:
     workflow_dispatch:

   permissions:
     contents: read
   ---
   ```

1. Commit your update to `main`.

<details>
<summary>Having trouble? 🤷</summary><br/>

- Keep `permissions` inside frontmatter between the `---` lines.
- Use `read`, not `write`.

</details>
