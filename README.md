# site-status
 
Manage permissions for the [k8s cluster](https://github.com/Fairbanks-io/flux-gitops-apps) as Code

## Repo Usage

#### Deployments

- `status`: Should new releases be allowed to deploy?
    - `enabled`: Deployments are allowed to proceed
    - `disable`: Deployments are NOT permitted at this time
- `reason`: If **status** is set too `disabled`, the `reason` will be shown when deployments are blocked
- `admins`: Array of Github usernames who are allowed to bypass these restrictions