# gitlab_issue_crawler

This repo can search gitlab issue comments by git grep!

* gitlab has no API to search issue comments
  * [Add Search option for Issues that User has commented on \(\#28268\) · Issues · GitLab\.org / GitLab · GitLab]( https://gitlab.com/gitlab-org/gitlab/issues/28268 )
  * [Ability to search issue comments \(not just original post\) \(\#28028\) · Issues · GitLab\.org / GitLab FOSS · GitLab]( https://gitlab.com/gitlab-org/gitlab-foss/issues/28028 )
  * [search in issue titles only \(\#25046\) · Issues · GitLab\.org / GitLab · GitLab]( https://gitlab.com/gitlab-org/gitlab/issues/25046 )
  * [Search / filter issues does not search issue comments \(\#15645\) · Issues · GitLab\.org / GitLab · GitLab]( https://gitlab.com/gitlab-org/gitlab/issues/15645 )

## how to use
```
# check project id
GITLAB_PRIVATE_TOKEN="xxx" GITLAB_URL="http://xxx:1234" gitlab_issue_crawler

# download project all issue (only comments)
GITLAB_PRIVATE_TOKEN="xxx" GITLAB_URL="http://xxx:1234" gitlab_issue_crawler <project_id>
```

```
git add <project_id> # dir
git grep 'keyword'
```

## TODO
* add function to download description

