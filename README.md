# Tilt Integration Documentation

This repository contains the public integration documentation for third-party BMS and smart appliances developers who want to integrate with Tilt platform.

## Purpose

This documentation aims to:
- Introduce Tilt's terminology and concepts
- Guide third-party developers in implementing a REST API that conforms to our OpenAPI specification
- Provide clear technical guidelines for authentication and seamless integration

## Documentation Structure

The documentation is built using [MkDocs](https://www.mkdocs.org/) and deployed to GitHub Pages. It includes:

- Introduction to Tilt's platform
- Core concepts and terminology
- API specification (OpenAPI)
- Integration guidelines
- Authentication and security
- Best practices

## Local Development

To run the documentation locally:

1. Install MkDocs:
```bash
pip install mkdocs mkdocs-material mkdocs-redoc-tag
```

2. Run the development server:
```bash
mkdocs serve
```

3. View the documentation at `http://127.0.0.1:8000`

## Deployment

The documentation is automatically deployed to GitHub Pages when changes are pushed to the `main` branch. The deployment process:

1. Builds the documentation using MkDocs
2. Deploys the generated site to the `gh-pages` branch
3. Makes the documentation available at `https://tilt-energy.github.io/integration_documentation/`

You can view the latest deployment status in the [Actions tab](https://github.com/tilt-energy/integration_documentation/actions) of the repository.

## Contributing

We welcome contributions to improve this documentation. Please see our [Contributing Guidelines](docs/contributing.md) for detailed information on how to contribute.

## License

This documentation is licensed under [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/).
