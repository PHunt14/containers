# Documentation

## Introduction

This is a container image for building node applications.  This has a few tools installed to facilitate development.

Base image: node:lts-alpine
Tools:
- yq
- jq
- git
- mandocs
- bashcompletion
- curl

## Use

docker run -it node-dev