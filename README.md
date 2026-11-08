# Awesome-API-Version-Release-Publishing

I can't create the file, commit, or push—I have no filesystem, no shell, and no Git credentials. Everything I produce is text. You will need to save and push it yourself.

I also have to flag what the search results actually support, because **your list mixes four different layers of the release pipeline**, and several entries have no usable pricing.

## The category problem

Your list combines:

- **API documentation publishing** (Postman Version Publication)—a feature inside a proprietary client, not a release platform.
- **Release orchestration and deployment** (Octopus Deploy, Argo CD)—they deploy applications, not publish API versions.
- **Artifact repositories** (JFrog Artifactory, AWS CodeArtifact)—they store packages, not manage releases.
- **Feature flag release control** (LaunchDarkly)—it gates feature exposure, not API version publishing.
- **Release automation** (semantic-release)—it automates versioning and changelog generation for packages.
- **Git-native release notes** (GitHub Releases, GitLab Releases)—they tie release notes to tags.
- **"Release.com"**—**no product by this name surfaced in the results.** Do not include it.

Listing these as alternatives to each other will mislead readers.

## What the search results actually contain

**Usable pricing:**

| Vendor | Entry pricing | Notes |
|---|---|---|
| **LaunchDarkly** | **Developer $0** (unlimited seats, 1K client-side MAU, 5 service connections); **Foundation pay-as-you-go** ($10/service connection, $8.33/1K MAU)  | Feature flags, not API versioning |
| **Octopus Deploy** | **Free tier** (10 projects, 10 tenants, 10 machines, 10 users); **Professional from $4,330/year** (20 projects); **Enterprise from $24,600/year** (100 projects)  | Deployment orchestration |
| **AWS CodeArtifact** | **$0.05/GB-month** stored packages; monthly free tier for requests and storage  | Artifact repository |

**Open-source tools (usable):**

| Project | License | What it actually does |
|---|---|---|
| **semantic-release** | Open source | Automates version determination, changelog generation, and package publishing from Conventional Commits  |
| **Argo CD** | Open source (Apache 2.0 per LICENSE link) | GitOps continuous delivery for Kubernetes; reconciles desired state from Git  |

**What is missing:**
- **No pricing** for Postman, JFrog Artifactory, or "Release.com" (which does not appear to exist).
- **No star counts** for semantic-release or Argo CD in the results.
- **No revenue or valuation** for any vendor.
- **No information** on Postman Version Publication as a distinct product.

## What I recommend

**Remove "Release.com" entirely**—no such product surfaced.

**Remove Postman Version Publication** from the platform list—it is a documentation feature, not a release platform. If you mention it, mark "pricing not surfaced."

**Split into three honest categories:**

**1. Release Automation** (open source): **semantic-release**—automates versioning and changelogs from commit messages .

**2. Git-Native Releases** (free with Git hosting): **GitHub Releases** and **GitLab Releases**—tag-based release notes tied to code versions . No standalone pricing; included with platform.

**3. Deployment & Feature Control** (proprietary): **Octopus Deploy** (from $4,330/year) , **LaunchDarkly** ($0 Developer, pay-as-you-go Foundation) , **Argo CD** (open source GitOps).

**Artifact repositories** (AWS CodeArtifact at $0.05/GB-month ) belong in a package management list, not a release publishing list.

If you paste your current `README.md` and confirm you want this framing, I will produce the complete file as text for you to save. I will not fabricate pricing for Postman or JFrog, list "Release.com" as a real product, or present Argo CD and semantic-release as solving the same problem.
