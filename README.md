# Jackson Antonio do Prado Lima - Curriculum Vitae

This repository contains my CV, generated using [RenderCV](https://github.com/rendercv/rendercv) from YAML source files.

📄 **View my CV**: [https://jacksonpradolima.github.io](https://jacksonpradolima.github.io)

## Quick Links

- 📥 [Download PDF](https://jacksonpradolima.github.io/Jackson_Antonio_do_Prado_Lima_CV.pdf)
- 🌐 [View Online (HTML)](https://jacksonpradolima.github.io/Jackson_Antonio_do_Prado_Lima_CV.html)
- 📝 [Markdown Version](https://jacksonpradolima.github.io/Jackson_Antonio_do_Prado_Lima_CV.md)

## About This Repository

This repository stores my CV in YAML format and automatically generates PDF, HTML, and Markdown versions using GitHub Actions. The generated files are published to GitHub Pages.

## Editing the CV

The CV source file is `Jackson_Prado_Lima_CV.yaml`. To make changes:

### Option 1: Using Dev Container (Recommended)

1. Install [VS Code](https://code.visualstudio.com/) and [Docker](https://www.docker.com/)
2. Install the [Dev Containers extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)
3. Open this repository in VS Code
4. Click "Reopen in Container" when prompted
5. Edit `Jackson_Prado_Lima_CV.yaml`
6. The devcontainer includes all necessary tools and VS Code extensions

### Option 2: Local Editing

```bash
# Install RenderCV
pip install 'rendercv[full]'

# Edit the YAML file
# Then generate outputs locally:
rendercv render Jackson_Prado_Lima_CV.yaml
```

### Automatic Updates

When you push changes to the `main` branch, GitHub Actions automatically:
- Generates PDF, HTML, and Markdown versions
- Publishes them to GitHub Pages

## Technical Details

- **Source Format**: YAML (RenderCV schema)
- **PDF Generation**: Typst (via RenderCV)
- **CI/CD**: GitHub Actions
- **Hosting**: GitHub Pages

## Legacy Files

Previous LaTeX-based CVs are preserved in the `academic/` and `public_tender/` directories for reference.

## More Information

- [RenderCV Documentation](https://docs.rendercv.com/)
- [RenderCV GitHub Repository](https://github.com/rendercv/rendercv)
