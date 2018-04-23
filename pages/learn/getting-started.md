---
title: Get started with {{ $device.name }} and {{ $language.name }}

layout: getting-started.html

dynamic:
  variables: [ $device, $language ]
  ref: $original_ref/$device/$language
  $switch_text: Get started with $device and $language
---

# {{ title }}

## Introduction

{{import "introduction"}}

## What you will need

{{import "whatYouNeed"}}

## Need help?

{{import "usingSupport"}}

## Account setup

If you don't already have a {{ $names.company.lower }} account, make sure to [sign up][link-to-signup].

{{import "sshKey/add"}}

## Create an application

{{import "createAnApp"}}

{{import "getOS"}}

{{import "selectNetworkConfig"}}

{{import "flashingOsToBootMedia"}}

## Provision your device
{{import "getDeviceOnDash"}}

## Deploy code

{{import "deployingCode"}}

## Next steps

- Learn more about the [Dockerfile][dockerfile] that is used to build your application.
- Build an application that uses [multiple containers][multicontainer].
- Get to know the [web terminal][terminal], which can be used to SSH into your application containers and the host OS.
- Try out [local mode][local-mode], the most efficient way to rapidly develop and test your {{ $names.company.lower }} application.

## Example projects

These example projects will give you an idea of more things that can be done with {{ $names.company.lower }}:

{{import "exampleProjects"}}



**Enjoy Resinifying All the Things!**
<img src="/img/common/resinify.jpg" width="80%">

[dockerfile]:/learn/develop/dockerfile
[terminal]:/learn/manage/ssh-access
[local-mode]:/learn/develop/local-mode
[multicontainer]:/learn/develop/multicontainer
[link-to-signup]:https://dashboard.{{ $names.domain }}/signup
