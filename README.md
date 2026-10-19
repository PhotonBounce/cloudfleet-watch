# cloudfleet-watch

A free 5-minute health check for a private Colab worker fleet, run by GitHub Actions on this public repo
(public repos get free Actions minutes). The repo holds only this workflow. The checker code and all data
live in a private repository, which the workflow reads with a repository secret, and the job prints nothing.

Needs one secret, `QUEUE_TOKEN`: a fine-grained personal access token limited to the private fleet repository
with **Contents: Read and write**.
