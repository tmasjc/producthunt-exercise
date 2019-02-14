## 数据字典


#### AllTopics.csv

	id - 主题ID - 用于 Product Hunt API 请求
	
	name - 主题名称
	
	description - 主题描述
	
	num_followers - 粉丝总数（截至 2016-11-29）
	
	num_posts - 帖子总数（截至 2016-11-11）- 请注意，许多产品会被发布到多个主题下


#### PostsForAnalysis.csv

列 1 - 14 为帖子的相关属性变量：

	id - Post ID 
	
	date - Date (yyyy-mm-dd)
	
	day - 7 days of week: Sunday through Saturday
	
	created_at - 帖子发布时间
	
	time_of_day - 发布时间: Morning, Afternoon, Evening, Night (all times in America / Los_Angeles timezone)
	
	name - 发布标题
	
	tagline - 帖子/产品简述
	
	thumbnail_type - 种预览格式: 图片, 视频, 音频, 书籍
	
	product_state - 产品现状: Default (默认), Pre\_launch (未发布), or No\_Longer\_Online (已下线)
	
	comments_count - 在帖子上发表的评论数量
	
	num_makers - 产品开发者数量（0表示开发者非 Product Hunt 用户，或者未标记产品）
	
	num_topics - 帖子被标记的主题数量
	
	user_id - 发布帖子的用户ID
	
	votes_count - 该帖子的总投票数



#### UsersForAnalysis.csv

	id - User ID
	
	created_at - Date/Time in Year-Month-DayT00:00:00.000-8:00
	
	name - 用户真实名
	
	username - 用户小名
	
	headline - 用户个性标题
	
	twitter_username - 用户的推特账号
	
	website_url - 用户个人网站
	
	collections_count - 用户收藏数量
	
	followed_topics_count - 用户关注的主题数量
	
	followers_count - 用户拥有的关注者的数量
	
	followings_count - 用户关注其他用户的数量
	
	maker_of_count - 产品开发数量
	
	posts_count - 帖子/产品发布数量
	
	votes_count - 提交的投票数量
	
	
#### PostsTopicsForAnalysis.csv

各个帖子对应的主题: `TRUE` 表示帖子被标记了该主题, 空值代表帖子没有被标记在该主题中.