.. _permissions:

Facebook and Instagram API Permissions
======================================

This document provides a comprehensive list of all the functions available in the `sage_meta` package, along with the necessary permissions required to use each function with the Facebook and Instagram Graph APIs.

AccountHandler Functions
------------------------

+------------------------------------------+-----------------------------+-------------------------------------------------------------+
| Function                                 | Permissions                 | Description                                                 |
+==========================================+=============================+=============================================================+
| get_accounts                             | pages_show_list             | Fetches the user's Facebook pages.                          |
+------------------------------------------+-----------------------------+-------------------------------------------------------------+
| get_instagram_business_account           | instagram_basic,            | Fetches the Instagram business account linked to a Facebook |
|                                          | instagram_manage_insights   | page.                                                       |
+------------------------------------------+-----------------------------+-------------------------------------------------------------+
| get_account_settings                     | instagram_basic             | Gets the settings of an Instagram account.                  |
+------------------------------------------+-----------------------------+-------------------------------------------------------------+

HashtagHandler Functions
------------------------

+------------------------------------------+-----------------------------+-------------------------------------------------------------+
| Function                                 | Permissions                 | Description                                                 |
+==========================================+=============================+=============================================================+
| search_hashtag                           | instagram_basic             | Searches for a hashtag.                                     |
+------------------------------------------+-----------------------------+-------------------------------------------------------------+
| get_hashtag_info                         | instagram_basic             | Gets information about a hashtag.                           |
+------------------------------------------+-----------------------------+-------------------------------------------------------------+
| get_recent_media                         | instagram_basic             | Gets recent media for a given hashtag.                      |
+------------------------------------------+-----------------------------+-------------------------------------------------------------+
| get_top_media                            | instagram_basic             | Gets top media for a given hashtag.                         |
+------------------------------------------+-----------------------------+-------------------------------------------------------------+

MediaHandler Functions
----------------------

+------------------------------------------+-----------------------------+-------------------------------------------------------------+
| Function                                 | Permissions                 | Description                                                 |
+==========================================+=============================+=============================================================+
| get_instagram_media                      | instagram_basic             | Fetches media items for a given Instagram account ID.       |
+------------------------------------------+-----------------------------+-------------------------------------------------------------+
| get_instagram_insights                   | instagram_manage_insights   | Fetches insights for Instagram media.                       |
+------------------------------------------+-----------------------------+-------------------------------------------------------------+

CommentHandler Functions
------------------------

+------------------------------------------+-----------------------------+-------------------------------------------------------------+
| Function                                 | Permissions                 | Description                                                 |
+==========================================+=============================+=============================================================+
| get_instagram_comments                   | instagram_manage_comments   | Fetches comments for Instagram media.                       |
+------------------------------------------+-----------------------------+-------------------------------------------------------------+
| get_post_mentions                        | instagram_manage_comments   | Fetches data about media posts where the IG user is         |
|                                          |                             | mentioned in the caption.                                   |
+------------------------------------------+-----------------------------+-------------------------------------------------------------+
| get_comment_mentions                     | instagram_manage_comments   | Gets data about comments in which the account has been      |
|                                          |                             | mentioned.                                                  |
+------------------------------------------+-----------------------------+-------------------------------------------------------------+
| reply_to_mention                         | instagram_manage_comments   | Replies to a comment or media object caption that the       |
|                                          |                             | account has been mentioned in.                              |
+------------------------------------------+-----------------------------+-------------------------------------------------------------+

StoryHandler Functions
----------------------

+------------------------------------------+-----------------------------+-------------------------------------------------------------+
| Function                                 | Permissions                 | Description                                                 |
+==========================================+=============================+=============================================================+
| get_instagram_stories                    | instagram_basic             | Fetches stories for a given Instagram account ID.           |
+------------------------------------------+-----------------------------+-------------------------------------------------------------+

ContentPublishing Functions
---------------------------

+------------------------------------------+-----------------------------+-------------------------------------------------------------+
| Function                                 | Permissions                 | Description                                                 |
+==========================================+=============================+=============================================================+
| publish_photo                            | instagram_content_publish   | Publishes a photo to Instagram.                             |
+------------------------------------------+-----------------------------+-------------------------------------------------------------+
| publish_video                            | instagram_content_publish   | Publishes a video to Instagram.                             |
+------------------------------------------+-----------------------------+-------------------------------------------------------------+
| publish_carousel                         | instagram_content_publish   | Publishes a carousel to Instagram.                          |
+------------------------------------------+-----------------------------+-------------------------------------------------------------+
| publish_story                            | instagram_content_publish   | Publishes a story to Instagram.                             |
+------------------------------------------+-----------------------------+-------------------------------------------------------------+
| get_media_status                         | instagram_basic             | Gets the status of a media item.                            |
+------------------------------------------+-----------------------------+-------------------------------------------------------------+
| put_comment                              | instagram_manage_comments   | Posts a comment to a post.                                  |
+------------------------------------------+-----------------------------+-------------------------------------------------------------+
| reply_to_comment                         | instagram_manage_comments   | Replies to a comment.                                       |
+------------------------------------------+-----------------------------+-------------------------------------------------------------+

CopyrightManager Functions
--------------------------

+------------------------------------------+-----------------------------+-------------------------------------------------------------+
| Function                                 | Permissions                 | Description                                                 |
+==========================================+=============================+=============================================================+
| check_copyright_status_unpublished       | instagram_basic             | Checks the copyright status of an unpublished video.        |
+------------------------------------------+-----------------------------+-------------------------------------------------------------+
| check_copyright_status_published         | instagram_basic             | Checks the copyright status of a published video.           |
+------------------------------------------+-----------------------------+-------------------------------------------------------------+

InstagramProductTagging Functions
---------------------------------

+------------------------------------------+-----------------------------+-------------------------------------------------------------+
| Function                                 | Permissions                 | Description                                                 |
+==========================================+=============================+=============================================================+
| create_tagged_container                  | instagram_basic,            | Creates a tagged media container.                           |
|                                          | instagram_shopping_tag      |                                                             |
+------------------------------------------+-----------------------------+-------------------------------------------------------------+
| publish_media                            | instagram_content_publish   | Publishes a media container.                                |
+------------------------------------------+-----------------------------+-------------------------------------------------------------+
| get_product_tags                         | instagram_basic             | Gets product tags of a media.                               |
+------------------------------------------+-----------------------------+-------------------------------------------------------------+
| delete_product_tags                      | instagram_manage_comments   | Deletes product tags of a media.                            |
+------------------------------------------+-----------------------------+-------------------------------------------------------------+
| update_product_tags                      | instagram_manage_comments   | Updates product tags of a media.                            |
+------------------------------------------+-----------------------------+-------------------------------------------------------------+
| get_catalogs                             | instagram_basic             | Gets available catalogs for an Instagram user.              |
+------------------------------------------+-----------------------------+-------------------------------------------------------------+
| get_eligible_products                    | instagram_basic             | Gets eligible products from a catalog.                      |
+------------------------------------------+-----------------------------+-------------------------------------------------------------+
| create_catalog                           | business_management         | Creates a new product catalog.                              |
+------------------------------------------+-----------------------------+-------------------------------------------------------------+
