# Setting up WP-CLI for Local by Flywheel
1. Clone this repo into your project's folder, usually found under ~/Local Sites/<project-name>. `git clone https://github.com/bigwing/local-wp-cli.git wp-cli`
1. Rename folder to `wp-cli`. (Hint: you can skip this step by specifying `wp-cli` as the destination directory when cloning initially.)
1. Open `wp-cli.local.yml` and edit the `<project-url>` and `<user>` fields to match your project.
1. Open `local.php` and edit the `DB_HOST` ip:port to match the project's settings. Local uses the same IP but assigns a new port for each project.
1. Move the `wp-cli.local.yml` up one directory into the root of the project. This lets you run `wp` commands directly from that folder, or any other folder inside the project.
1. Run wp-cli commands from within your active project without having to SSH into the machine first. Try `wp core version --extra` to test.
