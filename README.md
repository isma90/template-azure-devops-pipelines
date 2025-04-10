# Azure DevOps Modularized Pipelines Template

This repository provides a collection of modularized YAML templates for building comprehensive Azure DevOps pipelines. The design is focused on reusability and maintainability, allowing you to assemble your CI/CD workflows by composing modular pipeline fragments. Use this template as a starting point to create standardized and scalable pipelines across multiple projects.

## Overview

Modern DevOps practices demand pipelines that are easy to manage, extend, and maintain. This template splits the pipeline logic into separate YAML files (modules), enabling you to define reusable jobs, steps, and stages. With this approach, teams can quickly update or extend parts of the pipeline without reworking an entire monolithic configuration file.

## Features

- **Modular Structure:** Define and reuse individual pipeline modules for build, test, deploy, and more.
- **Ease of Customization:** Quickly adjust or extend functionality by modifying or adding new YAML templates.
- **Separation of Concerns:** Separate stages and tasks to maintain a clear overview of the CI/CD process.
- **Azure DevOps Ready:** Designed to be directly integrated with Azure DevOps pipelines, reducing setup and configuration time.

## Repository Structure

Below is an overview of the repository layout:

```bash
template-azure-devops-pipelines/
├── nestjs.yml                  # Main pipeline template.
├── python.yml                  # Main pipeline template.
├── templates/                  # Folder containing pipeline modules (jobs, stages, or reusable steps).
│   ├── package.yml             # module: Build stage definitions.
│   └── unit-test-runner.yml    # module: Test stage definitions.
├── examples/                   # Utility scripts that might be used within pipeline tasks.
│   └── nestjs.yml              # Example script for pipeline usage.
│   └── python.yml              # Example script for pipeline usage.
└── README.md                   # This documentation.
```

## Best Practices

- **Keep Modules Focused:** Each module should perform a specific function. This ensures reusability and easier troubleshooting.
- **Version Control:** Maintain a consistent version for the pipeline modules so that updates can be tracked and applied gradually.
- **Documentation:** Update the documentation within the repository (especially in the `docs/` folder) when new modules or features are added. This fosters better collaboration among team members.

## Contributing

Contributions to improve this template are welcome. If you have enhancements, bug fixes, or new ideas:
- Open an issue to discuss your proposed changes.
- Submit a pull request with detailed descriptions and testing instructions.

## License

This project is licensed under the MIT License. See the  [MIT License](https://opensource.org/license/mit) link for more details.
