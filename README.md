## GitHub Advisory Database 

A database of CVEs and GitHub-originated security advisories affecting the open source world. 

The database is free and open source and is a tool for and by the community.

Submit pull requests to help improve our database of software vulnerability information for all.

## Goals

* To provide a free and open-source repository of security advisories. 
* To enable our community to crowd-source their knowledge about these advisories. 
* To surface vulnerabilities in an industry-accepted formatting standard for machine interoperability. 

## Features 

All advisories acknowledged by GitHub are stored as individual files in this repository. They are formatted in the [Open Source Vulnerability (OSV) format](https://ossf.github.io/osv-schema/). 

You can submit a pull request to this database (see, [`Contributions`](#contributions)) to change or update the information in each advisory. 

Pull requests will be reviewed and either merged or closed by our internal security advisory curation team. If the advisory originated from a GitHub repository, we will also @mention the original publisher for optional commentary. 

## Contributions

There are two ways to contribute to the information provided in this repository. 

From any individual advisory on [github.com/advisories](https://github.com/advisories), click **Suggest improvements for this vulnerability** (shown below) to open an "Improve security advisory" form. Edit the information in the form and click **Submit improvements** to open a pull request with your proposed changes. 

![Screen shot showing the "Suggest improvements for this vulnerability" link in the right sidebar](https://user-images.githubusercontent.com/8700883/153685286-34c8416e-7021-4a85-b140-a0e5758c959b.png)

Alternatively, you can submit a pull request directly against a file in this repository. To do so, follow the [contribution guidelines](https://github.com/github/advisory-database/blob/main/CONTRIBUTING.md). 

## Supported ecosystems 

Unfortunately, we cannot accept community contributions to advisories outside of our supported ecosystems. Our curation team reviews each community contribution thoroughly and needs to be able to assess each change. 

Generally speaking, our ecosystems are the namespace used by a package registry. As such they’re focused on packages within the registry which tend to be dependencies used in software development.

Our supported ecosystems are:

- Composer (registry: https://packagist.org)
- Erlang (registry: https://hex.pm/)
- GitHub Actions (registry: https://github.com/marketplace?type=actions)
- Go (registry: https://pkg.go.dev/)
- Maven (registry: https://repo.maven.apache.org/maven2)
- npm (registry: https://www.npmjs.com/)
- NuGet (registry: https://www.nuget.org/)
- pip (registry: https://pypi.org/)
- Pub (registry: https://pub.dev/)
- RubyGems (registry: https://rubygems.org/)
- Rust (registry: https://crates.io/)

If you have a suggestion for a new ecosystem we should support, please open an [issue](https://github.com/github/advisory-database/issues) for discussion.

## License 

This project is licensed under the terms of the CC-BY 4.0 open source license. Please [see our documentation](https://docs.github.com/en/github/site-policy/github-terms-for-additional-products-and-features#12-advisory-database) for the full terms.

## FAQ

### Who reviews the pull requests? 

Our internal Security Advisory Curation team reviews the pull requests. They make the ultimate decision to merge or close. If the advisory originated from a GitHub repository, we will also @mention the original publisher for optional commentary. 

### Why is the base branch changed on a PR? 

This repository is a mirror of our advisory database. All contributions to this repository are merged into the main branch via our primary data source to preserve data integrity. 

We automatically create a staging branch for each PR to preserve the GitHub workflow you're used to. When a contribution is accepted from a PR in this repository, the changes are merged into the staging branch and then pushed to the primary data source to be merged into main by a separate process, at which point the staging branch is deleted.

### Will the structure of the database change?  

Here at GitHub, we ship to learn! As usage patterns emerge, we may iterate on how we organize this database and potentially make backwards-incompatible changes to it. 

### Where can I get more information about GitHub advisories?

Information about creating a repository security advisory can be found [here](https://docs.github.com/en/code-security/repository-security-advisories/creating-a-repository-security-advisory), and information about browsing security advisories in the GitHub Advisory Database can be found [here](https://docs.github.com/en/code-security/dependabot/dependabot-alerts/browsing-security-advisories-in-the-github-advisory-database).
