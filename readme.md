# Common SD2IEC Bugs

## Purpose

This repository serves as a **neutral, vendor-agnostic collection of common bugs** found in SD2IEC firmware and its derivatives. 

The goal is **not** to criticize any specific fork, developer, or hardware variant. Instead, it aims to:

- **Document** recurring issues that affect multiple forks.
- **Help users** understand why certain behaviors occur and how to avoid or work around them.
- **Assist developers** in identifying and fixing shared problems across the ecosystem.

This list is **not** a bug tracker for any specific fork. It is a reference document for the entire SD2IEC family.


## Inclusion Criteria

A bug is considered **"common"** and will be added to this list if **at least one** of the following conditions is met:

1. **The bug is present in the official upstream firmware** (sd2iec.de).  
   In this case, it is assumed that most forks derived from upstream are also affected, unless explicitly patched.

2. **The bug is present in at least three independent forks** that are *sufficiently different* from each other (see below).

If neither condition applies, the bug is considered **fork-specific** and does not belong in this list—even if it is severe.


## Fork Independence and "Sufficiently Different"

To prevent artificial inflation of the list through trivial clones, the following guidelines apply when counting forks:

A fork is considered **sufficiently different** if it meets at least one of these criteria:

- It supports different hardware (e.g., PETsd+, LCD-equipped variants).
- It contains significant code changes beyond cosmetic modifications (e.g., new fastloaders, hardware-specific I/O, custom filesystem layers).
- It has been actively maintained by an independent developer for a reasonable period of time.

> ⚠️ **Note:** The assessment of what qualifies as "sufficiently different" involves a degree of **editorial discretion**.  
> This is intentional: it prevents the list from being diluted by trivial forks that only change version strings or minor constants.  
> The maintainers of this list reserve the right to make this judgment on a case-by-case basis.

This policy ensures that the list remains focused on issues that genuinely affect a broad segment of the SD2IEC ecosystem.


## What This List Is Not

- **Not a bug tracker:** Please do not file pull requests asking to fix these bugs here. This is a *documentation* repository.
- **Not a complaint channel:** This list is not intended to shame any developer or project. It is a neutral fact-finding document.
- **Not exhaustive:** The list may not cover every known issue. Contributions that meet the inclusion criteria are welcome.


## Contributing

If you are aware of a common bug that is not yet listed:

1. Open an issue or pull request with:
   - A clear description of the bug.
   - Steps to reproduce it.
   - The expected vs. actual behavior.
   - Which forks are affected (and why they qualify as "sufficiently different").

2. The maintainers will review the submission against the inclusion criteria and decide on acceptance.

Please keep contributions **neutral and factual**. Avoid naming individual developers or making value judgments about forks.


## License

This documentation is provided under the terms of the [Creative Commons Zero (CC0) license](https://creativecommons.org/publicdomain/zero/1.0/).  
You are free to use, share, and adapt it without restriction.
