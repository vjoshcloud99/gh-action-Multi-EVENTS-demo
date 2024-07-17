### 💡   Notes About Forked Repo User Vs. Collaborators

> :white_check_mark: Collaborators are those user which are  <ins>TRUSTED</ins> by original repository owner, While  forked repository user is <ins>UNTRUSTED</ins>.

> :white_check_mark: If your repository is forked by another user and when they submit the pull request for original user, it don't trigger a WF ( Work-Flow ) run. <br> Since they need to be approved by the original user first and then only it will trigger the WF.

> :white_check_mark: Instead of above fork repository UseCase, if you have **Collaborator** ( A User which is TRUSTED by Original Repo Owner Once Approved ) then, <br> if he opens the ( PR ) Pull Request for same repo for which he is approved collaborator then It will certainly Trigger WF for it.

> :white_check_mark:  To add a collaborator  navigate to ropository > settings > collaborator > Add collaborator., which sends mail to intended collaborator ,<br> once he accepts the invitation his / her name displays in collaborators list.

> :white_check_mark: if  you push the code  to repo and suddenly you realised  that  it consist of error then you can cancel the workflow by clicking  Cancel Workflow <br> button inside . It will help to save budge and time for execution of  a workflow.

> :white_check_mark:  By default , workflows gets cancelled if job fails or at lease one step of a job fails, or you can cancel it manually.

###  <a href= "https://docs.github.com/en/actions/managing-workflow-runs/skipping-workflow-runs" target="_blank">Skipping workflow runs</a>

> :white_check_mark: If you just  added comments to repo files,  and if you wish to cancel tiggering workflows for such thing, because running workflows <br> for such commits is worthless, So to save budget and time for such workflows then while making a commit use below syntax 
 ``` $ git commit  -m " Added comments for Readme.md file [skip ci] ```

 You can follow other syntax as well given in below link <br><a href= "https://docs.github.com/en/actions/managing-workflow-runs/skipping-workflow-runs" target="_blank">Skipping workflow runs</a>

> :white_check_mark:  Skipping Wrokflow works only for  ``` on: push or on: pull_request ```