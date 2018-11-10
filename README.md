# namespace_with_quota
How to set resource quotas per namespace

```
* Note that if the team member is an admin on the cluster they would be able to edit the resource limits.
* The only way to get around that would be to create users and only assign them to certain namespaces.
* Now if you want to view your quota information you do this:

$ kubectl get resourcequota -n myspace
NAME            AGE
compute-quota   52m
object-quota    52m

$ kubectl describe resourcequota compute-quota -n myspace
$ kubectl edit resourcequota compute-quota -n myspace

```

