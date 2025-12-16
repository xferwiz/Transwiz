# Transwiz v1.19

Download latest version from Releases:       
https://github.com/transwizmig/Transwiz/releases/tag/v1.19

## Introduction

Transwiz is a technician-oriented Windows user-profile transfer utility built for workstation refreshes, break/fix rebuilds, and side-by-side PC replacements. It captures a complete profile into a standard ZIP-format transfer archive (.trans.zip) and restores it on a target machine while reconfiguring the profile for the destination operating system and account context.

Beyond the GUI wizard, Transwiz supports command-line automation for repeatable migrations: backup/restore switches, explicit source-account selection, archive password protection, logging, and silent/no-prompt/no-reboot behaviors for scripted runs. It can also rename the destination workstation, join it to the required domain, and set the restored account as the default logon—features you can disable via switches when you need strict change control.

For advanced operators, treat Transwiz as a controlled “user state” capture/restore step: validate profile size, pre-clean temp/browser caches, and stage transfer files on resilient storage with predictable throughput. After restore, spot-check profile ACLs, mapped resources, and line-of-business apps that bind to machine identity. Be aware of crypto-bound data: EFS-encrypted files generally can’t be migrated with their encryption keys, so decrypt sensitive folders before capture and re-encrypt after restore.

Operationally, it’s lightweight and reliable: you can often run it from a USB stick or network share using only Transwiz.exe and Transwiz.config, which helps when you’re working in locked-down environments.
