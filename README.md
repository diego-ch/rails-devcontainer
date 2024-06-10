# rails-devcontainer
This repository contains a Docker development environment for Ruby on Rails applications using Alpine Linux as the base image.

## Features
- Lightweight Alpine Linux base image
- Pre-installed Ruby and Rails dependencies

## Getting Started
To get started with this development environment, follow these steps:

1. Install Docker and Docker Compose if you haven't already.
2. Install VSCode and the [Dev Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers) extension.
3. Copy the .devcontainer folder to your rails app root directory
4. Run the command `> Reopen in Container` on VSCode.

## Troubleshooting
If your app uses sqlite3, you must update your `Gemfile` to use a `version >= 2.0`
to bypass dependency errors.

```
gem sqlite3 "~> 2.0", ">= 2.0.0"
```