---
slug: 003-GPG-101-How-to-get-your-first-GPG-Keys
title: How to Get Your First GPG Keys
date: 2023-04-22T21:55:27.154Z
excerpt: How to customize what you're seeing here and make it your own.
coverImage: docs/media/HEADER/GitHub-Repo-SecureGitGuide-ART-001.jpg
tags:
  - Documentation
---

<script>
  import CodeBlock from "$lib/components/molecules/CodeBlock.svelte";
</script>

# GPG - 101 - How to get your first GPG Keys

## Installing GPG

The steps to install GPG on your computer are the following:

1. Download the necessary software for your Operating System at:
   - [Windows](https://gpg4win.org/download.html)
   - [Linux - Installed through terminal](https://linuxhint.com/gpg-command-ubuntu/)
   - [Mac OS](https://sourceforge.net/p/gpgosx/docu/Download/)

## GPG4Win Kleopatra

### Generating your own new GPG Keys

---

Generating your own new GPG Keys is extremely easy.
Here is a series of screenshots of the process using the Kleopatra application for Windows.

(1)

![001](docs/media/003/KLEO_CREATE_001.png)

(2)

![002](docs/media/003/KLEO_CREATE_002.png)

**It is extremely important to use a passphrase and more important if you use it to actually write it down somewhere so that you never loose it.**

(3)

![003](docs/media/003/KLEO_CREATE_003.png)

(4)

![004](docs/media/003/KLEO_CREATE_004.png)

(5)

![005](docs/media/003/KLEO_CREATE_005.png)

(6)

![006](docs/media/003/KLEO_CREATE_006.png)

(7)

![007](docs/media/003/KLEO_CREATE_007.png)

(8)

![008](docs/media/003/KLEO_CREATE_008.png)

(9)

![009](docs/media/003/KLEO_CREATE_009.png)

(10)

![010](docs/media/003/KLEO_CREATE_010.png)

(11)

![011](docs/media/003/KLEO_CREATE_011.png)

### Creating a Revocation Certificate

---

(1)

![012](docs/media/003/KLEO_CREATE_012.png)

(2)

![013](docs/media/003/KLEO_CREATE_013.png)

(3)

![014](docs/media/003/KLEO_CREATE_014.png)

(4)

![015](docs/media/003/KLEO_CREATE_015.png)

### Sample Public GPG Key

---

![016](docs/media/003/KLEO_CREATE_016.png)

## Command Line or Terminal

In order to generate your new keys you have two options:

- Running the default setup.
- Running the full setup which lets you define some additional specifications such as the encryption level.

### Default Setup

---

Open the command line as an admin and type:

<CodeBlock>
    ```terminal
    gpg --gen-keys
    ```
</CodeBlock>
(1)

![cli001](docs/media/003/CLI_CREATE_001.png)

(2)

![cli002](docs/media/003/CLI_CREATE_002.png)

(3)

![cli003](docs/media/003/CLI_CREATE_003.png)

(4)

![cli004](docs/media/003/CLI_CREATE_004.png)

(5)

![cli005](docs/media/003/CLI_CREATE_005.png)

(6)

![cli006](docs/media/003/CLI_CREATE_006.png)

Once this has been done the keys get generated with the default encryption level of 3072.

### Full Setup

---

This option lets you:

- Define the encryption level up to 4096.
- Insert a comment.
- Define the key type (RSA, DSA, Elgamal, etc.).

It automatically generates also a revocation certificate at the default location which is indicated at the final step.

Open the command line as an admin and type:

<CodeBlock>
    ```terminal
    gpg --full-generate-keys
    ```
</CodeBlock>

#### Defining the key type

(1)

![cliFgk001](docs/media/003/CLI_CREATE_fgk_001.png)

(2)

![cliFgk002](docs/media/003/CLI_CREATE_fgk_002.png)

#### Defining the encryption level

(3)

![cliFgk003](docs/media/003/CLI_CREATE_fgk_003.png)

(4)

![cliFgk004](docs/media/003/CLI_CREATE_fgk_004.png)

#### Defining the expiration date

(5)

![cliFgk005](docs/media/003/CLI_CREATE_fgk_005.png)

(6)

![cliFgk006](docs/media/003/CLI_CREATE_fgk_006.png)

(7)

![cliFgk007](docs/media/003/CLI_CREATE_fgk_007.png)

#### Defining the user ID to identify the key

(8)

![cliFgk008](docs/media/003/CLI_CREATE_fgk_008.png)

(9)

![cliFgk009](docs/media/003/CLI_CREATE_fgk_009.png)

(10)

![cliFgk010](docs/media/003/CLI_CREATE_fgk_010.png)

(11)

![cliFgk011](docs/media/003/CLI_CREATE_fgk_011.png)

#### Final screen with revocation certificate location

(12)

![cliFgk012](docs/media/003/CLI_CREATE_fgk_012.png)

[Back to home](./)
