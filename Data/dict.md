## Data Dictionary


**AllTopics.csv**

`id` - Topic ID number - for use in Product Hunt API requests

`name` - Topic name / 'slug'

`description` - Topic description

`num_followers` - Total number of followers (as of 11-29-2016)

`num_posts` - Total number of posts (as of 11-29-2016) (note that many products are posted to more than one topic)

----

**PostsForAnalysis.csv**

Columns 1 through 12 are:

`id` - Post ID number

`date` - Date in Month / Day / Year

`day` - 7 days of week: Sunday through Saturday

`created_at` - Date / Time in Year-Month-DayT00:00:00.000-8:00

`time_of_day` - 4 times of day: Morning, Afternoon, Evening, Night (all times in America / Los_Angeles timezone)

`name` - Post name

`tagline` - Post / product tagline

`thumbnail_type` - 4 thumbnail formats: Image, Video, Audio, Book Preview

`product_state` - 3 states: Default, Pre\_launch, or No\_Longer\_Online

`comments_count` - Number of comments made on the post

`num_makers` - Number of makers of the product (0 denotes the maker is either not on Product Hunt or hasn't been tagged to the product)

`num_topics` - Number of topics in which the post was tagged

Columns 13 - 313 are all possible topics a post could be tagged within the timeframe of the data:

`TRUE` denotes the post was tagged in that topic

`No data` indicates FALSE; the post was not tagged in that topic

Columns 314 and 315 are:

`user_id` - the ID number of the user who posted the post

`votes_count` - total number of votes for the post


----

**UsersForAnalysis.csv**

`id` - User ID number

`created_at` - Date / Time in Year-Month-DayT00:00:00.000-8:00

`name` - The user's name

`username` - The user's Product Hunt handle

`headline` - User headline - typically Title and Company but can be anything or nothing at all

`twitter_username` - User's Twitter handle (in the case they signed up via Twitter)

`website_url` - User's website

`collections_count` - Total number of collections for this user

`followed_topics_count` - Total number of topics this user follows

`followers_count` - Number of followers this user has

`followings_count` - Number of Hunters this user follows

`maker_of_count` - Number of products this user has made

`posts_count` - Number of products this user has hunted

`votes_count` - Number of votes this user has submitted