# matrix
# Multi-Platform Matrix Build Demo

This repository demonstrates a GitHub Actions workflow with matrix builds and artifact management.

## Contact Information

**Email**: 23f2005572@ds.study.iitm.ac.in

## Workflow Overview

This project implements a multi-platform CI/CD pipeline using GitHub Actions matrix strategy.

### Matrix Configuration

The workflow builds across multiple configurations:
- **Operating Systems**: Ubuntu, macOS, Windows
- **Node.js Versions**: 16, 18, 20
- **Total Combinations**: 7 parallel jobs

### Features

✅ **Parallel Execution**: All matrix variants run simultaneously  
✅ **Artifact Generation**: Each job creates unique build artifacts  
✅ **Cross-Platform**: Tests on Linux, macOS, and Windows  
✅ **Metadata Tracking**: JSON metadata for each build  
✅ **Build Summary**: Aggregated results from all matrix jobs  

### Artifacts

Each matrix job produces:
- `output.txt` - Build information and environment details
- `metadata.json` - Structured build metadata

Artifact naming convention: `build-1b08871-{os}-node{version}`

### Running the Workflow

The workflow triggers on:
- Push to `main` or `master` branch
- Pull requests
- Manual dispatch (Actions tab → Run workflow)

### Viewing Results

1. Go to the **Actions** tab in this repository
2. Click on the latest workflow run
3. View the **Artifacts** section at the bottom
4. Download any artifact to inspect the build outputs

### Validation Checklist

- [x] At least 3 matrix jobs configured
- [x] All jobs run in parallel
- [x] Each job generates unique artifacts
- [x] Artifacts use `build-1b08871-` prefix
- [x] Step identifier `matrix-1b08871` included
- [x] All artifacts contain actual content
- [x] README contains email address

## Project Structure

```
.
├── .github/
│   └── workflows/
│       └── matrix-build.yml
└── README.md
```

## Technologies

- GitHub Actions
- Node.js (16, 18, 20)
- Multi-platform builds (Ubuntu, macOS, Windows)

---

**Repository**: [Add your GitHub URL here]  
**Workflow Status**: ![CI](https://github.com/YOUR_USERNAME/YOUR_REPO/workflows/Multi-Platform%20Matrix%20Build/badge.svg)
