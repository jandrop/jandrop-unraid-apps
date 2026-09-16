# jandrop's Unraid apps

Community Applications templates for the U-Manager family of Unraid plugins.
One XML file per plugin under `plugins/`; `ca_profile.xml` in the root is the
repository entry Community Applications shows.

| Plugin | What it does | Source |
| --- | --- | --- |
| **U-Manager Files** | Native file browser for your shares, with a REST API and a web UI. | [u-manager-files-releases](https://github.com/jandrop/u-manager-files-releases) |
| **U-Manager Companion** | Serves the U-Manager mobile app the Unraid API data upstream ships as a stub. | [u-manager-companion](https://github.com/jandrop/u-manager-companion) |
| **U-Manager Push Notifications** | Sends Unraid notifications to the U-Manager app as push notifications. | [u-manager-unraid-plugin](https://github.com/jandrop/u-manager-unraid-plugin) |

Each plugin is built and released from its own repository. This one only holds
the templates, so a release there needs no change here: the `<PluginURL>` entries
point at `releases/latest`.

Support and feature requests go through the GitHub Issues of the plugin's own
repository, or the [Discord](https://discord.gg/zfwWug8m).

## Adding a plugin

Drop an XML file in `plugins/` with a `<PluginURL>` pointing at the `.plg` in
that plugin's latest release, and a `<TemplateURL>` pointing at the raw URL of
that same file. Check that every URL in it resolves, icon and README included.
