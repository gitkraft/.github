# 👋 Welcome to GitKraft

GitKraft is a platform for distributing **software as source code** on GitHub, uniquely designed to empower end-users to **easily manage and retain custom, source-level modifications** of the software.

With GitKraft's **GitHub extensions**, users can create **private forks** of software, **customize its source code**, and **update** the software to the latest vendor or community release—all **without losing customizations**.

## Why Choose GitKraft?

Large organizations often need to **adapt the source code** of vendor or community software to meet specific requirements while keeping up with the latest updates. However, GitHub has a notable limitation: a fork of a public repository must also be public, as private forks of public repositories are not supported. GitKraft bridges this gap by enabling the creation of **private forks for public repositories**.

While GitHub allows private forks when the source repository is private (with the option to later make the source repo public), this approach introduces a significant security flaw. Users from other organizations can access commits from private repositories within the same fork network, even including commits from deleted private repositories. Truffle Security has highlighted this issue[^Truffle], which poses a severe risk of exposing confidential information. GitKraft's private forks address this problem, ensuring your data remains **secure** and **isolated**.

In addition to secure forks, GitKraft offers a modern and efficient solution for **managing source-code patches**, overcoming challenges associated with traditional approaches. Current patch management methods often obscure the change history, complicating code reviews and collaboration. Some common problems include:

- **`.patch` files in Git repositories**: Storing customizations as `.patch` files feels like using one version control system inside another, making it difficult to understand changes.
- **Merge**: Merging upstream changes into a private branch buries customizations within the branch's history, making it hard to distinguish between official releases and custom modifications.
- **Rebase**: Rebasing a patch branch over upstream changes disrupts workflows for developers who have already checked out the branch, leading to errors when running `git pull`.

To address these challenges, GitKraft introduces a novel approach to patch management with a new operation called **weld merge**. This operation preserves a transparent history of changes, simplifying audits and fostering effective collaboration.

In summary, GitKraft accelerates development and update cycles, enables rapid vulnerability fixes, and maintains clear audit trails. These features empower open-source collaboration, reduce reliance on permanent forks, and streamline contributions back to the community.

## GitKraft for Open Source

A prime example of software distributed as source code is **Helm charts**, commonly used to configure services on the Kubernetes platform. End-users often need to customize Helm templates at the source level, highlighting the need for robust patch management solutions like GitKraft. To benefit the public, GitKraft will distribute popular open-source Helm charts on its platform. This initiative is currently in progress. Stay tuned for updates.

## Stay in Touch

**[⭐ Star this project](https://github.com/gitkraft/gitkraft)**. Highly recommended, starred users may receive support priority over regular users.

**[📲 Follow me on LinkedIn](https://www.linkedin.com/in/akorzy)**. Don't miss out on updates.

**[▶️ Watch a demo](https://www.youtube.com/watch?v=G8VT_YaDY5U)**. See it in action.

**[✉️ Send me a free message on LinkedIn](https://www.linkedin.com/in/akorzy)**. If you're interested in this project, tell me what you need! I promise – no chatbot!

[^Truffle]: [Anyone can Access Deleted and Private Repository Data on GitHub](https://trufflesecurity.com/blog/anyone-can-access-deleted-and-private-repo-data-github), Truffle Security, July 24, 2024
