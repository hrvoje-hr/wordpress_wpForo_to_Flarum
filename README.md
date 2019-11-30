# wordpress_wpForo_to_Flarum
Migration Script from Wordpress wpForo to Flarum

Discussion https://discuss.flarum.org/d/1117-phpbb-migrate-script-updated-for-0-3-and-other-improvements

The Script performs a DB -> DB migration of Wordpress users, wpForo posts, wpForo topics and wpForo forums which are transformed into the Flarum tags. It WILL NOT COPY PASSWORDS! Users will be required to reset their passwords.

## Usage Instructions

1. Create a fresh Flarum using the standard install instructions
2. When you create the Flarum make sure the email is different to the original admin in Wordpress otherwise there will be some conflicts
3. Edit wpForo_to_Flarum.php lines 12 - 17 and fill in Database username, database password, Wordpress database name, Flarum database name, Wordpress tables prefix and Flarum database prefix
4. Place wpForo_to_Flarum.php file into the Flarum root directory
5. Run the script simply by visiting your_forum_url/wpForo_to_Flarum.php

## Known issues

1. It will not copy users passwords.
2. In Flarum user profile Posts & Discussions number will be "0" despite all succesfully transfered data. It will be updated to a real number after user's first new post/discussion in Flarum

## Contributions Welcome
Thanks to [all who have contributed on original PHPBB script](https://github.com/robrotheram/phpbb_to_flarum/graphs/contributors) :)
