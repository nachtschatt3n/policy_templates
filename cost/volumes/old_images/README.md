## Discover Old Images Policy Template

### What it does

This Policy Template will create a list old images in the cloud account. The age of images to list is provided in the *Number of days old image to delete* parameter.

### Input Parameters

This policy has the following input parameters required when launching the policy.

- *Email addresses* - A list of email addresses to notify
- *Number of days old image to delete* - if a image is older than this parameter it will be added to list
- *Images Tag List* - list of tags that a image can have to exclude it from the list.

### Policy Actions

The following policy actions are taken on any resources found to be out of compliance.

- Delete any old images on approval
- Send an email report

### Required Permissions

This policy requires permissions to access RightScale resources (clouds, volumes, volume_images and tags).  Before applying this policy add the following roles to the user applying the policy.  The roles should be applied to all Accounts where the policy will run or the Organization. For more information on modifying roles visit the [Governance Docs](https://docs.rightscale.com/cm/ref/user_roles.html)

- Cloud Management - `Observer`, `Actor`

### Supported Clouds

- AWS
- Azure
- Google

### Cost

This Policy Template does not launch any instances, and so does not incur any cloud costs.
