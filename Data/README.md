## Data Dictionary


**AllTopics.csv**

`id` - 主题ID - 用于 Product Hunt API 请求

`name` - 主题名称

`description` - 主题描述

`num_followers` - 粉丝总数（截至 2016-11-29）

`num_posts` - 帖子总数（截至 2016-11-11）- 请注意，许多产品会被发布到多个主题下

----

**PostsForAnalysis.csv**

> 列 1 - 12 为帖子的相关属性变量：

`id` - Post ID 

`date` - Date (yyyy-mm-dd)

`day` - 7 days of week: Sunday through Saturday

`created_at` - 帖子发布时间

`time_of_day` - 4 times of day: Morning, Afternoon, Evening, Night (all times in America / Los_Angeles timezone)

`name` - Post name

`tagline` - 帖子/产品简述

`thumbnail_type` - 4 种预览格式 : 图片, 视频, 音频, 书籍

`product_state` - 3 states: Default, Pre\_launch, or No\_Longer\_Online

`comments_count` - 在帖子上发表的评论数量

`num_makers` - 产品开发者数量（ 0 表示开发者非 Product Hunt 用户，或者未标记产品）

`num_topics` - 帖子被标记的主题数量

> 列 13 - 313 为帖子在相应时间范围内可以标注的所有可能的主题：

`TRUE` 表示帖子被标记了该主题

`No data` 帖子没有被标记在该主题中

> 列 314 - 315：

`user_id` - 发布帖子的用户ID

`votes_count` - 该帖子的总投票数


----

**UsersForAnalysis.csv**

`id` - User ID

`created_at` - Date / Time in Year-Month-DayT00:00:00.000-8:00

`name` - The user's name

`username` - The user's Product Hunt handle

`headline` - User headline - typically Title and Company but can be anything or nothing at all

`twitter_username` - User's Twitter handle (in the case they signed up via Twitter)

`website_url` - User's website

`collections_count` - 用户收藏数量

`followed_topics_count` - 用户关注的主题数量

`followers_count` - 用户拥有的关注者数量

`followings_count` - 用户关注的其他用户数量

`maker_of_count` - 产品开发数量

`posts_count` - 帖子/产品发布数量

`votes_count` - 提交的投票数量