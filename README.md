![nventive](https://nventive-public-assets.s3.amazonaws.com/nventive_logo_github.svg?v=2)

# Azure Devops Pipeline Templates

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg?style=flat-square)](LICENSE)

This repository contains templates and examples for creating Azure Devops pipelines. You can easily create templates using job templates in the `templates` directory as building blocks. Usage examples of each job templates are available withing the `examples` directory along with more complete examples in the `examples/complete` directory.

The templates cover the following use cases:

- Building, testing a dotnet project
- Building and pushing a Docker image

## How to use a template in this repositotry

Firstly you will need to create a service connection to GitHub in your Azure Devops project settings. After that, follow any of the examples in the `examples` directory and make sure to include the following configuration in your pipeline YAML file:

```yaml
resources:
  repositories:
    - repository: pipeline-templates
      name: nventive/pipeline-templates
      type: github
      endpoint: githubServiceConnection
      # We recommend pinning the template to a specific version
      # ref: refs/tags/1.0.0
```

## Breaking Changes

Please consult [BREAKING_CHANGES.md](BREAKING_CHANGES.md) for more information about version history and compatibility.

## Contributing

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on the process for
contributing to this project.

Be mindful of our [Code of Conduct](CODE_OF_CONDUCT.md).

## We're hiring

Look for current openings on BambooHR https://nventive.bamboohr.com/careers/

## Stay in touch

[nventive.com](https://nventive.com/) | [Linkedin](https://www.linkedin.com/company/nventive/) | [Instagram](https://www.instagram.com/hellonventive/) | [YouTube](https://www.youtube.com/channel/UCFQyvGEKMO10hEyvCqprp5w) | [Spotify](https://open.spotify.com/show/0lsxfIb6Ttm76jB4wgutob)
