# 介绍Meteor的相关项目

### Respondly - Social conversations

Respondly helps companies manage conversations with customers from a single, simple team inbox. It was launched by two developers — Tim Haines and Phil Cockfield. Phil has spoken at HTML5DevConf and Meteor Devshop about UI Harness, their scheme for modular, reusable UI components in Meteor. Respondly recently recruited Harrison Harnisch from Apple and are actively hiring more Meteor software engineers.

### Verso - Classroom tools
Verso is used commercially by thousands of schools to deliver flipped classroom content, analyze student progress, and measure teacher performance. It was built by Percolate Studio, a leading Meteor consulting shop, who used a three person team to build iOS and Android apps in just a few months. Read their popular Case Study on building Verso for their recommendations on mobile Meteor development.

### Workpop - Job marketplace
Workpop was founded in Los Angeles by former Zynga GM Reed Shaffner and Viddy cofounder Chris Ovitz. It’s a job marketplace that modernizes the process of hiring for hourly workers. Workpop has been featured in TechCrunch, Fox News, and the Wall Street Journal, and the company has raised a $7.9 million Series A led by Trinity Ventures. You can read about how Meteor benefits Workpop in the recruiting section of their website and in this blog post by Trinity partner Dan Scholnick.

### Classcraft - Classroom gamification
Classcraft has been featured by BBC, Fast Company, and VentureBeat and is used by over 18,000 teachers. The premium version comes with a native iOS app, which uses Jesse Bounds\' open-source Objective-DDP library to connect to the Meteor server over DDP. Classcraft is building an open-source Android DDP client library and hiring people to join their remote-friendly team of fifteen.

### Blonk - Mobile job search
Blonk is a mobile job search app built by a single developer. Box, BitTorrent, Lyft and other companies use it to help surface promising job candidates, who can swipe through job openings and tap “yes” if they’re interested in chatting. Blonk charges companies for job listings. It runs on both iOS and Android.

### Lookback - UX studies
Lookback is a startup founded in Sweden by ex-Spotify engineers Joachim Bengtsson and Jonatan Littke. Their service is used by thousands of companies to record user experiences and hunt down bugs on mobile apps, with Spotify, King.com, Yammer, and Venmo among their customers. Lookback has been featured in TechCrunch and The Next Web.

Respondly被Stripe和Slack等公司使用，用来管理团队的twitter对话，这是一个协作型app，
特色功能是是每个使用它的人都可以看到对方的实时动向，我们可以筛选这些tweets，并且看到每个人的
tweet。Respondly完全使用Meteor打造。

Verso是纯Javascript跨平台移动应用，为老师和学生提供服务。在这个App中，教师们
创建Clips，课程以视频，图片或文字形式给出。Verso使用Meteor和PhoneGap开发。
所以老师可以在App中使用摄像头和麦克风。学生使用app发表反馈。老师可以查看
学生的总体统计。驱动移动应用的Codebase同时提供了一个Web端的全校统计。

Workpop是一个洛杉矶的初创企业，使用Meteor构建了一个小时工的网上人才市场，它们获得
了多家知名风投的风险投资。求职者可以使用这个app来寻找和申请适合它们技能和时间的职位。
Workpop 可以自动保存你的工作时间和其他工作信息。招聘者有一个专属页面对求职者进行统一查看。

Classcraft是一个角色扮演类游戏，老师们用它来帮助学生提高课堂注意力。
这里是从Web浏览器端老师看到的界面，每个学生都对应有一个虚拟角色，
如果学生做了正确的事，教师可以给学生经验值奖励。老师们也可以设定游戏规则，
并且设定不同学生的职业。这个App使用Meteor和MongoDB搭建。
Classcraft同样有一个原生iOS应用。学生们使用它来控制自己的角色。
这个iOS App，通过DDP连接到Meteor的后端，用来同步数据。

Blonk是一个轻量级工作匹配App，作为一个求职者，你可以快速的浏览招聘信息，
点击Yes和No来反馈你的意向。招聘公司也做同样的事，如果你们都点了Yes，
那么会出现一个聊天室，你们可以在聊天室里详谈。Blonk使用Meteor和PhoneGap
打造，有iOS和Android两个版本。

Lookback是一个iOS可适用性测试应用，进行beta tests，包含了使用流程的同步视频与评论。
Lookback由两部分组成，一个iOS开发者插件，一个Meteor App，用来收集和记录所有的
用户体验，Lookback被包括Spotify等公司使用。