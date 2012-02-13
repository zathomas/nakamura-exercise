Nakamura Exercise
=================
This repository is just a simple starting point for creating new bundles for Sakai OAE.

The most common dependencies for working with OSGi and Sling servlets are annotated in the `pom.xml` file.

We inherit certain version numbers and scopes for the essential dependencies from the parent pom.

Assuming you have nakamura running on your local machine on port 8080, you may take advantage of our `redeploy` profile to install your bundle into the running server at the end of the build process. Like this:

    cd sample-bundle
    mvn -Predeploy clean install

Being able to redeploy to a running server shortens the build-run-test loop during development.