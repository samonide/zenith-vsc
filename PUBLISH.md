# Publishing Guide

Complete instructions for packaging and publishing the Zenith Theme to the VS Code Marketplace.

## Prerequisites

Install the VS Code Extension Manager:

```bash
npm install -g @vscode/vsce
```

## Step 1: Create a Publisher Account

1. Go to https://marketplace.visualstudio.com/manage
2. Sign in with your Microsoft account
3. Click **Create a publisher**
4. Choose a unique publisher name (e.g., "samonide")
5. Fill in the required details

## Step 2: Get a Personal Access Token

1. Go to https://dev.azure.com/
2. Click on your profile icon → **Personal access tokens**
3. Click **+ New Token**
4. Configure the token:
   - **Name**: VS Code Marketplace
   - **Organization**: All accessible organizations
   - **Expiration**: Choose your preferred duration
   - **Scopes**: Click "Show all scopes"
   - Check **Marketplace** → **Manage**
5. Click **Create**
6. **Copy the token** (you won't be able to see it again!)

## Step 3: Update package.json

Update the `publisher` field in `package.json`:

```json
{
  "publisher": "your-publisher-name",
  ...
}
```

## Step 4: Package the Extension

Create a `.vsix` file:

```bash
vsce package
```

This creates: `zenith-theme-3.0.0.vsix`

### Common Issues

- **Missing README**: Ensure README.md exists
- **Missing LICENSE**: Ensure LICENSE file exists
- **Icon warnings**: Icon is optional, you can ignore these warnings

## Step 5: Test Locally

Before publishing, test the extension:

```bash
code --install-extension zenith-theme-3.0.0.vsix
```

Or in VS Code:
1. Press `Ctrl+Shift+P`
2. Type "Extensions: Install from VSIX"
3. Select the `.vsix` file
4. Test all theme variants

## Step 6: Publish to Marketplace

### Option A: Publish with CLI

```bash
vsce publish
```

You'll be prompted for your Personal Access Token.

### Option B: Upload Manually

1. Go to https://marketplace.visualstudio.com/manage/publishers/YOUR-PUBLISHER-NAME
2. Click **+ New extension**
3. Choose **Visual Studio Code**
4. Upload the `.vsix` file
5. Click **Upload**

## Step 7: Verify Publication

1. Go to https://marketplace.visualstudio.com/items?itemName=YOUR-PUBLISHER-NAME.zenith-theme
2. Check that all information is correct
3. Test installation from marketplace

## Updating the Extension

1. Update version in `package.json`:
   ```json
   "version": "3.0.1"
   ```

2. Update `CHANGELOG.md` with changes

3. Commit changes:
   ```bash
   git add .
   git commit -m "Release v3.0.1"
   git tag v3.0.1
   git push && git push --tags
   ```

4. Package and publish:
   ```bash
   vsce package
   vsce publish
   ```

   Or publish directly with version bump:
   ```bash
   vsce publish patch  # 3.0.0 -> 3.0.1
   vsce publish minor  # 3.0.0 -> 3.1.0
   vsce publish major  # 3.0.0 -> 4.0.0
   ```

## Quick Reference

```bash
# Package
vsce package

# Publish (will prompt for token)
vsce publish

# Publish with version bump
vsce publish patch|minor|major

# Login to save token
vsce login YOUR-PUBLISHER-NAME

# Show extension info
vsce show

# List all files that will be packaged
vsce ls
```

## Troubleshooting

### "Cannot find publisher"

Run:
```bash
vsce login your-publisher-name
```
Enter your Personal Access Token when prompted.

### "Missing README.md"

Ensure `README.md` exists in the root directory.

### "Invalid publisher"

Update the `publisher` field in `package.json` to match your publisher account name.

### "Icon not found"

Icons are optional. Either:
- Remove `"icon"` field from `package.json`
- Or create the icon file

### Token expired

Create a new Personal Access Token and run:
```bash
vsce login your-publisher-name
```

## Best Practices

1. **Version Numbers**: Follow semantic versioning (MAJOR.MINOR.PATCH)
2. **Changelog**: Always update CHANGELOG.md before publishing
3. **Testing**: Test locally before publishing
4. **Git Tags**: Tag releases in git for easy tracking
5. **GitHub Releases**: Create GitHub releases alongside marketplace updates

## Resources

- [VS Code Publishing Extensions](https://code.visualstudio.com/api/working-with-extensions/publishing-extension)
- [Extension Manifest Reference](https://code.visualstudio.com/api/references/extension-manifest)
- [Marketplace Publisher Management](https://marketplace.visualstudio.com/manage)

---

**Ready to publish?** Follow the steps above and share Zenith with the world! 🚀
