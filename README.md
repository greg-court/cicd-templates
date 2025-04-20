Replicating the Block: To replicate the "block merge on failure" behavior, you need to configure Branch Protection Rules in GitHub:

- Go to your repository (gh-greg-court/azure-sandbox).
- Navigate to Settings > Branches.
- Find your main branch (or click Add branch protection rule if none exists for main).
- Enable "Require status checks to pass before merging".
- In the search box that appears, type the name of the job from your CI workflow. In your apim-ci.yaml, the job is named Terraform CI (Dev Env). Select this job.
- (Optional but recommended) Enable "Require branches to be up to date before merging".
- Save changes.