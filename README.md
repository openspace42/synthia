# bash-framework

## How to configure

It's extremely simple:

* 1\. Start your new project by cloning this repo.
* 2\. Edit and customize your `functions` file:
    * 2.1\. Define your variables below the `Insert your variables here` line.
    * 2.2\. Insert your global project-related functions below the `Insert project functions here` line.
    * 2.3\. Add your previously defined functions below the `Add your install-time functions here` line to have those executed during the install.
* 3\. Edit and customize your `restore` file:
    * 3.1\. Add your restore script arguments below the `Read any project-specific restore script arguments` line.
    * 3.2\. Edit the settings below the `Specify your restore-time settings here` line to fit your restore needs.

## Examples

* 2.1\.

```
proj_name="hello-world"
short_name="hw"
author_name="openspace42"
```

Set `skip_install_time_backup` to `y` if your project stores no data on end users' machines that could go lost during a re-install or update

Set `backup_ref_dir` to the directory that has the most impactful size when performing a backup [such as `/var/www/` for nginx-related projects]

## How to install the end project

```bash
bash <proj_name>/setup
```

## Live examples:

[aenigma](https://github.com/openspace42/aenigma)

[raptor](https://github.com/openspace42/raptor)
