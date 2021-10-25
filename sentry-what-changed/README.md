# sentry-what-changed


Uses https://github.com/dorny/paths-filter to determine what files were changed in a commit and then creates a GitHub Check
for the commit that corresponds to the type of files that were changed: "only frontend", "only backend", "fullstack"

This is used in sentry + getsentry, and requires a `.github/file-filters.yml` configuration with a `frontend` and `backend` collection. See https://github.com/getsentry/sentry/blob/master/.github/file-filters.yml for an example.
