# Curriculum Vitae - RenderCV

This repository uses [RenderCV](https://github.com/rendercv/rendercv) to generate professional CVs/resumes from YAML files.

## Features

- **RenderCV**: Modern CV generation using YAML instead of LaTeX
- **VS Code Integration**: Live preview and auto-completion support
- **Dev Container**: Ready-to-use development environment with all dependencies

## Getting Started

### Using Dev Container (Recommended)

1. Install [VS Code](https://code.visualstudio.com/) and [Docker](https://www.docker.com/)
2. Install the [Dev Containers extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)
3. Open this repository in VS Code
4. Click "Reopen in Container" when prompted (or use Command Palette: "Dev Containers: Reopen in Container")
5. Wait for the container to build and install dependencies

### Local Installation

If you prefer not to use Dev Containers:

```bash
# Install Python 3.10 or higher
# Install RenderCV
pip install rendercv

# Install LaTeX (required for PDF generation)
# On Ubuntu/Debian:
sudo apt-get install texlive-full

# On macOS:
brew install --cask mactex

# On Windows, install MiKTeX or TeX Live
```

## Usage

### Generating a CV

```bash
# Render CV to PDF
rendercv render Jackson_Prado_Lima_CV.yaml

# Output will be in rendercv_output/ directory
```

### Editing with Live Preview

When using VS Code with the Dev Container:

1. Open the YAML CV file (e.g., `Jackson_Prado_Lima_CV.yaml`)
2. The live preview should automatically activate
3. Edit the YAML file and save to regenerate the PDF

## CV File Structure

CV files are in YAML format with the following structure:

```yaml
cv:
  name: Your Name
  location: Your Location
  email: your.email@example.com
  phone: "+1234567890"
  social_networks:
    - network: LinkedIn
      username: yourprofile
  sections:
    Education:
      - institution: University Name
        degree: PhD
        start_date: 2020
        end_date: present
    Experience:
      - company: Company Name
        position: Job Title
        start_date: 2020-01
        end_date: 2022-12
        highlights:
          - Achievement 1
          - Achievement 2
design:
  theme: classic
  color: rgb(0,79,144)
```

## Documentation

- [RenderCV Documentation](https://docs.rendercv.com/)
- [RenderCV GitHub](https://github.com/rendercv/rendercv)
- [VS Code Setup Guide](https://docs.rendercv.com/user_guide/how_to/set_up_vs_code_for_rendercv/)

## Migration from LaTeX

The previous LaTeX-based CVs are preserved in the `academic/` and `public_tender/` directories for reference.
