# site-status
 
Manage permissions for the [k8s cluster](https://github.com/Fairbanks-io/flux-gitops-apps) as Code

## Setup

Create the folder structure `.github/workflows` and place the included [site-status.yaml](site-status.yaml) file in the directory.

## Repo Usage

#### Deployments

- `status`: Should new releases be allowed to deploy?
    - `enabled`: Deployments are allowed to proceed
    - `disabled`: Deployments are NOT permitted at this time
- `reason`: If **status** is set to `disabled` the `reason` will be shown when deployments are blocked
- `admins`: Array of Github usernames who are allowed to bypass these restrictions