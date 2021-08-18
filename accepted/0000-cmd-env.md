# Adding support to source a .env file for environment variables

## Summary

To consume env-cmd (https://www.npmjs.com/package/env-cmd) and activate it via cmd-line-switch -e

## Motivation

To be able to add environment variables to the execution environment via a .env file

## Detailed Explanation

when the user adds the cmd-line-switch -e the .env file is parsed for variables to add to the executiuon enviroment for consumption by scripts and programs launched via npx

## Rationale and Alternatives

I tried executing cmd-env before npx and while the variables seemed available to shell commands they aren't passed to code executed by npx.  I think the npx spawns an execution environment that doesn't include env vars sourced since the shell was started (I'm on a Mac) 

## Implementation

{{Give a high-level overview of implementation requirements and concerns. Be specific about areas of code that need to change, and what their potential effects are. Discuss which repositories and sub-components will be affected, and what its overall code effect might be.}}

{{THIS SECTION IS REQUIRED FOR RATIFICATION -- you can skip it if you don't know the technical details when first submitting the proposal, but it must be there before it's accepted}}

## Prior Art

see emv-cmd (https://www.npmjs.com/package/env-cmd)

{{Discuss existing examples of this change in other tools, and how they've addressed various concerns discussed above, and what the effect of those decisions has been}}

## Unresolved Questions and Bikeshedding

{{Write about any arbitrary decisions that need to be made (syntax, colors, formatting, minor UX decisions), and any questions for the proposal that have not been answered.}}

{{THIS SECTION SHOULD BE REMOVED BEFORE RATIFICATION}}
