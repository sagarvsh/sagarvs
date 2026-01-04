---
template: overrides/main.html
title: Blog
search:
  exclude: true
---

<style>
  .md-sidebar--secondary:not([hidden]) {
    visibility: hidden;
  }
</style>

# Blog

## [The past, present and future]

__2021 was a fantastic year for this project as we shipped many new awesome
features, saw significant user growth to make the
project sustainable.__

<aside class="mdx-author" markdown>
![@sagarvsh][@sagarvsh avatar]

<span>__Sagar V Shankaraiah__ · @sagarvsh</span>
<span>
:octicons-calendar-24: January 1, 2021 ·
:octicons-clock-24: 10 min read
</span>
</aside>

  [@sagarvsh avatar]: https://avatars.githubusercontent.com/u/23294710

---

# Forked Repo for developing your app is not a best practice

***Draft***

In recent days it's found that an increasing number of development teams have started to use forked repo for the development of the parent repo. 
This is **bad development practice** and must be avoided. 

You can fork the repo when you want to freely experiment with changes without affecting the original project or you like to contribute to a different project which you do not belong to. 

If you are part of the development team, you must use a branch, it’s incredibly fast, effective, and easy. Creating a fork will replicate the entire original repository, the fork does not stay synchronized and takes the additional manual effort to keep the forked repo synchronized and merging pull requests are damn slow which will also impact Sedated security scanning. 

All this additional effort will take a toll on GitHub performance, storage, security scanning and most of all developer's agility, efforts and time. 

Pros: 


Cons:

Suggestions:
Good branching practices and a solid understanding of branching methodologies are paramoutn to cohesive, risk-reductive code collaboration between developers. This also reliably scales as the size of the project team does. 

Reference:

I found these three posts to be the best for explaining the Git Branching model - and they even give examples with precise syntax.

https://nvie.com/posts/a-successful-git-branching-model/
https://datasift.github.io/gitflow/IntroducingGitFlow.html?b...
https://www.atlassian.com/git/tutorials/comparing-workflows/...
** The author of the top one is credited with being the creator of the Git branching model so he knows a thing or two about it.
