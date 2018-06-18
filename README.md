# desc-package-template

[cookiecutter](https://cookiecutter.readthedocs.org/en/latest/) template for DESC Python packages.

### Usage:
```
cookiecutter https://github.com/LSSTDESC/desc_package_template
```

After creating your repository, `cd` into it and do
```
git init
git add .
git commit -m "initial commit"
```
It is now ready for [pushing to GitHub](https://help.github.com/articles/create-a-repo/) and connecting to [Travis CI](https://travis-ci.org/).

You'll want to check that the package is set up the way you want it by browsing the files that `cookiecutter` made. Here are some things to watch out for:

* The LICENSE file adopts the BSD license recommended by the CI group, with the following Copyright statement that you might want to edit:
```
Copyright (c) 2018, the {{cookiecutter.repo_name}} contributors on GitHub, https://github.com/LSSTDESC/{{cookiecutter.repo_name}}/graphs/contributors.
All rights reserved.
```

* By default, you get a python `setup` script that works for DM Stack projects. For Level 3 projects that do not depend on the stack, you'll want to bring in your own `setup.py`.

### Repository Access

By default, if you make your repository with LSSTDESC authorship, not everyone in LSSTDESC will be able to see it. You must list the repository under certain teams. To do so, navigate to the *Collaborators* page in Settings, and add the appropriate teams. Unless you know you want to, leave the access levels at "Read".


### Feedback, License etc

`desc_package_template` is maintained (mainly) by Jim Chiang (@jchiang87) and (occasionally) Phil Marshall (@drphilmarshall). If you have comments, suggestions or questions, please [write us an issue](https://github.com/LSSTDESC/desc_package_template/issues).

This is open source software, available for re-use under the modified BSD license.
