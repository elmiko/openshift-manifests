# simple template to launch notebooks

This spec file will create a template to launch the radanalytics.io
base-notebook in your project. After adding this to your project you can
quickly spawn notebooks with custom image and passwords.

## instructions

1. `create -f base-notebook.yaml`
1. `oc new-app --template base-notebook -p IMAGE=my/image/uri -p PASSWORD=secret`

If no `IMAGE` or `PASSWORD` is specified, the template will use
`docker.io/radanalyticsio/base-notebook` for the image and will leave the
password empty.
