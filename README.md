# Automated Prebuilt kernel builder

This script will automatically build a prebuilt kernel for your device. It will also automatically upload images to the specified kernel repository after each successful build.

## Pre-requisites
- You must have a kernel manifest repository. Refer to [THIS LINK](https://github.com/Statix-Gram/android_kernel_manifest) to get started with your manifest.

- You must have a kernel repository. Refer to [THIS LINK](https://github.com/sajidshahriar72543/kernel_xiaomi_miatoll-kernel) to get started with your kernel repository.

## Secrets
- `GIT_TOKEN` - Your GitHub token. Refer to [THIS LINK](https://docs.github.com/en/github/authenticating-to-github/creating-a-personal-access-token) to create a token.
- `BOT_TOKEN` - Your Telegram bot token. Refer to [THIS LINK](https://core.telegram.org/bots#6-botfather) to create a bot.
- `CHAT_ID` - Your Telegram chat ID. 
- `GIT_ID` - Your GitHub username.
- `GIT_EMAIL` - Your GitHub email.

## Usage
- Fork this repository.
- Go to your repository's Settings > Secrets.
- Add the above secrets.
- Go to Actions tab and enable workflows.
- Go to your kernel manifest repository and edit the `default.xml` file according to your assets.
- Go to `workflows/main.yml` and change your `kernel` repository name.
- Trigger the workflow by pushing a commit to your forked `kernel_build` repository and see the magic happen!
