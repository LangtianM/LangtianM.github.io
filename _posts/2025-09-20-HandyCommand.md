---
layout: post
title: Handy Command Line Tools
date: 2025-09-20
tags: Tech
categories: Notes
citation: false
---

> Highly recommend Josean Martinez's [blog post](https://www.josean.com/posts/how-to-setup-wezterm-terminal) on how to setup an awesome terminal.

In this post, I’m sharing some handy command-line tools that have really boosted my productivity in day-to-day work. I’ll keep it up to date as I come across new tools that worth a try. Since I use macOS, all the instructions here are for macOS. You may refer to their official documentation for other platforms.

---

# Getting Started: Terminal, Command Line, and Shell

Before diving into the tools, let’s quickly clarify some terminology:

- **Terminal**: The program providing a text-based interface to your computer.  
- **Command Line**: The interface where you type commands.  
- **Shell**: The program that interprets your commands. Typical shells include:
  - **Zsh** (default on macOS)  
  - **PowerShell** (default on Windows)  
  - **Bash** (default on many Linux systems)  

# ShellGPT: Talk to your terminal using English

[ShellGPT](https://github.com/TheR1D/shell_gpt) is an open-sourced lightweight command-line tool powered by large language models. It allows you write commands in **natural language**, and converts them into proper shell commands for you -- it's like you can talk to your terminal using English! With it, you never need to memorize complex commands. It’s also very affordable if you’re just using it to generate commands—I’ve only spent less than 1 dollar over four months of use.

## Installation

On most systems, simply run:

```bash
pip install shell_gpt
```

On Debian-based Linux, where `pip` usage in system environment may be restricted, use `pipx` instead:

```bash
apt install pipx
pipx install shell_gpt
pipx ensurepath
```

## Configuration

Run ShellGPT with any prompt:

```bash
sgpt "what is command line"
```

The first time, it will ask for your OpenAI API key. You can generate one at the [OpenAI API Platform](https://platform.openai.com/api-keys).  

Later, you can update your key by editing the config file:

```bash
sed -i 's/^OPENAI_API_KEY=.*/OPENAI_API_KEY=<your_new_api_key_here>/' ~/.config/shell_gpt/.sgptrc
```

## Example Usage

To generate commands from natural language:

```bash
sgpt --shell "find all .txt files in this folder"
```

You can also install shell integration:

```bash
sgpt --install-integration
```

Then you can directly type in natural language in your terminal and press `Ctrl+l` to convert them into proper shell commands.

---

# Zoxide: Smarter Directory Navigation

[Zoxide](https://github.com/ajeetdsouza/zoxide) is a smarter alternative to `cd`. Instead of typing full paths, Zoxide remembers where you’ve been and lets you jump back with just a keyword.

## Installation

```bash
brew install zoxide
eval "$(zoxide init zsh)"
```

Or, without Homebrew:

```bash
curl -sSfL https://raw.githubusercontent.com/ajeetdsouza/zoxide/main/install.sh | sh
```

## Example Usage

cd into a path once.

```bash
z some/long/path/foo/
```

Zoxide will remember this path and you can go to it anytime by simply typing:

```bash
z foo
```

Want to completely replace `cd` with Zoxide? Just run:

```bash
zoxide init --cmd cd
```