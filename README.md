# 3dd

## Adding This Repository as a Remote

If you have an existing local Git repository and want to add this repository as a remote, follow these steps:

### 1. Add the remote

```bash
git remote add origin https://github.com/Novanz/3dd
```

If you want to use a different name instead of `origin`, replace `origin` with your preferred remote name:

```bash
git remote add upstream https://github.com/Novanz/3dd
```

### 2. Verify the remote was added

```bash
git remote -v
```

You should see output similar to:
```
origin  https://github.com/Novanz/3dd (fetch)
origin  https://github.com/Novanz/3dd (push)
```

### 3. Fetch the remote branches

```bash
git fetch origin
```

**Note:** Replace `origin` with your remote name if you used a different name in step 1.

### 4. Pull changes from the remote (optional)

If you want to merge changes from the remote repository:

```bash
git pull origin main
```

**Note:** Replace `origin` with your remote name if you used a different name in step 1, and replace `main` with the appropriate branch name if different.

### Troubleshooting

If you already have a remote named `origin`, you'll need to either:

- Remove the existing remote first:
  ```bash
  git remote remove origin
  git remote add origin https://github.com/Novanz/3dd
  ```

- Or use a different name for this remote:
  ```bash
  git remote add 3dd-upstream https://github.com/Novanz/3dd
  ```