
# `Software Development`

<br>

___

<br>

Covered in this file:
1. [`Software Development Lifecycle`](#software-development-lifecycle)
1. [`Software Development Stages`](#software-development-stages)
1. [`Software Versioning`](#software-versioning)
    1. [`Version Stages`](#version-stages)
    1. [`Version Numbering`](#version-numbering)
    1. [`Version Labeling`](#version-labeling)
1. [`Patches and Fixes`](#patches-and-fixes)


<br>

___

<br>

# `Software Development Lifecycle`
The `Software Development Lifecycle (SDLC)` is a structured process used to design, develop, test, and maintain software. 
* There are `6 phases` in the software development lifecycle. 

<br>


| **Phase**     | **What Happens** |
|---------------|------------------|
| `1. Plan`   | - Figure out what the software needs to do.<br>- Talk to people who will use it.<br>- Write down the goals and make a plan. |
| `2. Design` | - Decide how the software will work.<br>- Choose the tools and technologies to use.<br>- Plan how everything will fit together. |
| `3. Implement` | - Start writing the code.<br>- Break the work into small tasks.<br>- Build and test small parts as you go. |
| `4. Test`   | - Check the software for bugs.<br>- Make sure it does what it’s supposed to.<br>- Use both automated tools and manual testing. |
| `5. Deploy` | - Put the finished software on the server or app store.<br>- Set it up so users can use it. |
| `6. Maintain` | - Fix bugs that come up.<br>- Make improvements over time.<br>- Keep the software running smoothly. |

<br>

Here is a more in depth description:
| **Phase**     | **Description** |
|---------------|-----------------|
| `1. Plan`   | - Conduct cost-benefit analysis, scheduling, resource estimation, and allocation.<br>- Collect requirements from customers, internal/external experts, and managers.<br>- Create a Software Requirements Specification (SRS) document to:<br>  • Set expectation<br>  • Define common goals<br>  • Support project planning<br>- Estimate costs and create a detailed schedule and plan. |
| `2. Design` | - Analyze requirements to identify optimal solutions.<br>- Consider:<br>  • Technology choices<br>  • Pre-existing module integration<br>  • Development tools<br>  • IT infrastructure compatibility |
| `3. Implement` | - Convert requirements into working code.<br>- Break down work into smaller daily coding tasks.<br>- Development team writes and tests code. |
| `4. Test`   | - Use automated and manual testing to find bugs.<br>- Verify the software meets customer requirements.<br>- Testing often occurs in parallel with development. |
| `5. Deploy` | - Move the code from the build/test environment to the production environment.<br>- Tasks include:<br>  • Packaging<br>  • Environment configuration<br>  • Installation |
| `6. Maintain` | - Fix bugs, resolve issues, and manage updates.<br>- Monitor:<br>  • System performance<br>  • Security<br>  • User experience<br>- Continuously improve the software. |



<br>

[Back To Top](#software-development)

___

<br>

# `Software Development Stages`
`Software development stages` refer to the different environments and checkpoints that code passes through from initial development to being used by real users. Each stage has a specific purpose to ensure the software is stable, functional, and ready for release.

<br>

| **Stage**                     | **Description** |
|------------------------------|-----------------|
| `1. Development (Dev)`     | - Developers write and test initial code.<br>- Work on new features, bug fixes, and changes. |
| `2. Integration`           | - Combine code from multiple developers.<br>- Use Continuous Integration (CI) tools for automation and validation. |
| `3. Quality Assurance (QA) / Testing` | - Perform multiple testing types:<br>  • Unit testing<br>  • Integration testing<br>  • System testing<br>  • User Acceptance Testing (UAT) |
| `4. Staging / Pre-Production` | - Environment simulates production.<br>- Final step before release.<br>- Used for end-to-end testing and validation. |
| `5. User Acceptance Testing (UAT)` | - Conducted with real users or stakeholders.<br>- Confirms software meets business requirements. |
| `6. Production`            | - Live environment used by end-users.<br>- Code is fully deployed after passing all previous stages. |
| `7. Post-Production / Monitoring` | - Monitor the live environment for issues.<br>- Includes:<br>  • Performance monitoring<br>  • Logging<br>  • Incident handling |
| `8. Maintenance`           | - Apply regular updates, patches, and enhancements.<br>- Continuously maintain and improve the software. |
| `9. Rollback`              | - Safety mechanism if deployment causes major issues.<br>- Revert to a stable previous version. |

<br>

[Back To Top](#software-development)

___

<br>

# `Software Versioning`
`Software versioning` is the system used to assign unique numbers or identifiers to specific releases of a software product. 

<br>

## `Version Stages`

| **Stage**                        | **Description** |
|----------------------------------|-----------------|
| `1. Pre-Alpha`                 | - Internal development phase.<br>- Software is still being built—**not ready for testing**.<br>- Often unstable and incomplete. |
| `2. Alpha`                     | - First testing phase, usually **internal only**.<br>- May have major bugs and incomplete features.<br>- Purpose: Test core functionality and catch early issues. |
| `3. Beta`                      | - More stable than Alpha.<br>- Released to a **limited audience** (external testers or public).<br>- Purpose: Find bugs, gather feedback, improve usability.<br>- Features are mostly complete. |
| `4. Release Candidate (RC)`    | - **Almost production-ready**.<br>- Final testing before release.<br>- Labeled like: `v1.0.0-RC1`.<br>- Only released if no major bugs are found. |
| `5. General Availability (GA)` / `Production` | - **Official public release**.<br>- Fully tested, stable, and ready for users.<br>- Labeled like: `v1.0.0`. |

<br>

## `Version Numbering`
`Version numbering` is a system used to label different releases of a software product. 

<br>

`Semantic Versioning` is a version numbering system that uses a three-part format: `MAJOR.MINOR.PATCH` to clearly communicate the type and impact of changes in a software release.

<br>

```
MAJOR.MINOR.PATCH
```

| **Part**   | **What It Means** | **When It Changes** | **Example** |
|------------|-------------------|---------------------|-------------|
| `MAJOR`  | Breaking changes | When you make changes that `break backward compatibility` | `2.0.0` |
| `MINOR`  | New features | When you `add functionality` in a backward-compatible way | `2.1.0` |
| `PATCH`  | Bug fixes / small tweaks | When you `fix bugs` or make minor changes that don’t affect compatibility | `2.1.1` |

<br>

## `Version Labeling`
`Version labeling` is the practice of adding extra text to a version number to show the status, purpose, or condition of that version. 

| **Label**      | **Meaning**                                       | **Example**            |
|----------------|---------------------------------------------------|------------------------|
| `-alpha`       | Early development/testing stage. Often unstable.  | `1.0.0-alpha.1`        |
| `-beta`        | Feature-complete, but needs external testing.     | `1.0.0-beta.2`         |
| `-rc`          | Release Candidate. Nearly final, pending final testing. | `1.0.0-rc.1`       |
| `-hotfix`      | Emergency fix applied to a live/production system. | `1.0.0-hotfix.1`       |
| `-bugfix`      | Fix for a known issue (sometimes used interchangeably with `patch`). | `1.0.0-bugfix.3` |
| `-patch`       | Minor update or tweak, usually backward compatible. | `1.0.0-patch.2`       |
| `-dev`         | Actively being worked on; unstable development build. | `1.0.0-dev.5`       |
| `-snapshot`    | Snapshot of current development state (often auto-generated). | `1.0.0-snapshot` |


<br>

[Back To Top](#software-development)

___

<br>

# `Patches and Fixes`

| **Term**   | **What It Means** | **When It’s Used** |
|------------|-------------------|---------------------|
| `Bug-Fix` | A fix for a non-critical issue in the code (e.g., something not working as expected). | When minor issues or unexpected behavior are found during testing or after release. |
| `Hotfix`  | An urgent fix for a **critical** issue in a live/production system (e.g., security bug, crash). | When something is broken in production and needs to be fixed immediately. |
| `Patch`   | A general term for small updates that include bug fixes, performance improvements, or tiny features. | Regular maintenance releases that don’t introduce breaking changes. |

<br>

A `changelog` is a documented history of all the changes made to a software project. It typically includes information about new features, bug fixes, enhancements, and any other modifications made between versions. 

<br>

[Back To Top](#software-development)

___

<br>

*Created and maintained by Mr. Merritt*


