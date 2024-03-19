---
title: Create a pull request in Visual Studio
titleSuffix: ""
description: Create a pull request in Visual Studio by using GitHub or Azure DevOps.
ms.date: 10/23/2023
ms.topic: how-to
author: houghj16
ms.author: jehoughton
ms.manager: mijacobs

ms.subservice: general-ide
---
# Create a pull request in Visual Studio 

If you’re authenticated to GitHub or Azure DevOps and have pushed changes to your remote repository, you can create a pull request without leaving Visual Studio. Pull requests are an essential tool in GitHub and Azure DevOps for code review.  These reviews help catch issues in new features and allow teammates to share their experience with different regions of the codebase – improving the health of the codebase overall.  

> [!NOTE]
> To try out the feature, ensure it’s enabled in **Tools** > **Options** > **Environment** > **Preview Features** > **Pull Request**

To create a pull request, follow these steps:

1. Before you can create a pull request, you need to [create a new branch](git-create-branch.md) for your changes. This branch keeps your modifications separate from the main branch until they’re ready to be merged.

1. Then, you can [commit](git-make-commit.md) and [push](git-push-remote.md) your changes as you normally would in the Git Changes window.

1. Select the link in the notification banner to **Create in Visual Studio** or **Create in Browser**.

   :::image type="content" source="media/vs-2022/git-create-pull-request-infobar-two-links.png" alt-text="Screenshot of the Git Changes window with the infobar 'Successfully pushed QP to origin. Pull request: Create in Visual Studio or create in browser.' in Visual Studio 2022.":::
   
   Alternatively, you can create a pull request from a remote branch by navigating to the **New Pull Request** window via the top-level menu **Git** > **GitHub** or **Azure DevOps** > **New Pull Request**. Or right-click a branch in the Git Repository Window.
   
   :::image type="content" source="media/vs-2022/git-create-pr-top-level-menu.png" alt-text="The Git top level menu with GitHub selected and 'New Pull Request' text highlighted in Visual Studio 2022."::: 

   Or right select a branch in the Git Repository Window to open the context menu and select **New Pull Request**.

   :::image type="content" source="media/vs-2022/git-create-pr-git-repository-branch-context-menu.png" alt-text="The Git Repository window with the outgoing / incoming link text highlighted in Visual Studio 2022."::: 

1. Select the branch that you want to merge into and give your pull request a descriptive title and description. 

   > [!TIP]
   > You can use [markdown syntax](https://www.markdownguide.org/) to format your pull request description from Visual Studio. Try it out by typing the markdown symbols in the **Description** box and preview your markdown by selecting the **Preview** button.

   :::image type="content" source="media/vs-2022/git-create-pr-markdown.png" alt-text="The New Pull Request window with the preview button text highlighted in Visual Studio 2022."::: 

1. The difference preview allows you to see all the changes in the files that have been committed as a part of your pull request. See [Compare files - diff view](../ide/compare-with.md).

   > [!TIP]
   > The summary difference view option allows you to review only the changed sections of code. 

   :::image type="content" source="media/vs-2022/git-create-pr-summary-diff.png" alt-text="The New Pull Request window with the summary button text highlighted in Visual Studio 2022."::: 

1. You can link work items by referencing them with the [issue search](https://devblogs.microsoft.com/visualstudio/reference-github-issues-and-pull-requests-in-visual-studio/), by typing `#` in the description box or pressing the **#** button in the lower right corner. You can also add your reviewers by typing their GitHub username or Azure DevOps identity or email. 

   :::image type="content" source="media/vs-2022/git-create-pr-issue-search.png" alt-text="The New Pull Request with # in the description box and a list of the related GitHub issues and pull requests shown in Visual Studio 2022."::: 

1. Once you’ve clicked **Create** on your pull request, other developers can review your changes and provide feedback.

## Next steps

To continue your journey, visit the [Fetch, pull, and sync in Visual Studio](git-fetch-pull-sync.md) page.

## See also

- [Git experience in Visual Studio](git-with-visual-studio.md)
- [Visual Studio & GitHub: Better together](https://visualstudio.microsoft.com/vs/github/)
