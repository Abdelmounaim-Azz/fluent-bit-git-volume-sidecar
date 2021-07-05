# fluent-bit-git-repo-volume-sidecar
we use a Git repository to store container files
and create a pod containing a sidecar container and a gitRepo volume(The volume will clone
this Git repository which has the container file) . Every time
the pod is created, it pulls the latest version of the container file we want to ship and starts outputting it to its standard output so that it can be picked up by fluent-bit agent.
