CITC Upgrade Module
============

This was the module I used to make CITC go from the old Hotsauce to the new Hotsauce

The only thing I had to do manually was move the FPP's, but I gues syou could featurize them in the future

Instructions
------------

1. Enable this module
2. drush dis hot_core hot_pics hot_theme hot_magic hot_widgets hot_admin hot_users hot_pages hot_search hot_wysiwyg -y
3. Run 2xs = drush pm-uninstall hot_core hot_pics hot_theme hot_magic hot_widgets hot_admin hot_users hot_pages hot_search hot_wysiwyg -y
4. drush cc all
5. Delete old Hotsuace profile
6. copy in new hotsuace profile (i pulled in the github copy and ran this command in a seperate test site - drush make --yes profiles/hotsauce/drupal-org.make --no-core --contrib-destination=profiles/hotsauce)
7. drush en panopoly_core panopoly_images panopoly_theme panopoly_magic panopoly_widgets panopoly_admin panopoly_users panopoly_pages panopoly_search panopoly_wysiwyg -y
8. drush rr
