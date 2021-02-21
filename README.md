Why not GitHub?
===============

Copied from the original page: <https://sanctum.geek.nz/why-not-github.html>

[Tom Ryder](https://sanctum.geek.nz/), 27 Oct 2017\
Last updated 12 October 2019

I host all my own code on my [cgit
instance](https://sanctum.geek.nz/cgit/). I do have [an account on
GitHub](https://github.com/tejr), but only because it's a requirement to
contribute to certain projects and even to log into some websites. I
avoid using the account where possible, and I don't host code on it
anymore since June 2016.
The primary reason I host code on my own domain is a practical one: I
can retain control over its location via URI redirects if it needs to
move, including redirects to another site if necessary.
However, I also dislike the tacit acceptance of GitHub as the dominant
free software hosting platform for a decentralised version control
protocol, when it is itself centralised, proprietary, for-profit,
closed-source, and politically active. These things make it vulnerable
to the same issues and abuse that affected
[SourceForge](https://arstechnica.com/information-technology/2015/05/sourceforge-grabs-gimp-for-windows-account-wraps-installer-in-bundle-pushing-adware/).
I feel that the free software and open source communities turn a blind
eye to this massive liability.
Regardless of your position on individual cases, the fact that so much
controversy results from any censorship activity from GitHub should be
considered a warning sign that too much depends on their service. Some
examples:
-   [https://github.com/opal/opal/issues/941](https://web.archive.org/web/20151208143727/https://github.com/opal/opal/issues/941)
    \[archive\]
-   <https://www.theregister.co.uk/2013/12/19/feminist_software_foundation_c_plus_equality/>
-   <https://www.techdirt.com/articles/20150802/20330431831/github-nukes-repository-over-use-word-retard.shtml>
The issue here is not political correctness, it's centralisation. If
GitHub were not in this monopolistic position, nobody would care so much
about any of the above. The overwhelming monopoly that GitHub has as a
code host is a problem that the free software community chooses to
ignore.
Rules of acquisition
--------------------
GitHub has investors who do not care a whit for free software
principles, and eventually [the company *will* get
acquired](https://www.bloomberg.com/news/articles/2018-06-03/microsoft-is-said-to-have-agreed-to-acquire-coding-site-github)—maybe
tomorrow, maybe next year—and as we all know, [money changes
everything](https://www.youtube.com/watch?v=zLWbp3w2eqM).
Don't leave your project's nerve center—its primary address, its means
of contribution, its issue tracker, its website, its primary
documentation, its continuous integration, everything—in a way you
can't redirect!—at the mercy of people who merely want a return on
their investment, and do not care about the principles of a minority of
angry nerds.
Using Git does not require GitHub!
----------------------------------
If you are managing a free software project, *please do not host it on
GitHub*, or at least allow a method of contributing that does not depend
on using it or any other proprietary code hosting platform:
 Formatting and sending patches: 
:   Use [git-send-email(1)](https://git-scm.com/docs/git-send-email).
    The manual page even has instructions for using it with Gmail. Using
    this method, you don't need to host the code at all.
 Pull requests: 
:   Host your own repositories—[it's really
    easy](https://git-scm.com/book/no-nb/v1/Git-on-the-Server-The-Protocols#The-HTTP/S-Protocol)—and
    point maintainers to them with
    [git-request-pull(1)](https://git-scm.com/docs/git-request-pull).
 Web frontend: 
:   Use the superb [cgit](https://git.zx2c4.com/cgit/about/), or
    [gitweb(1)](https://git-scm.com/docs/gitweb), which is included in
    the Git source. Both are straightforward to configure for any
    CGI-capable webserver.
Other options include a [self-hosted
GitLab](https://about.gitlab.com/install/),
[Gogs](https://gogs.io/docs/installation),
[Gerrit](https://www.gerritcodereview.com/), or
[Gitea](https://gitea.io/) instance. More ambitious or puritan sysadmins
might choose to self-host Drew DeVault's stellar
[sr.ht](https://meta.sr.ht/) system, which implements a much wider range
of GitHub's features, for an "integrated development hosting"
environment.
There are some more good reasons not to use GitHub or its ilk discussed
here:
-   <https://miroslaw-zalewski.eu/blog/2015/why-i-dont-use-github-exclusively/>
-   <https://www.adamhyde.net/another-good-reason-not-to-use-github/>
-   <https://www.mirbsd.org/permalinks/wlog-10_e20170301-tg.htm>
-   <https://www.gnu.org/software/repo-criteria-evaluation.html#GitHub>
-   <https://github.com/torvalds/linux/pull/17#issuecomment-5654674>
-   <https://www.wired.com/2015/06/problem-putting-worlds-code-github/>
-   <https://valdyas.org/fading/kde/why-arent-you-using-github/>
Update—June 2018
------------------
Since this page was published, [Microsoft has acquired
GitHub](https://news.microsoft.com/2018/06/04/microsoft-to-acquire-github-for-7-5-billion/),
and there's been a small exodus to third-party hosting on GitLab,
proving as a community we still aren't really learning our lesson about
third-party code hosting. That said, at least the core software for
GitLab is open source, so it's a marginal improvement, but we could be
doing so much better.
If you're reading this because you're angry about the acquisition and
pondering a move to GitLab, I advise you instead to take the plunge and
self-host your code repositories, even if you use the resource-hungry
GitLab to do it. It is not as hard as you think, and once done, this
problem will never bite you again.
Update—July 2019—1/2
------------------------
[Dave Lane explains in
detail](https://davelane.nz/microsoft-there-way-win-our-trust) why the
"Microsoft Loves Linux" slogan is so empty.
Update—July 2019—2/2
------------------------
[GitHub is
blocking](https://www.zdnet.com/article/github-starts-blocking-developers-in-countries-facing-us-trade-sanctions/)
users from Crimea, Iran, and other places. For developers dependent on
it as a service for their projects, this has been crippling, in yet
another vindication for the decentralized design of Git that GitHub and
other third-party hosting sites have so callously butchered.
Update—September 2019
-----------------------
Hello, [visitors from
lobste.rs](https://lobste.rs/s/s0s8fu/why_not_github)! Thank you for
your discussion and critique. I've added mention of the
excellent-looking Gogs, Gerritt, and Gitea, and adjusted some wording
for accuracy and clarity.
To emphasise: nothing in this essay is intended as praise or criticism
specifically of social justice, advocacy for protected groups,
censorship, United States foreign policy, or its [effect on GitHub
specifically](https://help.github.com/en/articles/github-and-trade-controls)—they
have to follow the law, like anyone else. The focus here is on
centralisation onto a commercial service, running proprietary code,
subject to the laws of a single country, that already has a monopoly on
code hosting for free and open source software, and the free software
community's wilfully ignoring the issues therewith.
Update—October 2019—1/2
---------------------------
The [GitHub section of the GNU Ethical Repository
Criteria](https://www.gnu.org/software/repo-criteria-evaluation.html#GitHub)
now links to this page. Thank you, GNU!
Update—October 2019—2/2
---------------------------
It's become more widely known that [GitHub had a contract with United
States Immigrations and Customs Enforcement
(ICE)](https://www.theverge.com/2019/10/9/20906213/github-ice-microsoft-software-email-contract-immigration-nonprofit-donation),
an ethical hot-topic at present after [similar disputes with config
management software
Chef](https://techcrunch.com/2019/09/20/chef-ceo-says-hell-continue-to-work-with-ice-in-spite-of-protests/).
Again, the issue here is not whether this is good or bad, it's that
you're handing GitHub power over your work, while they may be using
their proprietary software to political ends that you find repugnant,
and refusing you the right to fork and apply their code in the way that
suits you, the user. Avoiding these sorts of problems is the entire
basis of [Freedom 0](https://www.gnu.org/philosophy/free-sw.en.html).



### Hi there 👋

<!--
**iCopyleft/iCopyleft** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
