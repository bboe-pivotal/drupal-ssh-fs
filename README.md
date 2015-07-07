# Drupal, configured to run on Cloud Foundry using MySQL and SSH-FS service
See [deploy.sh](deploy.sh) for info on how to deploy this demo.

The following customizations have been made to Drupal in order for it to run on Cloud Foundry:
* [.bp-config folder](drupal-7.38/.bp-config) for configuring the PHP buildpack.
* [settings.php](drupal-7.38/sites/default/settings.php) for making Drupal connect to connect to MySQL provided by Cloud Foundry.
* [mount.sh](drupal-7.38/.profile.d/mount.sh) for customizing folder structure for SSH-FS and setting up a temp directory.
