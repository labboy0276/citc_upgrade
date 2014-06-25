CITC Upgrade Module
============

This was the module I used to make CITC go from the old Hotsauce to the new Hotsauce

The only thing I had to do manually was move the FPP's, but I gues syou could featurize them in the future

Instructions
------------

1. drush en citc_upgrade
2. drush updb
3. drush dis hot_core hot_pics hot_theme hot_magic hot_widgets hot_admin hot_users hot_pages hot_search hot_wysiwyg -y
4. Run 2xs = drush pm-uninstall hot_core hot_pics hot_theme hot_magic hot_widgets hot_admin hot_users hot_pages hot_search hot_wysiwyg -y
5. drush cc all
6. Delete old Hotsuace profile
7. copy in new hotsuace profile (i pulled in the github copy and ran this command in a seperate test site - drush make --yes profiles/hotsauce/drupal-org.make --no-core --contrib-destination=profiles/hotsauce)
8. drush en panopoly_core panopoly_images panopoly_theme panopoly_magic panopoly_widgets panopoly_admin panopoly_users panopoly_pages panopoly_search panopoly_wysiwyg -y
9. drush rr
