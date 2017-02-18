# check_gitlab

Nagios/Icinga check for a GitLab server

GitLab provides a URL/token for retreiving health information. That URL can be found at `/admin/health_check` on a GitLab instance with admin access.
Pass that url as an argument to `check_gitlab` to check if it's returning 'success', which indicates a successful helth check.

This avoids having to use the `gitlab-ctl` cli tool on a remote host.
