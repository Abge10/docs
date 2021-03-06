---
title: 用户帐户仓库的权限级别
intro: 'A repository owned by a user account has two permission levels: the repository owner and collaborators.'
redirect_from:
  - /articles/permission-levels-for-a-user-account-repository
versions:
  free-pro-team: '*'
  enterprise-server: '*'
  github-ae: '*'
---

### About permissions levels for a user account repository

Repositories owned by user accounts have one owner. Ownership permissions can't be shared with another user account.

You can also {% if currentVersion == "free-pro-team@latest" %}invite{% else %}add{% endif %} users on {% data variables.product.product_name %} to your repository as collaborators. For more information, see "[Inviting collaborators to a personal repository](/github/setting-up-and-managing-your-github-user-account/inviting-collaborators-to-a-personal-repository)."

{% tip %}

**Tip:** If you require more granular access to a repository owned by your user account, consider transferring the repository to an organization. 更多信息请参阅“[转让仓库](/github/administering-a-repository/transferring-a-repository#transferring-a-repository-owned-by-your-user-account)”。

{% endtip %}

### Owner access for a repository owned by a user account

仓库所有者对仓库具有完全控制权。 In addition to the actions that any collaborator can perform, the repository owner can perform the following actions.

| 操作                                                                                                                                                                                                                           | 更多信息                                                                                                                                                                                                                                                                          |
|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| {% if currentVersion == "free-pro-team@latest" %}Invite collaborators{% else %}Add collaborators{% endif %}                                                                                                                  |                                                                                                                                                                                                                                                                               |
| "[邀请个人仓库的协作者](/github/setting-up-and-managing-your-github-user-account/inviting-collaborators-to-a-personal-repository)"                                                                                                     |                                                                                                                                                                                                                                                                               |
| Change the visibility of the repository                                                                                                                                                                                      | "[Setting repository visibility](/github/administering-a-repository/setting-repository-visibility)" |{% if currentVersion == "free-pro-team@latest" %}
| Limit interactions with the repository                                                                                                                                                                                       | "[Limiting interactions in your repository](/github/building-a-strong-community/limiting-interactions-in-your-repository)" |{% endif %}
| 合并受保护分支上的拉取请求（即使没有批准审查）                                                                                                                                                                                                      | "[关于受保护分支](/github/administering-a-repository/about-protected-branches)"                                                                                                                                                                                                      |
| 删除仓库                                                                                                                                                                                                                         | "[删除仓库](/github/administering-a-repository/deleting-a-repository)"                                                                                                                                                                                                            |
| Manage the repository's topics                                                                                                                                                                                               | "[Classifying your repository with topics](/github/administering-a-repository/classifying-your-repository-with-topics)" |{% if currentVersion == "free-pro-team@latest" %}
| Manage security and analysis settings for the repository                                                                                                                                                                     | "[Managing security and analysis settings for your repository](/github/administering-a-repository/managing-security-and-analysis-settings-for-your-repository)" |{% endif %}{% if currentVersion == "free-pro-team@latest" %}
| Enable the dependency graph for a private repository                                                                                                                                                                         | "[Exploring the dependencies of a repository](/github/visualizing-repository-data-with-graphs/exploring-the-dependencies-of-a-repository#enabling-and-disabling-the-dependency-graph-for-a-private-repository)" |{% endif %}{% if currentVersion == "free-pro-team@latest" %}
| 删除包                                                                                                                                                                                                                          | "[Deleting a package](/github/managing-packages-with-github-packages/deleting-a-package)" |{% endif %}
| Customize the repository's social media preview                                                                                                                                                                              | "[Customizing your repository's social media preview](/github/administering-a-repository/customizing-your-repositorys-social-media-preview)"                                                                                                                                  |
| Create a template from the repository                                                                                                                                                                                        | "[Creating a template repository](/github/creating-cloning-and-archiving-repositories/creating-a-template-repository)" |{% if currentVersion == "free-pro-team@latest" or enterpriseServerVersions contains currentVersion %}
| Receive                                                                                                                                                                                                                      |                                                                                                                                                                                                                                                                               |
| {% if currentVersion == "free-pro-team@latest" or currentVersion ver_gt "enterprise-server@2.21" %}{% data variables.product.prodname_dependabot_alerts %}{% else %}security alerts{% endif %} for vulnerable dependencies | "[About alerts for vulnerable dependencies](/github/managing-security-vulnerabilities/about-alerts-for-vulnerable-dependencies)" |{% endif %}{% if currentVersion == "free-pro-team@latest" %}
| Dismiss {% data variables.product.prodname_dependabot_alerts %} in the repository                                                                                                                                          | "[查看和更新仓库中的漏洞依赖项](/github/managing-security-vulnerabilities/viewing-and-updating-vulnerable-dependencies-in-your-repository)"                                                                                                                                                 |
| Manage data use for a private repository                                                                                                                                                                                     | "[Managing data use settings for your private repository](/github/understanding-how-github-uses-and-protects-your-data/managing-data-use-settings-for-your-private-repository)"|{% endif %}
| 定义仓库的代码所有者                                                                                                                                                                                                                   | "[关于代码所有者](/github/creating-cloning-and-archiving-repositories/about-code-owners)"                                                                                                                                                                                            |
| Archive the repository                                                                                                                                                                                                       | "[About archiving repositories](/github/creating-cloning-and-archiving-repositories/about-archiving-repositories)" |{% if currentVersion == "free-pro-team@latest" %}
| Create security advisories                                                                                                                                                                                                   | "[关于 {% data variables.product.prodname_security_advisories %}](/github/managing-security-vulnerabilities/about-github-security-advisories)"                                                                                                                                |
| Display a sponsor button                                                                                                                                                                                                     | "[Displaying a sponsor button in your repository](/github/administering-a-repository/displaying-a-sponsor-button-in-your-repository)"                                                                                                                                         |
| Allow or disallow auto-merge for pull requests                                                                                                                                                                               | "[Managing auto-merge for pull requests in your repository](/github/administering-a-repository/managing-auto-merge-for-pull-requests-in-your-repository)" | {% endif %}

### Collaborator access for a repository owned by a user account

Collaborators on a personal repository can pull (read) the contents of the repository and push (write) changes to the repository.

{% note %}

**注：**在私有仓库中，仓库所有者只能为协作者授予写入权限。 协作者不能对用户帐户拥有的仓库具有只读权限。

{% endnote %}

Collaborators can also perform the following actions.

| 操作                                                                                        | 更多信息                                                                                                                                                                                                            |
|:----------------------------------------------------------------------------------------- |:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Fork the repository                                                                       | "[关于复刻](/github/collaborating-with-issues-and-pull-requests/about-forks)"                                                                                                                                       |
| Create, edit, and delete comments on commits, pull requests, and issues in the repository | <ul><li>"[About issues](/github/managing-your-work-on-github/about-issues)"</li><li>"[Commenting on a pull request](/github/collaborating-with-issues-and-pull-requests/commenting-on-a-pull-request)"</li><li>"[Managing disruptive comments](/github/building-a-strong-community/managing-disruptive-comments)"</li></ul>                                                                                                                                                                                       |
| Create, assign, close, and re-open issues in the repository                               | "[Managing your work with issues](/github/managing-your-work-on-github/managing-your-work-with-issues)"                                                                                                         |
| Manage labels for issues and pull requests in the repository                              | "[Labeling issues and pull requests](/github/managing-your-work-on-github/labeling-issues-and-pull-requests)"                                                                                                   |
| Manage milestones for issues and pull requests in the repository                          | "[创建和编辑议题及拉取请求的里程碑](/github/managing-your-work-on-github/creating-and-editing-milestones-for-issues-and-pull-requests)"                                                                                         |
| Mark an issue or pull request in the repository as a duplicate                            | "[About duplicate issues and pull requests](/github/managing-your-work-on-github/about-duplicate-issues-and-pull-requests)"                                                                                     |
| Create, merge, and close pull requests in the repository                                  | "[Proposing changes to your work with pull requests](/github/collaborating-with-issues-and-pull-requests/proposing-changes-to-your-work-with-pull-requests)" |{% if currentVersion == "free-pro-team@latest" %}
| Enable and disable auto-merge for a pull request                                          | "[Automatically merging a pull request](/github/collaborating-with-issues-and-pull-requests/automatically-merging-a-pull-request)"{% endif %}
| Apply suggested changes to pull requests in the repository                                | "[Incorporating feedback in your pull request](/github/collaborating-with-issues-and-pull-requests/incorporating-feedback-in-your-pull-request)"                                                                |
| Create a pull request from a fork of the repository                                       | "[从复刻创建拉取请求](/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request-from-a-fork)"                                                                                                          |
| Submit a review on a pull request that affects the mergeability of the pull request       | "[审查拉取请求中提议的更改](/github/collaborating-with-issues-and-pull-requests/reviewing-proposed-changes-in-a-pull-request)"                                                                                              |
| Create and edit a wiki for the repository                                                 | "[关于 wikis](/github/building-a-strong-community/about-wikis)"                                                                                                                                                   |
| Create and edit releases for the repository                                               | "[Managing releases in a repository](/github/administering-a-repository/managing-releases-in-a-repository)"                                                                                                     |
| Act as a code owner for the repository                                                    | "[About code owners](/articles/about-code-owners)" |{% if currentVersion == "free-pro-team@latest" %}
| Publish, view, or install packages                                                        | "[Publishing and managing packages](/github/managing-packages-with-github-packages/publishing-and-managing-packages)" |{% endif %}
| 作为仓库协作者删除自己                                                                               | "[从协作者的仓库删除您自己](/github/setting-up-and-managing-your-github-user-account/removing-yourself-from-a-collaborators-repository)"                                                                                    |

### 延伸阅读

- "[组织的仓库权限级别](/articles/repository-permission-levels-for-an-organization)"
