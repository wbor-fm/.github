# Hello!

[WBOR (91.1 FM)](https://wbor.org) is the noncommercial, community public radio station licensed to Bowdoin College. This is the public repository for our technology operations. We develop in-house solutions to many of the technical problems that we face. Please [contact us](https://wbor.org/contact) if you have any questions or would like to become involved in projects.

## APIs

Powered by [our Spinitron proxy](https://github.com/wbor-fm/spinitron-proxy), you may fetch WBOR [Spinitron API data](https://spinitron.github.io/v2api/) using the base URL `https://api-1.wbor.org/api` (example: [recent spins](https://api-1.wbor.org/api/spins)).

## System Architecture

Our online streams are made possible [AzuraCast](https://github.com/AzuraCast/AzuraCast/), an excellent piece of open source software. In terms of hosting, we are split between on and off-prem servers. Off-prem we currently use [DigitalOcean droplets](https://www.digitalocean.com/products/droplets).

### Diagram

Coming soon!

## Contributing
We're delighted you want to help contribute to our technical operations. We welcome folks at all levels of experience.

If you'd like to make changes, please follow these steps:
1. Clone the repo that you would like to make changes to your personal GitHub account.
2. Make changes in your local repo.
3. Create a pull request to the main WBOR repo. Someone will review your code and provide feedback if needed.

## Code Style

[See guidelines here.](https://github.com/wbor-fm/.github/blob/main/STYLE.md)
