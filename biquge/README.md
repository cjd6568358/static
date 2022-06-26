# biquge
笔趣阁APP 网页版

### 校验用户名是否可用
POST https://user.pigqq.com/BookAction.aspx HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
Content-Type: application/x-www-form-urlencoded
Content-Length: 41
Host: user.pigqq.com
Connection: Keep-Alive
Accept-Encoding: gzip

action=checkusername&username=17730354264

{"status":1,"info":"用户名可用","data":{"result":"0"}}

### 注册
POST https://user.pigqq.com/Register.aspx HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
Content-Type: application/x-www-form-urlencoded
Content-Length: 326
Host: user.pigqq.com
Connection: Keep-Alive
Accept-Encoding: gzip

extinfo=plateform%3Dandroid%23sex%3D1%23pak%3Dcom.biquge.ebook.app%23appname%3D%E7%AC%94%E8%B6%A3%E9%98%81%23versionName%3D8.0.20200710%23osver%3D11%23device%3D9b54bc6314734939da7663c4c8e28155%23brand%3DXiaomi%23model%3DM2102J2SC&password=123456&repassword=123456&action=newuser&email=17730354264%40189.cn&username=17730354264

{"status":1,"info":"success","data":{"UserInfo":{"UserName":"17730354264","VipLevel":0,"IsNoAd":false,"IsFirstLogin":false,"ExtInfo":"plateform=android#sex=1#pak=com.biquge.ebook.app#appname=笔趣阁#versionName=8.0.20200710#osver=11#device=9b54bc6314734939da7663c4c8e28155#brand=Xiaomi#model=M2102J2SC","Balance":0.0,"Coin":0,"Integral":0,"KingPower":false,"NeedChanagePwd":false},"Message":"注册成功","Status":1}}

### 找回密码
POST https://user.pigqq.com/ModifyUser.aspx HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
cookie: ASP.NET_SessionId=jfwqbjvat4i1wt2m2ovi2yqa; ; m_uid=521f1f09-44ba-4b46-9e79-1161e18e4c92; expires=Fri, 22-Oct-2021 15:26:05 GMT; member_username=17730354264;
Content-Type: application/x-www-form-urlencoded
Content-Length: 81
Host: user.pigqq.com
Connection: Keep-Alive
Accept-Encoding: gzip

password=123456&action=forwardpwd&email=17730354264%40189.cn&username=17730354264

{"status":1,"info":"success","data":{"UserInfo":{"UserName":"17730354264","VipLevel":0,"IsNoAd":false,"IsFirstLogin":false,"Balance":0.0,"Coin":0,"Integral":0,"KingPower":false,"NeedChanagePwd":false},"Message":"密码修改成功","Status":1}}
### 登录
POST https://user.pigqq.com/Login.aspx HTTP/1.1
password=123456&usecookie=43200&action=login&username=13512341234

{"status":1,"info":"success","data":{"UserInfo":{"UserName":"17712522763","Email":"cjd6568358@163.com","VipLevel":0,"IsNoAd":false,"IsFirstLogin":false,"ExtInfo":"plateform=android#sex=1#pak=com.biquge.ebook.app#appname=笔趣阁#versionName=8.0.20200710#osver=11#device=c3cc42bd20d3ed228255cf79c6aad504#brand=Xiaomi#model=M2102J2SC","Balance":0.00,"Coin":0,"Integral":0,"KingPower":false,"NeedChanagePwd":false},"Message":"用户登录成功","Status":1}}
需要保存cookie

### 书单
POST https://userxs.pigqq.com/Bookshelf.aspx HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
cookie: ASP.NET_SessionId=3tm5cppasezlyax4pf3c1q4y; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 12:25:54 GMT; member_username=17712522763;
Content-Type: application/x-www-form-urlencoded

{"status":1,"info":"success","data":[{"ChapterId":3697892,"ChapterName":"第758章 誓言","NewChapterCount":37,"PostTime":null,"Playsources":null,"Id":598066,"Name":"旧日之箓","Area":null,"AreaCodde":"","Author":"熊狼狗","Img":"jiurizhilu.jpg","HostKey":"","Desc":null,"BookStatus":null,"LastChapterId":3709232,"LastChapter":"第795章 发展和地震","CName":null,"HitCount":null,"CollectCount":null,"CommendCount":null,"UpdateTimeForChapterContent":null,"UpdateTime":"2021-09-20 00:09","FirstChapterId":null,"Score":null},{"ChapterId":3245152,"ChapterName":"583 弯道超车","NewChapterCount":17,"PostTime":null,"Playsources":null,"Id":559500,"Name":"我真不想读档","Area":null,"AreaCodde":"","Author":"一文倒","Img":"wozhenbuxiangdudang.jpg","HostKey":"","Desc":null,"BookStatus":null,"LastChapterId":3245932,"LastChapter":"600 阿姨的模式太多了","CName":null,"HitCount":null,"CollectCount":null,"CommendCount":null,"UpdateTimeForChapterContent":null,"UpdateTime":"2021-09-20 22:17","FirstChapterId":null,"Score":null},{"ChapterId":3449606,"ChapterName":"第二百七十一章 吊在树上的人","NewChapterCount":430,"PostTime":null,"Playsources":null,"Id":610529,"Name":"从红月开始","Area":null,"AreaCodde":"","Author":"黑山老鬼","Img":"conghongyuekaishi.jpg","HostKey":"","Desc":null,"BookStatus":null,"LastChapterId":3535058,"LastChapter":"第七百零一章 单兵的层次","CName":null,"HitCount":null,"CollectCount":null,"CommendCount":null,"UpdateTimeForChapterContent":null,"UpdateTime":"2021-09-21 21:00","FirstChapterId":null,"Score":null}]}

### initconf 未知
GET https://scxs.pigqq.com/prov8/base/initconf.html HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
Content-Type: application/x-www-form-urlencoded
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Host: scxs.pigqq.com
Connection: Keep-Alive
Accept-Encoding: gzip

### 上传进度 action=bookcaselimit 确认上传限制
POST https://userxs.pigqq.com/BookAction.aspx HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Content-Type: application/x-www-form-urlencoded
Content-Length: 20
Host: userxs.pigqq.com
Connection: Keep-Alive
Accept-Encoding: gzip

action=bookcaselimit

{"status":1,"info":"success","data":{"isclose":false,"canupload":true,"alreadyuse":3,"caselimit":100}}

### 上传进度 实际上传
POST https://userxs.pigqq.com/BookAction.aspx HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Content-Type: application/x-www-form-urlencoded
Content-Length: 141
Host: userxs.pigqq.com
Connection: Keep-Alive
Accept-Encoding: gzip

chapterid=3245932&chaptername=600%20%E9%98%BF%E5%A7%A8%E7%9A%84%E6%A8%A1%E5%BC%8F%E5%A4%AA%E5%A4%9A%E4%BA%86&action=addbookmark&bookid=559500

{"status":1,"info":"加入书签成功！","data":{"result": "1"}}

### 下载进度
POST https://userxs.pigqq.com/Bookshelf.aspx HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Content-Type: application/x-www-form-urlencoded
Content-Length: 8
Host: userxs.pigqq.com
Connection: Keep-Alive
Accept-Encoding: gzip

cache=no


{"status":1,"info":"success","data":[{"ChapterId":3709232,"ChapterName":"第795章 发展和地震","NewChapterCount":0,"PostTime":null,"Playsources":null,"Id":598066,"Name":"旧日之箓","Area":null,"AreaCodde":"","Author":"熊狼狗","Img":"jiurizhilu.jpg","HostKey":"","Desc":null,"BookStatus":null,"LastChapterId":3709232,"LastChapter":"第795章 发展和地震","CName":null,"HitCount":null,"CollectCount":null,"CommendCount":null,"UpdateTimeForChapterContent":null,"UpdateTime":"2021-09-20 00:09","FirstChapterId":null,"Score":null},{"ChapterId":3245932,"ChapterName":"600 阿姨的模式太多了","NewChapterCount":0,"PostTime":null,"Playsources":null,"Id":559500,"Name":"我真不想读档","Area":null,"AreaCodde":"","Author":"一文倒","Img":"wozhenbuxiangdudang.jpg","HostKey":"","Desc":null,"BookStatus":null,"LastChapterId":3245932,"LastChapter":"600 阿姨的模式太多了","CName":null,"HitCount":null,"CollectCount":null,"CommendCount":null,"UpdateTimeForChapterContent":null,"UpdateTime":"2021-09-20 22:17","FirstChapterId":null,"Score":null},{"ChapterId":3449606,"ChapterName":"第二百七十一章 吊在树上的人","NewChapterCount":430,"PostTime":null,"Playsources":null,"Id":610529,"Name":"从红月开始","Area":null,"AreaCodde":"","Author":"黑山老鬼","Img":"conghongyuekaishi.jpg","HostKey":"","Desc":null,"BookStatus":null,"LastChapterId":3535058,"LastChapter":"第七百零一章 单兵的层次","CName":null,"HitCount":null,"CollectCount":null,"CommendCount":null,"UpdateTimeForChapterContent":null,"UpdateTime":"2021-09-21 21:00","FirstChapterId":null,"Score":null}]}

### 小说 banner
GET https://scxs.pigqq.com/prov8/base/banner_man.html HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
Content-Type: application/x-www-form-urlencoded
If-Modified-Since: Wed, 31 Mar 2021 13:12:36 GMT
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Host: scxs.pigqq.com
Connection: Keep-Alive
Accept-Encoding: gzip

{
  "status": 1,
  "info": "",
  "data": [
  {
      "type": "book",
      "param": "576561",
      "imgurl": "https://imgapixs.pysmei.com/shudan/images/576561.jpg"
    },
    {
      "type": "book",
      "param": "610529",
      "imgurl": "https://imgapixs.pysmei.com/shudan/images/610529.jpg"
    },
    {
      "type": "book",
      "param": "615702",
      "imgurl": "https://imgapixs.pysmei.com/shudan/images/615702.jpg"
    }
  ]
}

### 小说书城

GET https://scxs.pigqq.com/prov8/base/man2.html HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
Content-Type: application/x-www-form-urlencoded
If-Modified-Since: Fri, 14 May 2021 16:35:54 GMT
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Host: scxs.pigqq.com
Connection: Keep-Alive
Accept-Encoding: gzip

{
	"status": 1,
	"info": "success",
	"data": [{
		"Category": "热门连载",
		"ChangeFlag": "no",
		"More": "https://scxs.pysmei.com/top/man/top/hot/week/{page}.html",
		"MoreFlag": "api",
		"NavIcon": "hhttps://scmh.pysmei.com/pubimgs/recommend5.png",
		"ViewType": "1r3c3c",
		"Books":  [{
			"Id": 626698,
			"Name": "深空彼岸",
			"Area": null,
			"AreaCodde": "",
			"Author": "辰东",
			"Img": "shenkongbian.jpg",
			"HostKey": "",
			"Desc": "浩瀚的宇宙中，一片星系的生灭，也不过是刹那的斑驳流光。仰望星空，总有种结局已注定的伤感，千百年后你我在哪里？家国，文明火光，地球，都不过是深空中的一粒尘埃。星空一瞬，人间千年。虫鸣一世不过秋，你我一样在争渡。深空尽头到底有什么？",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "玄幻奇幻",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "9.6"
		}, {
			"Id":630009,
"Name":"星门",
"Area":null,
"AreaCodde":"",
"Author":"老鹰吃小鸡",
"Img":"xingmen.jpg",
"HostKey":"",
"Desc":"传说，在那古老的星空深处，伫立着一道血与火侵染的红色之门。\r\n\r\n 传奇与神话，黑暗与光明，无尽传说皆在这古老的门户中流淌。\r\n\r\n 俯瞰星门，热血照耀天地，黑暗终将离去！",
"BookStatus":null,
"LastChapterId":null,
"LastChapter":null,
"CName":"玄幻奇幻",
"HitCount":null,
"CollectCount":null,
"CommendCount":null,
"UpdateTimeForChapterContent":null,
"UpdateTime":null,
"FirstChapterId":null,
"Score":"8.3"
		}, {
			"Id": 625913,
			"Name": "万相之王",
			"Area": null,
			"AreaCodde": "",
			"Author": "天蚕土豆",
			"Img": "wanxiangzhiwang.jpg",
			"HostKey": "",
			"Desc": "天地间，有万相。而我李洛，终将成为这万相之王。",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "玄幻奇幻",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "6.0"
		}, {
			"Id": 623345,
			"Name": "顶级气运，悄悄修炼千年",
			"Area": null,
			"AreaCodde": "",
			"Author": "任我笑",
			"Img": "dingjiqiyun，qiaoqiaoxiulianqiannian.jpg",
			"HostKey": "",
			"Desc": "转世来到修仙世界，韩绝发现自己带着游戏属性，竟然可以摇骰子刷新灵根资质与先天气运。\r\n\r\n 于是乎，他花了十一年摇先天气运。\r\n\r\n 【绝世无双：仙姿，魅力顶级】\r\n\r\n 【天命剑痴：剑道资质顶级，剑道悟性顶级】\r\n\r\n 【身法绝尘：身法资质顶级】\r\n\r\n 【仙帝后裔：获得一部绝世修仙功法、一千块上品灵石】\r\n\r\n 韩绝为了长生，决定悄悄修炼，不出风头。\r\n\r\n 千年后，修真界一代换一代。\r\n\r\n 当仙界清理凡间",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "武侠仙侠",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "7.0"
		}, {
			"Id": 618211,
			"Name": "我的治愈系游戏",
			"Area": null,
			"AreaCodde": "",
			"Author": "我会修空调",
			"Img": "wodezhiyuxiyouxi.jpg",
			"HostKey": "",
			"Desc": "警察同志，如果我说这是一款休闲治愈系游戏，你们信吗？",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "玄幻奇幻",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "9.2"
		}, {
			"Id": 612233,
			"Name": "我不是野人",
			"Area": null,
			"AreaCodde": "",
			"Author": "孑与2",
			"Img": "wobushiyeren.jpg",
			"HostKey": "",
			"Desc": "下一本书的名字已经确定了叫做——《我不是野人》！这一次我们将会回到远古时期，见识一下我们的老祖宗。见识一下被猪脚提醒学会冶炼青铜，最后提着青铜轩辕剑的黄帝把骑着大熊猫手持两柄石斧的恶霸蚩尤打的狼狈逃窜的故事，见识一下炎帝的老奸巨猾，见识一下刑天如何被黄帝砍掉脑袋之后还能战斗的故事。",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "历史军事",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "8.9"
		}, {
			"Id": 521014,
			"Name": "大奉打更人",
			"Area": null,
			"AreaCodde": "",
			"Author": "卖报小郎君",
			"Img": "dafengdagengren.jpg",
			"HostKey": "",
			"Desc": "这个世界，有儒；有道；有佛；有妖；有术士。\r\n\r\n 警校毕业的许七安幽幽醒来，发现自己身处牢狱之中，三日后流放边陲.....\r\n\r\n 他起初的目的只是自保，顺便在这个没有人权的社会里当个富家翁悠闲度日。\r\n\r\n ......\r\n\r\n 多年后，许七安回首前尘，身后是早已逝去的敌人和朋友，以及累累白骨。\r\n\r\n 滚滚长江东逝水，浪花淘尽英雄，是非成败转头空。\r\n\r\n 青山依旧在，几度夕阳红。\r\n\r\n PS：本书不悲",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "武侠仙侠",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "9.1"
		}]
	}, {
		"Category": "抖音热书",
		"ChangeFlag": "no",
		"More": "https://scxs.pysmei.com/top/man/top/collect/week/{page}.html",
		"MoreFlag": "api",
		"NavIcon": "https://scmh.pysmei.com/pubimgs/recommend5.png",
		"ViewType": "3c3c",
		"Books":  [{
			"Id": 626638,
			"Name": "狂龙战尊",
			"Area": null,
			"AreaCodde": "",
			"Author": "凌皓秦雨欣",
			"Img": "kuanglongzhanzun.jpg",
			"HostKey": "",
			"Desc": "西境之王，影门之主，一代战神，凌皓！五年前，养父一家人被人灭门，九死一生的他被秦雨欣救回一条命，尔后被神秘人带走，机缘巧合下进入军营。五年后，一条短信将战神从枪林弹雨的战场召回了红尘俗世，直到这一刻，他才发现自己多了个女儿。自此，蛟龙入海，风起云涌，一代战神化身超级奶爸，护家人，斗豪门，刀光剑影，快意恩仇…",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "都市言情",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "6.0"
		}, {
			"Id": 626637,
			"Name": "镇国战神奶爸",
			"Area": null,
			"AreaCodde": "",
			"Author": "杨凡梁曦月",
			"Img": "zhenguozhanshennaiba.jpg",
			"HostKey": "",
			"Desc": "战神：你女儿是我的，现在你老婆也是我的了，速领离婚证吧！\\n战神归来，发现女儿被贩卖，一怒之下霸道回归！从此称霸都市当起全职奶爸，孩子她妈有点受欢迎，只好被迫各种打脸，专治不服，低调打脸，高调宠娃，顺便撩撩孩子她妈，狠斗丈母娘，走上至尊无上的都市之路！",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "都市言情",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "6.0"
		}, {
			"Id": 626636,
			"Name": "活了万年终于有了老婆孩子",
			"Area": null,
			"AreaCodde": "",
			"Author": "徐长生周葵",
			"Img": "huolewannianzhongyuyoulelaopohaizi.jpg",
			"HostKey": "",
			"Desc": "我是一个跨越了无尽时间长河的长生者，由于某些原因，这么多年我膝下无子，举目无亲……直到这一天，有人告诉我，我有了个女儿。",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "都市言情",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "6.0"
		}, {
			"Id": 626584,
			"Name": "谢邀，人在洪荒，拒绝妖皇",
			"Area": null,
			"AreaCodde": "",
			"Author": "鱼台小龙虾",
			"Img": "xieyao_renzaihonghuang_jujueyaohuang.jpg",
			"HostKey": "",
			"Desc": "穿越洪荒，成为帝俊和东皇太一长兄。\r\n\r\n 深知后世巫妖量阶走向的道尘，当即决定带着两个小老弟，闭关太阳星，打死不踏出一步。\r\n\r\n 自此洪荒天机发生变化，妖族无主，巫族一家独大。\r\n\r\n 圣人一个脑袋两个大。\r\n\r\n 鸿钧：你出关，圣位灵宝随你挑。\r\n\r\n 洪荒大妖：求求你出关吧，巫族太凶了。\r\n\r\n 系统：宿主求求你出关吧，三清和十二祖巫，人头打出狗脑子了。\r\n\r\n 道尘：不存在的，等我再闭个十个八个元会再",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "武侠仙侠",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "6.0"
		}, {
			"Id": 607975,
			"Name": "此刻，我为华夏守护神",
			"Area": null,
			"AreaCodde": "",
			"Author": "风花雪乐",
			"Img": "cike，woweihuaxiashouhushen.jpg",
			"HostKey": "",
			"Desc": "0260年12月24日平安夜，米国旧铜山首现大批海兽，全城人民无一幸存！\r\n\r\n 0261年4月23日，北熊国出现6级海兽，全国沦陷！\r\n\r\n 0262年1月1日，新年第一天，华夏出现10级海兽，代号【饕餮】，华夏沦陷！\r\n\r\n ......\r\n\r\n 0260年1月，华夏战神臣风重生到海兽爆发十一个月前。\r\n\r\n 他赢得高层信任，将在华夏近两万公里的海岸线上铸起一座钢铁长城！\r\n\r\n 外媒惊为：东方奇迹！",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "都市言情",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "8.0"
		}, {
			"Id": 515103,
			"Name": "萧阳龙王殿",
			"Area": null,
			"AreaCodde": "",
			"Author": "萧阳云舒",
			"Img": "xiaoyanglongwangdian.jpg",
			"HostKey": "",
			"Desc": "生而为王，年少父母被杀，他消失数年，成为世界地下世界的超级王者回归都市，这次回来，看他如何改变天下大势，成为王者至尊。",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "都市言情",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "8.0"
		}]
	}, {
		"Category": "高分神作",
		"ChangeFlag": "no",
		"More": "https://scxs.pysmei.com/top/man/top/vote/week/{page}.html",
		"MoreFlag": "api",
		"NavIcon": "https://scmh.pysmei.com/pubimgs/recommend5.png",
		"ViewType": "3c3c",
		"Books": [{
			"Id": 603425,
			"Name": "孙猴子是我师弟",
			"Area": null,
			"AreaCodde": "",
			"Author": "汉宝",
			"Img": "sunhouzishiwoshidi.jpg",
			"HostKey": "",
			"Desc": "孙悟空：师兄教我法术。\r\n\r\n 金肆：教你一招尾兽玉，来，张嘴\r\n\r\n 菩提老祖：你弄一头小狐狸回来做什么？\r\n\r\n 金肆：我看看它有没有培养成狐狸精的潜质。",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "玄幻奇幻",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "8.8"
		}, {
			"Id": 600715,
			"Name": "我家老婆来自一千年前",
			"Area": null,
			"AreaCodde": "",
			"Author": "花还没开",
			"Img": "wojialaopolaiziyiqiannianqian.jpg",
			"HostKey": "",
			"Desc": "“我想回家。”\r\n\r\n “你可能回不去了。”\r\n\r\n “为什么？”\r\n\r\n “因为这里离你家很远。”\r\n\r\n “有多远？”\r\n\r\n “一千二百多年那么远。”\r\n\r\n 许青看着眼前来自唐朝的少女，脸上带有一丝同情：“你所熟悉的一切，都已经变成历史。”\r\n\r\n 亲朋，好友，敌人，全部沉寂在一千二百年前。\r\n\r\n ———\r\n\r\n 日常文，单女主\r\n\r\n （已有完本精品，质量保证。）",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "都市言情",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "9.5"
		}, {
			"Id": 579600,
			"Name": "全职艺术家",
			"Area": null,
			"AreaCodde": "",
			"Author": "我最白",
			"Img": "quanzhiyishujia.jpg",
			"HostKey": "",
			"Desc": "“音乐、影视、绘画、书法、雕塑、文学……”\r\n\r\n “你都懂？”\r\n\r\n “略知一二。”\r\n\r\n “都会一点的意思？”\r\n\r\n “嗯，都会亿点的意思。”\r\n\r\n 怀揣系统，靠艺术征服世界，成为各界人士顶礼膜拜的无冕之王。",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "都市言情",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "8.0"
		}, {
			"Id": 564222,
			"Name": "陆地键仙",
			"Area": null,
			"AreaCodde": "",
			"Author": "六如和尚",
			"Img": "ludijianxian.jpg",
			"HostKey": "",
			"Desc": "被雷劈的少年醒来发现自己成为公爵府上门女婿，新婚之夜被发现睡在小姨子床上，面对这地狱开局看他如何靠一块键盘逢凶化吉。天不生我祖安，喷道万古如长夜。键来！",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "玄幻奇幻",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "8.2"
		}, {
			"Id": 253077,
			"Name": "黎明之剑",
			"Area": null,
			"AreaCodde": "",
			"Author": "远瞳",
			"Img": "limingzhijian.jpg",
			"HostKey": "",
			"Desc": "高文穿越了，但穿越的时候稍微出了点问题。在某个异界大陆上空飘了十几万年之后，他觉得自己可能需要一具身体才算是成为一个完整的穿越者，但他并没想到自己好不容易成功之后竟然还需要带着这具身体从棺材里爬出来，并且面对两个吓蒙了的曾曾曾曾……曾孙女。以及一个即将迎来纪元终结的世界。",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "科幻灵异",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "9.3"
		}, {
			"Id": 3230,
			"Name": "逆天邪神",
			"Area": null,
			"AreaCodde": "",
			"Author": "火星引力",
			"Img": "nitianxieshen.jpg",
			"HostKey": "",
			"Desc": "掌天毒之珠，承邪神之血，修逆天之力，一代邪神，君临天下！【添加微信公众号：火星引力】【我们的YY频道：49554】......",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "玄幻奇幻",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "8.1"
		}]
	}, {
		"Category": "微信热书",
		"ChangeFlag": "no",
		"More": "https://scxs.pysmei.com/top/man/top/commend/week/{page}.html",
		"MoreFlag": "api",
		"NavIcon": "https://scmh.pysmei.com/pubimgs/recommend5.png",
		"ViewType": "3c3c",
		"Books": [{
			"Id": 626578,
			"Name": "都市绝世帝君",
			"Area": null,
			"AreaCodde": "",
			"Author": "当仁不让",
			"Img": "doushijueshidijun.jpg",
			"HostKey": "",
			"Desc": "一年佣人，一年上门女婿，所有人都以为我是一个窝囊废。却没有人知道，我其实是天下最神秘组织【九天】之主，人称轩辕帝君。更不知道，我还有一个惊人的秘密，那就是我已经活了一万年！",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "都市言情",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "6.0"
		}, {
			"Id": 625047,
			"Name": "吾乃皇太子",
			"Area": null,
			"AreaCodde": "",
			"Author": "黄河落日圆",
			"Img": "wunaihuangtaizi.jpg",
			"HostKey": "",
			"Desc": "穿越成为废太子，想着远离争端，挣点小钱，娶个媳妇，过个潇洒日子，可惜家国危机，朝廷动荡，废太子也是太子，山河锦绣岂能拱手让人！",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "历史军事",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "6.0"
		}, {
			"Id": 617322,
			"Name": "重生之人生巅峰",
			"Area": null,
			"AreaCodde": "",
			"Author": "李晋苏晚晴",
			"Img": "zhongshengzhirenshengdianfeng.jpg",
			"HostKey": "",
			"Desc": "前世蹉跎四十年，上天给了李晋重活一次的机会，站在2000年的拐点上，李晋发誓:\\n改写未来，走上人生巅峰！",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "都市言情",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "6.0"
		}, {
			"Id": 615714,
			"Name": "帝师王婿",
			"Area": null,
			"AreaCodde": "",
			"Author": "叶凡何思凝",
			"Img": "dishiwangxu.jpg",
			"HostKey": "",
			"Desc": "那一晚，他把自己的第一次给了一个女大学生...",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "都市言情",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "6.0"
		}, {
			"Id": 613211,
			"Name": "惊龙战神",
			"Area": null,
			"AreaCodde": "",
			"Author": "且看杯中酒",
			"Img": "jinglongzhanshen.jpg",
			"HostKey": "",
			"Desc": "女儿遭歹人掠绑，关押铁笼如狗对待，妻子含泪下跪。镇北王冲天一怒荡九州，动我妻女，本王屠你九族！",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "玄幻奇幻",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "6.0"
		}, {
			"Id": 609865,
			"Name": "我在娘胎已无敌",
			"Area": null,
			"AreaCodde": "",
			"Author": "沉沦和尚",
			"Img": "wozainiangtaiyiwudi.jpg",
			"HostKey": "",
			"Desc": "【火爆全网】【每日十更】【收藏有惊喜】\r\n\r\n 先天神道胎，混沌种青莲，不灭元始经，未出生我已无敌！\r\n\r\n 九天最强祖神宁尘重活一世，于凡尘中崛起，踏上热血争霸之路，跨千山万水，闯九天十地，一路横扫无敌，只为斩尽前世敌，救最爱之人……",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "玄幻奇幻",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "6.0"
		}]
	}, {
		"Category": "豆瓣高分",
		"ChangeFlag": "no",
		"More": "https://scxs.pysmei.com/top/man/top/new/week/{page}.html",
		"MoreFlag": "api",
		"NavIcon": "https://scmh.pysmei.com/pubimgs/recommend5.png",
		"ViewType": "1r3c3c",
		"Books": [{
			"Id": 610529,
			"Name": "从红月开始",
			"Area": null,
			"AreaCodde": "",
			"Author": "黑山老鬼",
			"Img": "conghongyuekaishi.jpg",
			"HostKey": "",
			"Desc": "红月亮出现在天上的那一刻开始，全世界的人都成了疯子。\r\n\r\n 除了我！",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "玄幻奇幻",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "9.0"
		}, {
			"Id": 584678,
			"Name": "全球迈入神话时代",
			"Area": null,
			"AreaCodde": "",
			"Author": "最终永恒",
			"Img": "quanqiumairushenhuashidai.jpg",
			"HostKey": "",
			"Desc": "平静的生活中，陆一鸣突然拥有了超能力，原本以为自己即将迈向人生巅峰，却发现整个世界已经发生了翻天覆地的变化！\r\n\r\n 古老的传说成为现实，神秘的预言被不断验证，武功、魔法、修仙、妖魔、鬼怪等各种超自然现象依次出现在世人面前。\r\n\r\n 旧有的秩序崩塌了，人类即将迎来一个全新的时代……神话时代！",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "科幻灵异",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "8.0"
		}, {
			"Id": 513562,
			"Name": "柯南之我不是蛇精病",
			"Area": null,
			"AreaCodde": "",
			"Author": "烟火酒颂",
			"Img": "kenanzhiwobushishejingbing.jpg",
			"HostKey": "",
			"Desc": "穿越名侦探柯南的世界，池非迟被送进了医院。\r\n\r\n 周二。\r\n\r\n 医生：“明天周几？”\r\n\r\n 池非迟：“周三。”\r\n\r\n 医生：“咳，明天周五。”\r\n\r\n 池非迟：“……”\r\n\r\n 8月21日。\r\n\r\n 医生：“明天几月几日？”\r\n\r\n 池非迟：“8月22日。”\r\n\r\n 医生：“咳，明天1月1日。”\r\n\r\n 池非迟：“……”\r\n\r\n 当所有人都认为混乱的时间是正确的，而其中一人无法正确辩识并融入其中，那这个人就是异",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "玄幻奇幻",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "9.0"
		}, {
			"Id": 504505,
			"Name": "盖世双谐",
			"Area": null,
			"AreaCodde": "",
			"Author": "三天两觉",
			"Img": "gaishishuangxie.jpg",
			"HostKey": "",
			"Desc": "江湖路上走走停停翻开年少漂泊的回忆如今走过这世间，万般留恋峰吹起了从前",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "武侠仙侠",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "9.3"
		}, {
			"Id": 345672,
			"Name": "天阿降临",
			"Area": null,
			"AreaCodde": "",
			"Author": "烟雨江南",
			"Img": "tianajianglin.jpg",
			"HostKey": "",
			"Desc": "楚君归，本是盛唐王朝以禁法培育的绝秘实验体，试图创造出能够征战星海任何角落的深空战士。然而在一次意外中，他脱离实验基地，破除限制，得到独立人格。自此在这星际开拓的大时代中，他征战八方，踏尽星河，终为人类开启全新时代。",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "玄幻奇幻",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "9.3"
		}, {
			"Id": 269599,
			"Name": "大医凌然",
			"Area": null,
			"AreaCodde": "",
			"Author": "志鸟村",
			"Img": "dayilingran.jpg",
			"HostKey": "",
			"Desc": "医学院学生凌然有一个小目标，要成为世界上最伟大的医生，结果不小心实现了。",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "都市言情",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "8.5"
		}, {
			"Id": 189473,
			"Name": "反叛的大魔王",
			"Area": null,
			"AreaCodde": "",
			"Author": "赵青杉",
			"Img": "fanpandedamowang.jpg",
			"HostKey": "",
			"Desc": "文艺版：不朽已提前进场，带着宁静的馥郁与芬芳。\r\n\r\n 除了破裂黑暗的聚光灯、不可恕的原罪、荆棘王冠。\r\n\r\n 我出场的时候还需要令群星颤抖的BGM、让白夜褪尽的微风以及鲜血凝结的威严之花。\r\n\r\n 通俗版：我是大魔王，我就是来装B的。",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "都市言情",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "8.6"
		}]
	}, {
		"Category": "完本精选",
		"ChangeFlag": "no",
		"More": "https://scxs.pysmei.com/top/man/top/over/week/{page}.html",
		"MoreFlag": "api",
		"NavIcon": "https://scmh.pysmei.com/pubimgs/recommend5.png",
		"ViewType": "3c3c",
		"Books": [{
			"Id": 606432,
			"Name": "学霸的日本女友",
			"Area": null,
			"AreaCodde": "",
			"Author": "转角吻猪",
			"Img": "xuebaderibennvyou.jpg",
			"HostKey": "",
			"Desc": "来自日本的美少女留学生-浅羽梨香，在父亲的安排下寄宿到了我家里，我光荣的被任命为梨香的华夏生活导师。\r\n\r\n 在相处中，我发现了她的超多秘密……\r\n\r\n 出门一定会迷路、睡觉喜欢缩成一团、喝水必然是两只手捧着杯子、对娃娃机钟爱到疯狂、决心努力赚钱自己买房……\r\n\r\n 这么笨的女孩子，我才不会喜欢！\r\n\r\n 若干年后，梨香牵着我的手问我：\r\n\r\n “沈郁，你为什么喜欢科研？”\r\n\r\n “因为世界上所有的问题，都",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "都市言情",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "9.6"
		}, {
			"Id": 482139,
			"Name": "我师兄实在太稳健了",
			"Area": null,
			"AreaCodde": "",
			"Author": "言归正传",
			"Img": "woshixiongshizaitaiwenjianle.jpg",
			"HostKey": "",
			"Desc": "重生在封神大战之前的上古时代，李长寿成了一个小小的炼气士，没有什么气运加身，也不是什么注定的大劫之子，他只有一个想要长生不老的修仙梦。\r\n\r\n 为了能在残酷的洪荒安身立命，他努力不沾因果，杀人必扬其灰，凡事谋而后动，从不轻易步入危险之中。\r\n\r\n 藏底牌，修遁术，炼丹毒，掌神通，不动稳如老狗，一动石破天惊，动后悄声走人。\r\n\r\n 本来李长寿规划中，自己会一直躲在山中平安无事的修行成仙，直到有一年，他的老",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "武侠仙侠",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "9.1"
		}, {
			"Id": 465277,
			"Name": "烂柯棋缘",
			"Area": null,
			"AreaCodde": "",
			"Author": "真费事",
			"Img": "lankeqiyuan.jpg",
			"HostKey": "",
			"Desc": "烂柯旁棋局落叶，老树间对弈无人\r\n\r\n 兴所致天元一子，再回首山海苍茫\r\n\r\n ……\r\n\r\n 一觉醒来，计缘成了一个破旧山神庙中的半瞎乞丐。\r\n\r\n 实力不够嘴炮来凑，真人一柄剑，神棍一张嘴，就是计缘在这个可怕的世界安身立足的根本。",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "武侠仙侠",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "9.0"
		}, {
			"Id": 333522,
			"Name": "转生眼中的火影世界",
			"Area": null,
			"AreaCodde": "",
			"Author": "空想之龙",
			"Img": "zhuanshengyanzhongdehuoyingshijie.jpg",
			"HostKey": "",
			"Desc": "战战兢兢的日向镜，终于得到了梦寐以求的宝物...\r\n\r\n 在宝蓝色的转生眼中，火影的世界究竟是什么样的呢？",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "玄幻奇幻",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "9.3"
		}, {
			"Id": 86745,
			"Name": "圣墟",
			"Area": null,
			"AreaCodde": "",
			"Author": "辰东",
			"Img": "shengxu.jpg",
			"HostKey": "",
			"Desc": "在破败中崛起，在寂灭中复苏。\r\n\r\n 沧海成尘，雷电枯竭，那一缕幽雾又一次临近大地，世间的枷锁被打开了，一个全新的世界就此揭开神秘的一角……",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "玄幻奇幻",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "6.0"
		}, {
			"Id": 36007,
			"Name": "修真聊天群",
			"Area": null,
			"AreaCodde": "",
			"Author": "圣骑士的传说",
			"Img": "xiuzhenliaotianqun.jpg",
			"HostKey": "",
			"Desc": "某天，感冒中的宋书航缩在床上看电影时，被一个叫‘黄山真君’的群主加入了一个聊天群——那是个仙侠中二病资深患者的交流群，里面的群友们都以‘道友’相称，群名片都是各种府主、洞主、真人、天师。连群主走失的宠物犬都称为大妖犬离家出走。整天聊的是炼丹、闯秘境、炼功经验啥的。\r\n\r\n 起初，宋书航只是为了看乐子，每天刷一遍聊天记录，看看中二病患者们的聊天日常。\r\n\r\n 直到有一天，",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "都市言情",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "9.2"
		}]
	}]
}

### 小说详情
GET https://infosxs.pigqq.com/BookFiles/Html/627/626698/info.html HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
Content-Type: application/x-www-form-urlencoded
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Host: infosxs.pigqq.com
Connection: Keep-Alive
Accept-Encoding: gzip

{"status":1,"info":"success","data":{"Id":626698,"Name":"深空彼岸","Img":"shenkongbian.jpg","Author":"辰东","Desc":"浩瀚的宇宙中，一片星系的生灭，也不过是刹那的斑驳流光。仰望星空，总有种结局已注定的伤感，千百年后你我在哪里？家国，文明火光，地球，都不过是深空中的一粒尘埃。星空一瞬，人间千年。虫鸣一世不过秋，你我一样在争渡。深空尽头到底有什么？[辰东]","CId":95,"CName":"玄幻奇幻","LastTime":"2021-09-21 22:23","FirstChapterId":3376533,"LastChapter":"第二百九十四章 秘典无数","LastChapterId":4221361,"BookStatus":"连载","SameUserBooks":[{"Id":2999,"Name":"不死不灭","Author":"辰东","Img":"busibumie.jpg","LastChapterId":5073141,"LastChapter":"我的新书《圣墟》已上传","Score":0.0},{"Id":2622,"Name":"长生界","Author":"辰东","Img":"zhangshengjie.jpg","LastChapterId":5066011,"LastChapter":"我的新书《圣墟》已上传","Score":0.0},{"Id":630630,"Name":"辰南","Author":"辰东","Img":"chennan.jpg","LastChapterId":3558616,"LastChapter":"我的新书《圣墟》现已上传","Score":0.0},{"Id":2953,"Name":"神墓","Author":"辰东","Img":"shenmu.jpg","LastChapterId":5072499,"LastChapter":"我的新书《圣墟》现已上传","Score":0.0},{"Id":86745,"Name":"圣墟","Author":"辰东","Img":"shengxu.jpg","LastChapterId":5322799,"LastChapter":"我的新书《深空彼岸》上传了","Score":0.0},{"Id":631369,"Name":"圣墟楚风","Author":"辰东","Img":"shengxuchufeng.jpg","LastChapterId":3991853,"LastChapter":"我的新书《深空彼岸》上传了","Score":0.0},{"Id":629774,"Name":"石昊","Author":"辰东","Img":"shihao.jpg","LastChapterId":4248957,"LastChapter":"我的新书《圣墟》已上传","Score":0.0},{"Id":5,"Name":"完美世界","Author":"辰东","Img":"5.jpg","LastChapterId":4755824,"LastChapter":"我的新书《圣墟》已上传","Score":0.0},{"Id":631436,"Name":"王煊秦诚","Author":"辰东","Img":"wangxuanqincheng.jpg","LastChapterId":4579415,"LastChapter":"第二百九十三章 终于进入老钟的书房","Score":0.0},{"Id":629011,"Name":"叶凡姬紫月","Author":"辰东","Img":"yefanjiziyue.jpg","LastChapterId":3691308,"LastChapter":"我的新书《圣墟》已上传","Score":0.0},{"Id":3051,"Name":"遮天","Author":"辰东","Img":"zhetian.jpg","LastChapterId":5073798,"LastChapter":"我的新书《圣墟》已上传","Score":0.0}],"SameCategoryBooks":[{"Id":573573,"Name":"从斗罗开始签到女神","Img":"congdouluokaishiqiandaonvshen.jpg","Score":2.8},{"Id":424293,"Name":"现实世界的神奇宝贝","Img":"xianshishijiedeshenqibaobei.jpg","Score":5.7},{"Id":507516,"Name":"忍界大统一","Img":"renjiedatongyi.jpg","Score":5.7},{"Id":459488,"Name":"库洛牌的魔法使","Img":"kuluopaidemofashi.jpg","Score":8.1},{"Id":265792,"Name":"武炼神帝","Img":"wulianshendi.jpg","Score":8.0},{"Id":213652,"Name":"表哥快跑","Img":"biaogekuaipao.jpg","Score":8.0},{"Id":446847,"Name":"海贼世界的木遁使用者","Img":"haizeishijiedemudunshiyongzhe.jpg","Score":8.0},{"Id":155103,"Name":"全能无敌至尊","Img":"quannengwudizhizun.jpg","Score":8.0},{"Id":614628,"Name":"快进到3077","Img":"kuaijindao3077.jpg","Score":8.0},{"Id":619972,"Name":"扭曲的日常物语","Img":"niuquderichangwuyu.jpg","Score":8.0},{"Id":613822,"Name":"超强梦幻少年","Img":"chaoqiangmenghuanshaonian.jpg","Score":8.0},{"Id":345672,"Name":"天阿降临","Img":"tianajianglin.jpg","Score":9.1}],"BookVote":{"BookId":626698,"TotalScore":2942,"VoterCount":347,"Score":8.5},"UpUser":"157******20","Declare":"该作品由 书友157******20 上传贡献，仅供在线阅读，禁止下载，转载方式传播！"}}

### 小说详情 未知接口
GET https://pinglun.chinadegi.com/Novel/sn_626698/0/index.html HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
Content-Type: application/x-www-form-urlencoded
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Host: pinglun.chinadegi.com
Connection: Keep-Alive
Accept-Encoding: gzip

{"status":1,"info":"获取数据成功","data":{"list":"{{{}}}N6s6xWefIOnWnhd2EweQ+0lQtYLn1n/xSs/UX6vmfllqV9ClqZpDk/cmmb0wTEoh5PfrGm4D4/+KLqQ7agVxMFJk1/LdjegFVIHOt10MO5fKvB73MGcvCmDxujSjEYUXRob/psFI1VUuIx+lQHPkS1ByRjWIHxOHf9Z/ODkMk4u1HLyURimorkGlFmtVbTzV337iIcA64KohjN4gJHAK9L67UzS2ivmvoRAstuqDbqrWgsLJsteeSi/sfM84GoElXe5PYgNhkkTj5SvRiwc9LRULtkgv9H8nsZhKnugmn4xhKv5HIO+3PM7Z8++FDf2Zt+rOMhVC1EI867hQbqxkbU6kBzpnihOjuueQn8yFgfwOG5rW40vHjeWus3dHYN22+Uls7XOJ8gF0gwnhkjJHMrR4DZYYlCiez3aS6HK9uxT+Q6c1tIu/IMsB+7J4voYOl7bvllKl0Lo6DBaia8CyNY5m+kVRgntwsE9HWJUXWoxs3+fB27LgylJq54XCsSwLgGtFg4hRffDLMIaRS1UJ92t+fl7U17kZk/nIGnQ4V/l0g3odlr2bOFDAFAtRdcnffA2LgWR8uFaDZ0UhPY4I9kZ/8E1IyvBC64HH+Em+4O1+TJ/B6H7ECnhB//eyHb2s/VZ7etq97PwHQwy2mB5zqy35jTmUirMv9Tzozulb/oCedwSzFp8wOA5lHs2w3HuwChBh2Sr6W4Y9PowgH9rruQcNilOpbQQhj91FgGn69mY7XdasavNqhU4RfuT11IithsxxGEWm1LP/CIZk0a8q84XMSW2PorxUnAGYXxC1IBok1657CPwEnjt2riCFWSKhfPOewlcAU7ye+77e5J6YPiObN+K+hNlqQDe8/H4H3QVhGxKWnI1d0scEnK3yOHZyqJu6jOeBhpZ6FcR/zWuLBduc992uTzD67RLoDcPP3sR/wwxNkzoUrXsuBf5i3/WFhtQ/WfxEvMaJlu/k/dAcShqmg4J+HRIdIe4jT6Dj3Ufv7+t6Gxx0tuJ47+7TxylQFVcXKhC6Mg2CGdGYaOieQvv3SFeYQQgXceCmYCkvIFtdz3RD9MY+4BnhkK29bTYhL64nEpEmVkjN6/LzDDfjZouFs7yHOIvzW8UvZnOFk/ckDSj8ryrYD3POUnIt3Ck5mDy5XqpBWOKEn+c6K+Tt3Ob/yB/cBdlaSj3TD0+WYSyVyxQT2qEoI++LI52x53cMq0jpzpYyHRZe+szyIgN35N0p0G6vypPxFcuQbMUc7go2PKmNBphpI3OEw61LwrnAdhEbVSyfxQ4VOKmwa7tb2Q1xV7BTzA+y/g9w8ETkD866RRWo1p1dEw==","Page":1,"HasNext":false}}

### 小说详情 缓存命中
POST https://userxs.pigqq.com/BookAction.aspx HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Content-Type: application/x-www-form-urlencoded
Content-Length: 27
Host: userxs.pigqq.com
Connection: Keep-Alive
Accept-Encoding: gzip

action=addhit&bookid=626698

200

### 小说 加入书架
POST https://userxs.pigqq.com/BookAction.aspx HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Content-Type: application/x-www-form-urlencoded
Content-Length: 32
Host: userxs.pigqq.com
Connection: Keep-Alive
Accept-Encoding: gzip

action=addbookcase&bookId=626698

{"status":1,"info":"success","data":{"result": "2"}}

### 小说 弹幕
GET https://dmapp.chinadegi.com/Novel/626698/3376533.html HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
Content-Type: application/x-www-form-urlencoded
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Host: dmapp.chinadegi.com
Connection: Keep-Alive
Accept-Encoding: gzip

{"status":1,"info":"获取数据成功！","data":{"result":1,"list":"[{\"BookId\":\"626698\",\"ChapterId\":\"3376533\",\"Content\":\"王煊？王腾的什么人\",\"Tags\":\"\",\"UserIn\":\"Novel\",\"Color\":\"#ffffff\",\"Addtime\":\"2021/09/20 18:08:09\"},{\"BookId\":\"626698\",\"ChapterId\":\"3376533\",\"Content\":\"这是新系列还是荒那个系列\",\"Tags\":\"\",\"UserIn\":\"Novel\",\"Color\":\"#99cc00\",\"Addtime\":\"2021/09/19 16:01:55\"},{\"BookId\":\"626698\",\"ChapterId\":\"3376533\",\"Content\":\"不穿越吗\",\"Tags\":\"\",\"UserIn\":\"Novel\",\"Color\":\"#ff4444\",\"Addtime\":\"2021/09/17 23:19:47\"},{\"BookId\":\"626698\",\"ChapterId\":\"3376533\",\"Content\":\"不穿越吗？\",\"Tags\":\"\",\"UserIn\":\"Novel\",\"Color\":\"#ffffff\",\"Addtime\":\"2021/09/17 23:19:35\"},{\"BookId\":\"626698\",\"ChapterId\":\"3376533\",\"Content\":\"举报学校。我们已经成功了。\",\"Tags\":\"\",\"UserIn\":\"Novel\",\"Color\":\"#ffffff\",\"Addtime\":\"2021/09/17 15:31:27\"},{\"BookId\":\"626698\",\"ChapterId\":\"3376533\",\"Content\":\"真水啊\",\"Tags\":\"\",\"UserIn\":\"Novel\",\"Color\":\"#ffffff\",\"Addtime\":\"2021/09/13 16:54:01\"},{\"BookId\":\"626698\",\"ChapterId\":\"3376533\",\"Content\":\"我是你爹的爹\",\"Tags\":\"\",\"UserIn\":\"Novel\",\"Color\":\"#ffffff\",\"Addtime\":\"2021/09/11 20:05:28\"},{\"BookId\":\"626698\",\"ChapterId\":\"3376533\",\"Content\":\"大家好，我是嫩爹\",\"Tags\":\"\",\"UserIn\":\"Novel\",\"Color\":\"#ffffff\",\"Addtime\":\"2021/09/10 09:45:04\"},{\"BookId\":\"626698\",\"ChapterId\":\"3376533\",\"Content\":\"我嫩叠\",\"Tags\":\"\",\"UserIn\":\"Novel\",\"Color\":\"#ffffff\",\"Addtime\":\"2021/09/08 18:07:49\"},{\"BookId\":\"626698\",\"ChapterId\":\"3376533\",\"Content\":\"大家好\",\"Tags\":\"\",\"UserIn\":\"Novel\",\"Color\":\"#ffffff\",\"Addtime\":\"2021/09/08 10:51:04\"},{\"BookId\":\"626698\",\"ChapterId\":\"3376533\",\"Content\":\"都是现代修仙，能换点花样？\",\"Tags\":\"\",\"UserIn\":\"Novel\",\"Color\":\"#ffffff\",\"Addtime\":\"2021/09/08 02:11:35\"},{\"BookId\":\"626698\",\"ChapterId\":\"3376533\",\"Content\":\"你家在哪？指个方向\",\"Tags\":\"\",\"UserIn\":\"Novel\",\"Color\":\"#ffffff\",\"Addtime\":\"2021/09/08 00:51:12\"},{\"BookId\":\"626698\",\"ChapterId\":\"3376533\",\"Content\":\"我孙王腾有大帝之资\",\"Tags\":\"\",\"UserIn\":\"Novel\",\"Color\":\"#ffffff\",\"Addtime\":\"2021/09/07 01:38:25\"},{\"BookId\":\"626698\",\"ChapterId\":\"3376533\",\"Content\":\"我是在座各位所有人的爹\",\"Tags\":\"\",\"UserIn\":\"Novel\",\"Color\":\"#ffffff\",\"Addtime\":\"2021/09/04 04:11:35\"},{\"BookId\":\"626698\",\"ChapterId\":\"3376533\",\"Content\":\"哈哈哈\",\"Tags\":\"\",\"UserIn\":\"Novel\",\"Color\":\"#ffffff\",\"Addtime\":\"2021/09/02 01:23:26\"},{\"BookId\":\"626698\",\"ChapterId\":\"3376533\",\"Content\":\"王仙帝\",\"Tags\":\"\",\"UserIn\":\"Novel\",\"Color\":\"#ffffff\",\"Addtime\":\"2021/09/01 18:48:09\"},{\"BookId\":\"626698\",\"ChapterId\":\"3376533\",\"Content\":\"牛马\",\"Tags\":\"\",\"UserIn\":\"Novel\",\"Color\":\"#ffffff\",\"Addtime\":\"2021/08/30 20:12:58\"},{\"BookId\":\"626698\",\"ChapterId\":\"3376533\",\"Content\":\"弟弟\",\"Tags\":\"\",\"UserIn\":\"Novel\",\"Color\":\"#ffffff\",\"Addtime\":\"2021/08/30 20:05:49\"},{\"BookId\":\"626698\",\"ChapterId\":\"3376533\",\"Content\":\"红毛东\",\"Tags\":\"\",\"UserIn\":\"Novel\",\"Color\":\"#ff4444\",\"Addtime\":\"2021/08/29 22:52:16\"},{\"BookId\":\"626698\",\"ChapterId\":\"3376533\",\"Content\":\"赞\",\"Tags\":\"\",\"UserIn\":\"Novel\",\"Color\":\"#ffffff\",\"Addtime\":\"2021/08/28 07:37:32\"},{\"BookId\":\"626698\",\"ChapterId\":\"3376533\",\"Content\":\"领券半价点外卖去薇芯搜小贤饭票\",\"Tags\":\"\",\"UserIn\":\"Novel\",\"Color\":\"#ff4444\",\"Addtime\":\"2021/08/27 00:17:03\"},{\"BookId\":\"626698\",\"ChapterId\":\"3376533\",\"Content\":\"领券半价点外卖去薇芯搜小贤饭票\",\"Tags\":\"\",\"UserIn\":\"Novel\",\"Color\":\"#ff4444\",\"Addtime\":\"2021/08/27 00:16:25\"},{\"BookId\":\"626698\",\"ChapterId\":\"3376533\",\"Content\":\"荒天帝无敌\",\"Tags\":\"\",\"UserIn\":\"Novel\",\"Color\":\"#ffffff\",\"Addtime\":\"2021/08/25 20:25:38\"},{\"BookId\":\"626698\",\"ChapterId\":\"3376533\",\"Content\":\"我儿王腾有大帝之资\",\"Tags\":\"\",\"UserIn\":\"Novel\",\"Color\":\"#ffffff\",\"Addtime\":\"2021/08/23 23:42:34\"},{\"BookId\":\"626698\",\"ChapterId\":\"3376533\",\"Content\":\"啊啊啊，我好难受，我感觉有红毛要破体而出\",\"Tags\":\"\",\"UserIn\":\"Novel\",\"Color\":\"#ffffff\",\"Addtime\":\"2021/08/23 21:04:43\"},{\"BookId\":\"626698\",\"ChapterId\":\"3376533\",\"Content\":\"我有生之年还能看完吗\",\"Tags\":\"\",\"UserIn\":\"Novel\",\"Color\":\"#ffffff\",\"Addtime\":\"2021/08/23 17:51:50\"},{\"BookId\":\"626698\",\"ChapterId\":\"3376533\",\"Content\":\"敏感词？\",\"Tags\":\"\",\"UserIn\":\"Novel\",\"Color\":\"#ffffff\",\"Addtime\":\"2021/08/23 01:34:43\"},{\"BookId\":\"626698\",\"ChapterId\":\"3376533\",\"Content\":\"尼玛\",\"Tags\":\"\",\"UserIn\":\"Novel\",\"Color\":\"#ffffff\",\"Addtime\":\"2021/08/23 01:34:29\"},{\"BookId\":\"626698\",\"ChapterId\":\"3376533\",\"Content\":\"很好\",\"Tags\":\"\",\"UserIn\":\"Novel\",\"Color\":\"#ff4444\",\"Addtime\":\"2021/08/22 23:26:47\"},{\"BookId\":\"626698\",\"ChapterId\":\"3376533\",\"Content\":\"谁在称拖更？哪个人敢言水货？网文时代都不\",\"Tags\":\"\",\"UserIn\":\"Novel\",\"Color\":\"#ffffff\",\"Addtime\":\"2021/08/22 22:15:20\"},{\"BookId\":\"626698\",\"ChapterId\":\"3376533\",\"Content\":\"，\",\"Tags\":\"\",\"UserIn\":\"Novel\",\"Color\":\"#ffffff\",\"Addtime\":\"2021/08/22 20:32:41\"},{\"BookId\":\"626698\",\"ChapterId\":\"3376533\",\"Content\":\"我儿王腾有大帝之资\",\"Tags\":\"\",\"UserIn\":\"Novel\",\"Color\":\"#33b5e5\",\"Addtime\":\"2021/08/22 13:48:45\"},{\"BookId\":\"626698\",\"ChapterId\":\"3376533\",\"Content\":\"又是熟悉的套路\",\"Tags\":\"\",\"UserIn\":\"Novel\",\"Color\":\"#ffffff\",\"Addtime\":\"2021/08/21 18:17:05\"},{\"BookId\":\"626698\",\"ChapterId\":\"3376533\",\"Content\":\"又该王家人当主角啦？\",\"Tags\":\"\",\"UserIn\":\"Novel\",\"Color\":\"#ffffff\",\"Addtime\":\"2021/08/19 21:48:16\"},{\"BookId\":\"626698\",\"ChapterId\":\"3376533\",\"Content\":\"万年不变同学聚会\",\"Tags\":\"\",\"UserIn\":\"Novel\",\"Color\":\"#ffffff\",\"Addtime\":\"2021/08/19 14:11:05\"},{\"BookId\":\"626698\",\"ChapterId\":\"3376533\",\"Content\":\"辰东改写科幻了？\",\"Tags\":\"\",\"UserIn\":\"Novel\",\"Color\":\"#ff4444\",\"Addtime\":\"2021/08/18 07:20:01\"},{\"BookId\":\"626698\",\"ChapterId\":\"3376533\",\"Content\":\"发发发\",\"Tags\":\"\",\"UserIn\":\"Novel\",\"Color\":\"#ffffff\",\"Addtime\":\"2021/08/17 15:44:22\"},{\"BookId\":\"626698\",\"ChapterId\":\"3376533\",\"Content\":\"好人\",\"Tags\":\"\",\"UserIn\":\"Novel\",\"Color\":\"#ffffff\",\"Addtime\":\"2021/08/16 15:41:11\"},{\"BookId\":\"626698\",\"ChapterId\":\"3376533\",\"Content\":\"我儿王煊有大帝之资\",\"Tags\":\"\",\"UserIn\":\"Novel\",\"Color\":\"#F9739A\",\"Addtime\":\"2021/08/16 15:27:55\"},{\"BookId\":\"626698\",\"ChapterId\":\"3376533\",\"Content\":\"红毛怪辰东\",\"Tags\":\"\",\"UserIn\":\"Novel\",\"Color\":\"#ffffff\",\"Addtime\":\"2021/08/16 13:20:12\"},{\"BookId\":\"626698\",\"ChapterId\":\"3376533\",\"Content\":\"我是你爹\",\"Tags\":\"\",\"UserIn\":\"Novel\",\"Color\":\"#ffffff\",\"Addtime\":\"2021/08/16 03:17:32\"},{\"BookId\":\"626698\",\"ChapterId\":\"3376533\",\"Content\":\"有什么办法可以延迟开学？\",\"Tags\":\"\",\"UserIn\":\"Novel\",\"Color\":\"#ffffff\",\"Addtime\":\"2021/08/15 11:06:13\"},{\"BookId\":\"626698\",\"ChapterId\":\"3376533\",\"Content\":\"要开学了\",\"Tags\":\"\",\"UserIn\":\"Novel\",\"Color\":\"#ff4444\",\"Addtime\":\"2021/08/15 11:05:02\"},{\"BookId\":\"626698\",\"ChapterId\":\"3376533\",\"Content\":\"不详预感\",\"Tags\":\"\",\"UserIn\":\"Novel\",\"Color\":\"#ffffff\",\"Addtime\":\"2021/08/14 17:32:23\"},{\"BookId\":\"626698\",\"ChapterId\":\"3376533\",\"Content\":\"哦豁\",\"Tags\":\"\",\"UserIn\":\"Novel\",\"Color\":\"#ffffff\",\"Addtime\":\"2021/08/14 17:31:30\"},{\"BookId\":\"626698\",\"ChapterId\":\"3376533\",\"Content\":\"老辰晚年不祥\",\"Tags\":\"\",\"UserIn\":\"Novel\",\"Color\":\"#ffffff\",\"Addtime\":\"2021/08/13 08:49:25\"},{\"BookId\":\"626698\",\"ChapterId\":\"3376533\",\"Content\":\"不是吧\",\"Tags\":\"\",\"UserIn\":\"Novel\",\"Color\":\"#ffffff\",\"Addtime\":\"2021/08/09 09:43:44\"},{\"BookId\":\"626698\",\"ChapterId\":\"3376533\",\"Content\":\"哈哈哈哈\",\"Tags\":\"\",\"UserIn\":\"Novel\",\"Color\":\"#ffffff\",\"Addtime\":\"2021/08/04 08:19:06\"}]"}}

### 小说 正文
GET https://contentxs.pigqq.com/BookFiles/Html/627/626698/3376533.html HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
Content-Type: application/x-www-form-urlencoded
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Host: contentxs.pigqq.com
Connection: Keep-Alive
Accept-Encoding: gzip

{"status":1,"info":"success","data":{"id":626698,"name":"深空彼岸","cid":3376533,"cname":"第一章 旧土","pid":-1,"nid":3376534,"content":"\r\n　　红日西坠，列车远去，在与铁轨的震动声中带起大片枯黄的落叶，也带起秋的萧瑟。\r\n　　王煊注视，直至列车渐消失，他才收回目光，又送走了几位同学。\r\n　　自此一别，将天各一方，不知道多少年后才能再相见，甚至有些人再无重逢期。\r\n　　周围，有人还在缓慢地挥手，久久未曾放下，也有人沉默着，颇为伤感。\r\n　　大学四年，一起走过，积淀下的情谊总有些难以割舍。\r\n　　落日余晖斜照飘落的黄叶，光影斑驳，交织出几许岁月流逝之感。\r\n　　一位清秀的女生转过身去，暗自擦去镜片后的眼泪。\r\n　　在这个特殊的年代，毕业后他们将各自归去，此生可能都不再相遇。\r\n　　秋风吹过，黄叶凌乱，纷纷扬扬。\r\n　　在这个季节，有人失意，有人得意。\r\n　　毕业四个月了，有人留在了这座城市，前程灿烂，也有人在忐忑中等待，坚守，而更多的人则怅然离去，将回故里。\r\n　　王煊走在回去的路上，也在想自己将何去何从。\r\n　　街道陈旧，路两旁的梧桐树大片地坠落叶子，满地都是。\r\n　　有人与他并肩走在一起，为他鸣不平：“留下的人没有你，为什么会这样？他们竟将你放弃！”\r\n　　身为同窗兼好友，在秦诚看来，但凡有名额都绕不开王煊，他必然会被选中。\r\n　　结果出来后，许多人心情复杂，王煊居然落选。\r\n　　“不说我了，你怎么样，有结果了吗？”王煊问他。\r\n　　秦诚小声告诉他，家里托了关系，可能要去新月。\r\n　　“新月，深空对岸，不知道以后我们还能不能再见。”王煊停下脚步，身边的好友都将远行了。\r\n　　他身材颀长，并不单薄，匀称有力，在晚霞中，身上有一层淡金光彩，一双眼睛清澈而有神。\r\n　　“我会回来的，肯定还能相见。”秦诚是个感性的人，难舍故土，尤其是想到，很难再见到好友，心中有些不好受。\r\n　　“回来时喊我！”王煊用力抱了抱他的肩头。\r\n　　风中有哽咽声传来，王煊与秦诚回头，看到一位男同学情绪很激动。\r\n　　他脸色苍白，哭出声来，用力喊着：“我真的很想留在这座城市，想等到最后的机会，我不想这样回老家！”\r\n　　在这里生活与学习了四年，他已经很努力了，拼搏、争取、规划自己的未来，想找到自己的位置，但终究留不下来。\r\n　　他失声痛哭。\r\n　　秋风带着凉意，一些同窗跟着心情低落。\r\n　　另一边，一对情侣停下脚步，彼此相顾，没有言语，只是在无声地落泪。\r\n　　他们将分别，从此以后相距不是数千里，而是隔着一片星空，此生或许再也见不到了。\r\n　　两人脸上满是泪水，最后一次相拥，而后，只剩下沉默。\r\n　　这座城市很大，但却有些陈旧，保留着旧时代的痕迹，路旁不少古树都很粗，有一两百年了。\r\n　　相对而言，整座城市承接过去的风格，在岁月中保存下来。\r\n　　其他地方，有些旧时代留下的城市则废弃了，久无人迹，大面积的荒芜，爬满藤蔓，荆棘丛生，渐渐被草木淹没。\r\n　　回到校区后，秦诚还在为王煊不忿，劝他去找人了解原因，为什么被放弃，讨一个说法。\r\n　　即便毕业了，他们也被允许住宿在校区，直到确定完最终的所有人选。\r\n　　这次机会难得，被选中的人留在这座城市等待，不久后将前往新星，那边似乎有了某种非同寻常的发现。\r\n　　秦诚也没有被选中，他家里人费尽力气也只是给了他进入深空的机会。\r\n　　他将前往新月，那颗围绕新星转动的月亮，是新星外最重要的基地。\r\n　　秦诚低声道：“你知道吗，即便现在那边只有一鳞半爪的传闻，也已经让提前得到小道消息的人热血沸腾。无论如何，你都要得到一个名额！”\r\n　　月色下，树影婆娑，王煊在草坪上舒展身体，他在演练旧时代的“散术”，实战性极强，将地面上大量的黄叶都带动的飞舞了起来，漫天都是。\r\n　　他没有停下，动作很快，但呼吸平稳，道：“我在等最后的结果。”\r\n　　深空无垠，宇宙广袤，但它却是冰冷的，死寂的，除却旧土外，人们只寻到另外一颗生命新星。\r\n　　然而，很多年前，移居新星的大门就关闭了，旧土的普通人很难再进入。\r\n　　相对新星，有些人逐渐开始将这里称为旧土。\r\n　　而昔日，这里名为地球，是人类的起源地。\r\n　　或许，它的确有些“陈旧”了，各地有不少荒芜的城市，蒿草丛生，无人居住。\r\n　　所有这一切，都是因为旧时代的一场战争导致的。\r\n　　当科技发展到一定高度，一旦发生热战将非常可怕。\r\n　　繁华世界被摧毁，变得无比荒凉与萧条。\r\n　　当时，有大批的人逃向太空中。\r\n　　其实，那时人类的科技并没有想象中那么璀璨，战前刚开始在月球上建立基地。\r\n　　所以，逃走的人只能暂时以月亮为立足地。\r\n　　就是在这种情况下，人类竟突然间实现大迁移，发现并进入一颗生命新星！\r\n　　旧土的人至今都觉得不可思议。\r\n　　许多人都不禁对那个历史时间节点产生疑问，究竟是什么原因导致前沿科技突然大爆发？\r\n　　各方讳莫如深。\r\n　　以当年的科技高度而言，无论是稳态虫洞，还是曲速引擎等黑科技，都不可能在短时间内实现。\r\n　　旧土有人怀疑，一切答案都可能在月球上！\r\n　　可惜，热战造成的后果太严重了，大地半摧毁，旧土这么多年过去都没有恢复过来，科技等严重倒退，很长时间无法登月。\r\n　　一百多年过去了，旧土人口才恢复到十亿左右，远无法与当年相比，许多地方至今都还很荒凉。\r\n　　早期开发新星时，曾将旧土大量的幸存者带走，大批人才随之离去，这也是旧土严重倒退、久未恢复的原因之一，而这种大迁移持续了数十年。\r\n　　直到百余年前，新星才关闭大门。\r\n　　再加上热战后大地上满目疮痍，环境极其恶劣，旧土人口没剩下多少，想要恢复谈何容易。\r\n　　朦胧月光下，王煊正在演绎“散术”，动作忽然加快，砰的一声，其右手在一棵大树上留下清晰的手印，大树剧烈颤动，漫天黄叶如瀑坠落。\r\n　　秦诚很吃惊：“散术，你竟然真的练出了一些名堂？他们放弃你绝对会后悔的！”\r\n　　嫩嫩的新书，向大家打声招呼，别忘记收藏，请多支持，后面还有章节。\r\n　　\f\t\n","hasContent":1}}

### 小说 目录
GET https://infosxs.pigqq.com/BookFiles/Html/627/626698/index.html HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
Content-Type: application/x-www-form-urlencoded
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Host: infosxs.pigqq.com
Connection: Keep-Alive
Accept-Encoding: gzip

{"status":1,"info":"success","data":{"id":626698, "name":"深空彼岸","list":[{"name":"正文卷","list":[{"id":3376533,"name":"第一章 旧土","hasContent":1},{"id":3376534,"name":"第二章 韶华易逝","hasContent":1},{"id":3376535,"name":"第三章 续命项目","hasContent":1},{"id":3376858,"name":"第四章 超自然","hasContent":1},{"id":3392860,"name":"第五章 弃若敝履","hasContent":1},{"id":3393444,"name":"第六章 女神","hasContent":1},{"id":3395508,"name":"第七章 列仙不存","hasContent":1},{"id":3408495,"name":"第八章 聚会","hasContent":1},{"id":3410068,"name":"第九章 同窗","hasContent":1},{"id":3410751,"name":"第十章 新术","hasContent":1},{"id":3460819,"name":"第十一章 新旧争锋","hasContent":1},{"id":3461416,"name":"第十二章 温和俯视","hasContent":1},{"id":3472286,"name":"第十三章 旧术路的尽头","hasContent":1},{"id":3473120,"name":"第十四章 探险","hasContent":1},{"id":3475776,"name":"第十五章 羽化","hasContent":1},{"id":3476551,"name":"第十六章 银色兽皮书","hasContent":1},{"id":3478406,"name":"第十七章 截胡","hasContent":1},{"id":3479107,"name":"第十八章 偶遇","hasContent":1},{"id":3480757,"name":"第十九章 前女友","hasContent":1},{"id":3483449,"name":"第二十章 小王太猛","hasContent":1},{"id":3486700,"name":"第二十一章 不许成精","hasContent":1},{"id":3491394,"name":"第二十二章 与死亡擦肩","hasContent":1},{"id":3493881,"name":"第二十三章 超感","hasContent":1},{"id":3494837,"name":"第二十四章 先秦竹简的正确开启方式","hasContent":1},{"id":3498164,"name":"第二十五章 接触神秘","hasContent":1},{"id":3499143,"name":"第二十六章 不具普适性","hasContent":1},{"id":3500495,"name":"第二十七章 仙坟","hasContent":1},{"id":3509205,"name":"第二十八章 钓鱼","hasContent":1},{"id":3511161,"name":"第二十九章 活着的女方士","hasContent":1},{"id":3518772,"name":"第三十章 登仙失败","hasContent":1},{"id":3520406,"name":"第三十一章 长生种计划","hasContent":1},{"id":3521601,"name":"第三十二章 奇物","hasContent":1},{"id":3523420,"name":"第三十三章 通向内景地的捷径","hasContent":1},{"id":3524269,"name":"第三十四章 你走光了","hasContent":1},{"id":3527466,"name":"第三十五章 近仙近妖","hasContent":1},{"id":3528217,"name":"第三十六章 出事儿了","hasContent":1},{"id":3531064,"name":"第三十七章 天仙伴入眠","hasContent":1},{"id":3531907,"name":"第三十八章 雨中寻仙","hasContent":1},{"id":3549231,"name":"第三十九章 黑山大战","hasContent":1},{"id":3550194,"name":"第四十章 为旧术蹚出一条路","hasContent":1},{"id":3568727,"name":"第四十一章 人生第一次","hasContent":1},{"id":3569739,"name":"第四十二章 老陈归来","hasContent":1},{"id":3571987,"name":"第四十三章 仙佛在侧","hasContent":1},{"id":3572907,"name":"第四十四章 佛求凡人当如何","hasContent":1},{"id":3575235,"name":"第四十五章 菩萨搬迁","hasContent":1},{"id":3577487,"name":"第四十六章 邂逅","hasContent":1},{"id":3582119,"name":"第四十七章 千金司机","hasContent":1},{"id":3594017,"name":"第四十八章 来自深空的信","hasContent":1},{"id":3599861,"name":"第四十九章 招仙的体质","hasContent":1},{"id":3603053,"name":"第五十章 稀世神物","hasContent":1},{"id":3607260,"name":"第五十一章 理念与利益","hasContent":1},{"id":3607990,"name":"第五十二章 新旧对决","hasContent":1},{"id":3609306,"name":"第五十三章 旧术最后的辉煌","hasContent":1},{"id":3627979,"name":"第五十四章 大宗师","hasContent":1},{"id":3629200,"name":"第五十五章 挖旧术的根","hasContent":1},{"id":3630221,"name":"第五十六章 被截了个大胡","hasContent":1},{"id":3632070,"name":"第五十七章 璀璨落幕","hasContent":1},{"id":3633879,"name":"第五十八章 以一己之力为旧术续命","hasContent":1},{"id":3647219,"name":"第五十九章 激起血性","hasContent":1},{"id":3661148,"name":"第六十章 老陈的护道人","hasContent":1},{"id":3661149,"name":"第六十一章 登仙遗物","hasContent":1},{"id":3662407,"name":"第六十二章 众志成城","hasContent":1},{"id":3664793,"name":"第六十三章 女剑仙","hasContent":1},{"id":3666341,"name":"第六十四章 王教祖","hasContent":1},{"id":3668582,"name":"第六十五章 看见剑就想吐","hasContent":1},{"id":3669220,"name":"第六十六章 安城圈贵","hasContent":1},{"id":3673518,"name":"第六十七章 古今境界层次初对照","hasContent":1},{"id":3674299,"name":"第六十八章 内景之忧","hasContent":1},{"id":3675650,"name":"第六十九章 最后的宁静时光","hasContent":1},{"id":3687021,"name":"第七十章 抱爆了","hasContent":1},{"id":3688510,"name":"第七十一章 老陈被猫叼走了","hasContent":1},{"id":3689414,"name":"第七十二章 菩萨吓跑","hasContent":1},{"id":3699151,"name":"第七十三章 强势女妖仙","hasContent":1},{"id":3699912,"name":"第七十四章 内景地第一次染血","hasContent":1},{"id":3702464,"name":"第七十五章 小王立威","hasContent":1},{"id":3707484,"name":"第七十六章 心有热血","hasContent":1},{"id":3709287,"name":"第七十七章 只身凿穿所有阵营","hasContent":1},{"id":3711067,"name":"第七十八章 宝藏少年","hasContent":1},{"id":3712963,"name":"第七十九章 三年后世界会何等恐怖","hasContent":1},{"id":3717523,"name":"第八十章 三年之约","hasContent":1},{"id":3730219,"name":"第八十一章 旧约锁真言","hasContent":1},{"id":3733341,"name":"第八十二章 捋清旧术史","hasContent":1},{"id":3744140,"name":"第八十三章 旧术不旧","hasContent":1},{"id":3753483,"name":"第八十四章 战舰可否打杀列仙","hasContent":1},{"id":3777251,"name":"第八十五章 雨夜奔杀","hasContent":1},{"id":3778221,"name":"第八十六章 王宗师!","hasContent":1},{"id":3780386,"name":"第八十七章 神话","hasContent":1},{"id":3781773,"name":"第八十八章 时代变了","hasContent":1},{"id":3781931,"name":"第八十九章 雷霆滚滚杀人夜","hasContent":1},{"id":3785187,"name":"第九十章 明天会怎样","hasContent":1},{"id":3789820,"name":"第九十一章 鬼神退避的古剑","hasContent":1},{"id":3792079,"name":"第九十二章 终于可以参加葬礼","hasContent":1},{"id":3796315,"name":"第九十三章 图文并茂","hasContent":1},{"id":3801035,"name":"第九十四章 驾驶飞船采摘天药","hasContent":1},{"id":3808231,"name":"第九十五章 仙口夺食","hasContent":1},{"id":3819596,"name":"第九十六章 宗师意识","hasContent":1},{"id":3819597,"name":"第九十七章 红颜知己","hasContent":1},{"id":3822418,"name":"第九十八章 向往列仙的异类","hasContent":1},{"id":3822419,"name":"第九十九章 深空密地","hasContent":1},{"id":3824366,"name":"第一百章 璀璨的王宗师","hasContent":1},{"id":3825800,"name":"第一百零一章 天纵神资","hasContent":1},{"id":3828434,"name":"第一百零二章 曲终人散","hasContent":1},{"id":3830065,"name":"第一百零三章 扎心分别","hasContent":1},{"id":3832805,"name":"第一百零四章 神秘接触","hasContent":1},{"id":3838073,"name":"第一百零五章 星际旅行","hasContent":1},{"id":3850750,"name":"第一百零六章 偶遇","hasContent":1},{"id":3855578,"name":"第一百零七章 月亮之上","hasContent":1},{"id":3860260,"name":"第一百零八章 菩萨们太热情了","hasContent":1},{"id":3879004,"name":"第一百零九章 老凌威武","hasContent":1},{"id":3881005,"name":"第一百一十章 追求与践行","hasContent":1},{"id":3882826,"name":"第一百一十一章 杀了个仙人","hasContent":1},{"id":3883725,"name":"第一百一十二章 被仙盯上","hasContent":1},{"id":3885572,"name":"第一百一十三章 神话不在现世中","hasContent":1},{"id":3886260,"name":"第一百一十四章 月坑爆了","hasContent":1},{"id":3888156,"name":"第一百一十五章 人间属于谁","hasContent":1},{"id":3889432,"name":"第一百一十六章 战舰打列仙","hasContent":1},{"id":3891039,"name":"第一百一十七章 大幕后的世界","hasContent":1},{"id":3892157,"name":"第一百一十八章 旧约的代价与报复","hasContent":1},{"id":3893805,"name":"第一百一十九章 初临新世界","hasContent":1},{"id":3894736,"name":"第一百二十章 新星原住民","hasContent":1},{"id":3896434,"name":"第一百二十一章 密地所在","hasContent":1},{"id":3897302,"name":"第一百二十二章 团灭是常态","hasContent":1},{"id":3899191,"name":"第一百二十三章 老钟扛着战舰跑了","hasContent":1},{"id":3900263,"name":"第一百二十四章 赵女神","hasContent":1},{"id":3902557,"name":"第一百二十五章 大时代临近","hasContent":1},{"id":3903355,"name":"第一百二十六章 星辰大海","hasContent":1},{"id":3904899,"name":"第一百二十七章 那一脚的风情","hasContent":1},{"id":3905995,"name":"第一百二十八章 新世界初体验","hasContent":1},{"id":3907563,"name":"第一百二十九章 月夜人面现","hasContent":1},{"id":3907752,"name":"上架感言","hasContent":0},{"id":3908219,"name":"第一百三十章 血色浪漫","hasContent":1},{"id":3908367,"name":"第一百三十一章 月夜奇迹","hasContent":1},{"id":3908368,"name":"第一百三十二章 人性","hasContent":1},{"id":3908471,"name":"第一百三十三章 情侣","hasContent":1},{"id":3910140,"name":"第一百三十四章 蛟","hasContent":1},{"id":3910974,"name":"第一百三十五章 金身再蜕变","hasContent":1},{"id":3911115,"name":"感谢大家!","hasContent":0},{"id":3912789,"name":"第一百三十六章 大宗师","hasContent":1},{"id":3913670,"name":"第一百三十七章 黑暗密地","hasContent":1},{"id":3915258,"name":"第一百三十八章 单骑杀穿敌营","hasContent":1},{"id":3916239,"name":"第一百三十九章 拯救","hasContent":1},{"id":3922441,"name":"第一百四十章 不超凡皆尘埃","hasContent":1},{"id":3923474,"name":"第一百四十一章 在异域娶妻生子","hasContent":1},{"id":3935233,"name":"第一百四十二章 密地新人类","hasContent":1},{"id":3937244,"name":"第一百四十三章 杀外星人","hasContent":1},{"id":3939606,"name":"第一百四十四章 小钟宝物无数","hasContent":1},{"id":3940392,"name":"第一百四十五章 狩猎超凡","hasContent":1},{"id":3941734,"name":"第一百四十六章 超凡之吻","hasContent":1},{"id":3942568,"name":"第一百四十七章 与佛陀试比高","hasContent":1},{"id":3945097,"name":"第一百四十八章 成为妖魔","hasContent":1},{"id":3946423,"name":"第一百四十九章 羽化摆渡人","hasContent":1},{"id":3952135,"name":"第一百五十章 与列仙交易","hasContent":1},{"id":3952910,"name":"第一百五十一章 熟仙相见分外眼红","hasContent":1},{"id":3954407,"name":"第一百五十二章 又见红衣妖仙","hasContent":1},{"id":3955113,"name":"第一百五十三章 人间有约","hasContent":1},{"id":3958939,"name":"第一百五十四章 外围之变","hasContent":1},{"id":3960247,"name":"第一百五十五章 一切只为造化","hasContent":1},{"id":3962297,"name":"第一百五十六章 万古夜未央","hasContent":1},{"id":3962299,"name":"第一百五十七章 重逢","hasContent":1},{"id":3968483,"name":"第一百五十八章 实力全面暴露","hasContent":1},{"id":3970407,"name":"第一百五十九章 恋人未满","hasContent":1},{"id":3975692,"name":"第一百六十章 从旧土跟来","hasContent":1},{"id":3981297,"name":"第一百六十一章 不再是仙","hasContent":1},{"id":3983219,"name":"第一百六十二章 真没想钓鱼","hasContent":1},{"id":3983845,"name":"第一百六十三章 地仙炸开","hasContent":1},{"id":3985845,"name":"第一百六十四章 列仙觊觎的奇物","hasContent":1},{"id":3986818,"name":"第一百六十五章 内景之变","hasContent":1},{"id":3988894,"name":"第一百六十六章 地仙泉","hasContent":1},{"id":3991979,"name":"第一百六十七章 造化","hasContent":1},{"id":3997207,"name":"第一百六十八章 斩超凡","hasContent":1},{"id":3998588,"name":"第一百六十九章 金榜垂钓","hasContent":1},{"id":3999561,"name":"第一百七十章 万法皆朽","hasContent":1},{"id":4001193,"name":"第一百七十一章 染着列仙血的石板经文","hasContent":1},{"id":4003197,"name":"第一百七十二章 最强根须养成","hasContent":1},{"id":4004349,"name":"第一百七十三章 现世最后的大方士","hasContent":1},{"id":4005179,"name":"第一百七十四章 狐狸精吴茵","hasContent":1},{"id":4006499,"name":"第一百七十五章 狐王茵","hasContent":1},{"id":4007309,"name":"第一百七十六章 赔进去两人一兽","hasContent":1},{"id":4008534,"name":"第一百七十七章 天人五衰病由来","hasContent":1},{"id":4009265,"name":"第一百七十八章 列仙舞","hasContent":1},{"id":4010537,"name":"第一百七十九章 顶级秘法","hasContent":1},{"id":4011646,"name":"第一百八十章 妖魔大乱","hasContent":1},{"id":4013076,"name":"第一百八十一章 常年背锅陈","hasContent":1},{"id":4014033,"name":"第一百八十二章 古代修行路的几大境界","hasContent":1},{"id":4015354,"name":"第一百八十三章 踏足超凡领域","hasContent":1},{"id":4016506,"name":"第一百八十四章 摆渡人吓毛了","hasContent":1},{"id":4018650,"name":"第一百八十五章 复仇者联盟","hasContent":1},{"id":4021786,"name":"第一百八十六章 老钟超脱世外","hasContent":1},{"id":4024939,"name":"第一百八十七章 赵与吴","hasContent":1},{"id":4032174,"name":"第一百八十八章 王超凡的奇景","hasContent":1},{"id":4033667,"name":"第一百八十九章 看吴美不美","hasContent":1},{"id":4034288,"name":"第一百九十章 对抗顶级修仙家族的后人","hasContent":1},{"id":4035306,"name":"第一百九十一章 打哭了一群天才","hasContent":1},{"id":4037333,"name":"第一百九十二章 复制佛陀的道路","hasContent":1},{"id":4038217,"name":"第一百九十三章 血染密地","hasContent":1},{"id":4196588,"name":"感谢大家!","hasContent":1},{"id":4040043,"name":"第一百九十四章 绝境蜕变","hasContent":1},{"id":4040779,"name":"第一百九十五章 王燃灯大清算","hasContent":1},{"id":4044275,"name":"第一百九十六章 狩猎超凡","hasContent":1},{"id":4048959,"name":"第一百九十七章 全灭","hasContent":1},{"id":4050033,"name":"第一百九十八章 躺赢","hasContent":1},{"id":4052498,"name":"第一百九十九章 王炸","hasContent":1},{"id":4053891,"name":"第二百章 至宝","hasContent":1},{"id":4054742,"name":"第二百零一章 列仙重奖","hasContent":1},{"id":4058194,"name":"第二百零二章 神话正在腐朽","hasContent":1},{"id":4060198,"name":"第二百零三章 最后的绚烂,绝响","hasContent":1},{"id":4061581,"name":"第二百零四章 都在做准备","hasContent":1},{"id":4063244,"name":"第二百零五章 密地之旅结束","hasContent":1},{"id":4067798,"name":"第二百零六章 战舰灭地仙","hasContent":1},{"id":4069977,"name":"第二百零七章 报答","hasContent":1},{"id":4071893,"name":"第二百零八章 修行太快","hasContent":1},{"id":4073334,"name":"第二百零九章 晚宴","hasContent":1},{"id":4078126,"name":"第二百一十章 适应与列仙相处的时代","hasContent":1},{"id":4080617,"name":"第二百一十一章 精神出窍","hasContent":1},{"id":4085172,"name":"第二百一十二章 欲猎超凡者","hasContent":1},{"id":4089544,"name":"第二百一十三章 新星第一次超凡战匆匆落幕","hasContent":1},{"id":4096561,"name":"第二百一十四章 热议与毁灭","hasContent":1},{"id":4097978,"name":"第二百一十五章 王之蔑视","hasContent":1},{"id":4099667,"name":"第二百一十六章 地仙之资","hasContent":1},{"id":4100521,"name":"第二百一十七章 盗内景","hasContent":1},{"id":4103522,"name":"第二百一十八章 分水岭级大事件","hasContent":1},{"id":4104197,"name":"第二百一十九章 超凡败了","hasContent":1},{"id":4105055,"name":"第二百二十章 大幕揭开","hasContent":1},{"id":4109995,"name":"第二百二十一章 反击超级财阀","hasContent":1},{"id":4112189,"name":"第二百二十二章 深夜惊雷","hasContent":1},{"id":4112934,"name":"第二百二十三章 投资王煊","hasContent":1},{"id":4113823,"name":"第二百二十四章 比肩古代传说","hasContent":1},{"id":4114265,"name":"第二百二十五章 风暴","hasContent":1},{"id":4115090,"name":"第二百二十六章 一夜突进八百里","hasContent":1},{"id":4118561,"name":"第二百二十七章 内鬼","hasContent":1},{"id":4119116,"name":"第二百二十八章 决战就绪","hasContent":1},{"id":4125101,"name":"第二百二十九章 牧城大战","hasContent":1},{"id":4129626,"name":"第二百三十章 先下一城","hasContent":1},{"id":4133571,"name":"第二百三十一章 躁动的夜晚","hasContent":1},{"id":4133815,"name":"第二百三十二章 决战灿烂","hasContent":1},{"id":4135301,"name":"第二百三十三章 有何不敢","hasContent":1},{"id":4137965,"name":"第二百三十四章 金刚怒目,菩萨低眉","hasContent":1},{"id":4142064,"name":"第二百三十五章 剑指孙家","hasContent":1},{"id":4142500,"name":"第二百三十六章 释迦真经","hasContent":1},{"id":4143435,"name":"第二百三十七章 形势复杂","hasContent":1},{"id":4145981,"name":"第二百三十八章 树欲静而风不止","hasContent":1},{"id":4152918,"name":"第二百三十九章 列仙有请","hasContent":1},{"id":4158647,"name":"第二百四十章 补足短板","hasContent":1},{"id":4173307,"name":"第二百四十一章 广积粮","hasContent":1},{"id":4174124,"name":"第二百四十二章 亵渎神灵","hasContent":1},{"id":4175111,"name":"第二百四十三章 屠龙开始","hasContent":1},{"id":4176001,"name":"第二百四十四章 皆大欢喜","hasContent":1},{"id":4178528,"name":"第二百四十五章 击破神话","hasContent":1},{"id":4179310,"name":"第二百四十六章 龙潭虎穴","hasContent":1},{"id":4180312,"name":"第二百四十七章 让列仙动心","hasContent":1},{"id":4180887,"name":"第二百四十八章 列仙祸","hasContent":1},{"id":4181838,"name":"第二百四十九章 母舰重启","hasContent":1},{"id":4182469,"name":"第二百五十章 先下手为强","hasContent":1},{"id":4183100,"name":"第二百五十一章 孙家秘库的真正主人","hasContent":1},{"id":4184445,"name":"第二百五十二章 剑仙死了","hasContent":1},{"id":4185048,"name":"第二百五十三章 又一条秘路","hasContent":1},{"id":4185816,"name":"第二百五十四章 神秘世界","hasContent":1},{"id":4187688,"name":"第二百五十五章 超凡回归","hasContent":1},{"id":4191002,"name":"第二百五十六章 人间变了天","hasContent":1},{"id":4193769,"name":"第二百五十七章 万法之始","hasContent":1},{"id":4196569,"name":"第二百五十八章 为超凡找出路","hasContent":1},{"id":4197178,"name":"第二百五十九章 秘库皆被占据","hasContent":1},{"id":4200762,"name":"第二百六十章 天下已无净土","hasContent":1},{"id":4201133,"name":"第二百六十一章 见仙","hasContent":1},{"id":4201911,"name":"第二百六十二章 仙人保镖","hasContent":1},{"id":4202376,"name":"第二百六十三章 天药","hasContent":1},{"id":4203115,"name":"第二百六十四章 四方云动","hasContent":1},{"id":4203578,"name":"第二百六十五章 仙血四溅","hasContent":1},{"id":4204241,"name":"第二百六十六章 给列仙上一课","hasContent":1},{"id":4205847,"name":"第二百六十七章 斩断仙命","hasContent":1},{"id":4206433,"name":"第二百六十八章 弑仙","hasContent":1},{"id":4206942,"name":"第二百六十九章 干预现世反被狩猎","hasContent":1},{"id":4207866,"name":"第二百七十章 我们是未来的你","hasContent":1},{"id":4208243,"name":"第二百七十一章 超凡世界崩塌","hasContent":1},{"id":4208843,"name":"第二百七十二章 真的出现了","hasContent":1},{"id":4209438,"name":"第二百七十三章 周围全是狠人","hasContent":1},{"id":4210126,"name":"第二百七十四章 类瘆灵","hasContent":1},{"id":4210537,"name":"第二百七十五章 要出王炸","hasContent":1},{"id":4211495,"name":"第二百七十六章 真……王炸","hasContent":1},{"id":4211975,"name":"第二百七十七章 剑劈战舰","hasContent":1},{"id":4212391,"name":"第二百七十八章 教育到明白事理","hasContent":1},{"id":4212683,"name":"第二百七十九章 仙胎","hasContent":1},{"id":4213238,"name":"第二百八十章 修为提升","hasContent":1},{"id":4213882,"name":"第二百八十一章 世间如此妖娆","hasContent":1},{"id":4214493,"name":"第二百八十二章 仙界","hasContent":1},{"id":4215260,"name":"第二百八十三章 新时代新妖怪新神仙","hasContent":1},{"id":4215945,"name":"第二百八十四章 万事俱备","hasContent":1},{"id":4216443,"name":"第二百八十五章 天血天命","hasContent":1},{"id":4216660,"name":"第二百八十六章 跃出河流改命的鱼","hasContent":1},{"id":4217109,"name":"第二百八十七章 魔胎","hasContent":1},{"id":4218038,"name":"第二百八十八章 大丰收","hasContent":1},{"id":4218567,"name":"第二百八十九章 我是郑武","hasContent":1},{"id":4219159,"name":"第二百九十章 公子无双","hasContent":1},{"id":4219665,"name":"第二百九十一章 现实世界的教祖","hasContent":1},{"id":4220343,"name":"第二百九十二章 隔绝万物","hasContent":1},{"id":4220703,"name":"第二百九十三章 终于进入老钟的书房","hasContent":1},{"id":4221361,"name":"第二百九十四章 秘典无数","hasContent":1},]},]}}

### 小说 批量下载
GET https://downbakxs.pigqq.com/BookFiles/Html/627/626698/3376535.html HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
Content-Type: application/x-www-form-urlencoded
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Host: downbakxs.pigqq.com
Connection: Keep-Alive
Accept-Encoding: gzip

{"status":1,"info":"success","data":{"id":626698,"name":"深空彼岸","cid":3376535,"cname":"第三章 续命项目","pid":3376534,"nid":3376858,"content":"\r\n　　那些老人很迫切，他们时光无多，没有岁月可以耽搁，急需研究出成果。\r\n　　所以，旧术实验班选择的都是高校学生，而非从孩童开始，前者年龄大一些，悟性更强。\r\n　　散术都出自旧土，那些组织、研究机构认为，从源头恢复旧术研究，或许是最好的选择。\r\n　　最为重要的是，既然所有神话传说等都源自旧土，这里或许有什么“神秘因子”也说不定。\r\n　　只是这种认知与绚烂的深空科技文明相悖，不能列在纸面上。\r\n　　但是，一些身份背景惊人的老人到了晚年后，似乎尤其信这些神秘学。\r\n　　他们所求的是什么？更久远的寿命，希冀从神话中挖掘，沿着前人的足迹追寻到不死之路等。\r\n　　尽管冷静时他们自己也知道，这多半是梦幻泡影，可如果时光无多，而自身又掌握有庞大的资源等，为什么不去试试呢？\r\n　　所以，旧土开始被关注，一些“研究”相继在此展开，投入大量的资金。\r\n　　人性自古相通，从秦皇开始到现在，许多人都不能免俗。\r\n　　这些年来，一些财阀中的老人一直在推动，想要获得“新生”，资助了很多研究机构。\r\n　　当然，旧术研究只是他们关注的方向之一，有实力去推动“生命变革”的人，不可能将希望只寄托在一项研究中。\r\n　　长年以来，各大财阀资助过各种基因团队、生命研究所等，有些项目已经取得惊人的进展。\r\n　　比如数种抗衰老药剂，已有了初步的成效。\r\n　　旧术研究只是他们所投资的数十个“续命项目”之一。\r\n　　其实这些“续命项目”彼此间也有交集，尤其是在投资人的干预下，有时会相互合作。\r\n　　比如，王煊他们平日的食物，补血益气，养精神，且有部分抗衰效用，其中的成分与配比等都与一家药剂研究所有关。\r\n　　旧术实验班的人平日消耗心神过重，但无论多么疲累，经过食补等配合，很快就能恢复过来。\r\n　　对于每天都在研究与演练旧术的人来说，这是福音，一段时间过后他们的体质都有明显的提升。\r\n　　此外，有些生物基因团队也希望合作，主动找上门来，想从基因方面入手，帮助实验班的人改变体质。\r\n　　其中一支基因队伍专注于线粒体的研究，通过改变端粒的长度，理论上可以达到增加寿命的效果。\r\n　　当时所有人都抵触，虽然号称是旧术实验班，但他们不是小白鼠，绝不会同意那样做。\r\n　　王煊得到消息后，险些直接退出，无论如何他都不会接受。\r\n　　他精研体术，琢磨冥想法，研究采气术等，是一个循序渐进改变体质的过程。\r\n　　在他看来，这种基因工程粗暴的改变现状，可能会留下不可弥合的隐患，与他观念不相符，非他所求。\r\n　　事实上，这项合作很快就被上面否决了，说话有分量的人开口，认为技术还不够成熟。\r\n　　事后有小道消息传出，来自新星的学生中有些人身份不简单，他们的家人不可能让他们冒险。\r\n　　同时，也是一位有背景的同学意外透露，新星那边有些“状况”，有人在旧术上练出了名堂，所以，他们这些人才赶到旧术发源地，甘愿深入参悟。\r\n　　但事后他不承认，说那些都是醉话。\r\n　　王煊觉得，他可能说漏嘴了。\r\n　　但秦诚却相信，那就是醉话，因为当天就是他灌醉了那位同学。\r\n　　王煊认为新星那边或许发现了什么，所以某些财阀的后人才会加入实验班，开始研究旧术。\r\n　　此刻明月高挂，在深秋中略带冷意。\r\n　　秦诚接了个电话，不断点头，而后转身对王煊叹道：“当年，周坤不是醉话啊，他确实说漏嘴了。”\r\n　　在电话中，他得到最新消息，新星那边近期出现的一鳞半爪的传闻，有了模糊的指向，似乎与几起神秘现象有关。\r\n　　早在三年前，那位来自新星的同学周坤就给予了他们提示！\r\n　　尽管是因为醉酒，并非他本意想告知。\r\n　　“你一定要获取一个前往新星的名额！”秦诚道，然后告别，转身离去。\r\n　　身为旧术研究班的学生，他们的宿舍区较为安静，因为平日需要冥想以及练体术等，不容打扰。\r\n　　每人都有独立的房间，且被提供由深空送来的特殊食物，可以说“旧术研究”这个项目很受重视。\r\n　　清晨，王煊起床，演练一种名为金刚拳的体术后，安静下来，开始迎着朝霞练采气术。\r\n　　按照老教授的说法，采气术、冥想、内养法等，必须精通一两种，这是旧术根之所在，力量的源头。\r\n　　体术，比如形意、金刚等，都是根之上的枝叶，唯有根系强，才能枝繁叶茂。\r\n　　王煊自然无比重视，对所有“根法”都有涉猎，后来更是有选择的精研。\r\n　　校园这片区域大树较多，草坪上满是黄叶，此时很宁静。\r\n　　王煊闭着眼睛，沐浴朝霞，他在采气，结合内养法，心中想象着接引来一缕又一缕金色霞光，将自己淹没。\r\n　　虽是内养法，存想于心中，但他的身体似乎真的发热了，感觉像是被金色光焰缭绕着。\r\n　　如有人在附近，一定能看出王煊身上的一些异常，他身上的朝霞比别人“浓郁”，像是有一层火光在流动。\r\n　　王煊一边采气，一边动用内养法，虽然只是在心中存想接引金霞的样子，但现实中似乎真的在发生。\r\n　　他周身滚热，最后更是酥酥麻麻，有一股劲力在身上钻，先是酸痛，而后又觉得很舒服。\r\n　　他这种异样的感受，是在近期才出现的。\r\n　　王煊知道，由于常年练采气术，并结合内养法，他现在开始“收获”。\r\n　　昨天夜里，他的右手猛力按下去，直接在粗大而坚硬的树干上留下清晰的手印，就是“根法”逐渐有成的体现。\r\n　　在旧术这条路上，他有了长足的进步。\r\n　　实验班中，秦诚、周坤等人虽然也都在练旧术，但大多都只是体质提升了，像王煊这般采气入体，内养己身，算是仅有。\r\n　　秦诚、周坤等如果对上普通人的话，一个人能对抗十几人没问题。\r\n　　常年练旧术以及长期服食稀珍药膳，让他们的身体素质提升了一大截。\r\n　　王煊在没有采气前，就已经比同窗强很多。\r\n　　所以，秦诚一直为他鸣不平，如果单以旧术对抗的话，根本没有人能够与王煊并论。\r\n　　甚至，他仅动用一只手，应该就可以压制旧术实验班中的任何一位同学。\r\n　　王煊身体滚热，到了后来甚至有些发烫了，从血肉到骨骼，似有一道道细小的电流在经过。\r\n　　这是采气、内养有了一定火候的体现。\r\n　　王煊在心中存想一缕缕朝霞进入身体，而后又存想体内有黑色浊雾自体表散发出去。\r\n　　以此对应，他的身体出现异常，新陈代谢加快，身上排出一些黏糊糊的汗液，湿漉漉。\r\n　　他觉得，血肉像是在被朝霞洗礼，内外澄净，精气神异常充沛，全身充满了力量。\r\n　　清晨的阳光穿过树林，让几缕薄雾都带上淡金色彩，四名年轻男女散步走来，两名男子只是偶尔说上一两句话，主要是两名女子在谈论着什么。\r\n　　其中一名女子非常靓丽，一直在说话，不时发出笑声，一看就是活泼跳脱的性格。\r\n　　另外一名女子很柔美，有种书香气韵，带着温和的笑。\r\n　　他们也是旧术实验班的学生，来自新星。\r\n　　“你们看，那不是王煊吗，他的身体怎么像是在发光？”青春活力十足的那个女子开口，漂亮的眼睛睁得很大，怀疑自己是否看错了。\r\n　　那个有些文静的女子讶然：“他该不会练成采气术了吧？”\r\n　　两位男子中的一人很吃惊：“实验班中……竟然真的有人练成了！”\r\n　　但很快他又摇了摇头，因为他知道，现在这些已经失去意义。\r\n　　另一名男子也开口：“可惜，旧时代的术终究是过时了，现在被正式放弃了，不久后我们就要回新星了，那边又有了新发现，把握住机会，新的时代可能要来了。”\r\n　　几人来自新星，都了解最新内情，旧术被认为过时了，已经被抛弃，现在有了更好的选择！\r\n　　恍若隔世的感觉，规则都变了，新书期间就可以投月票了，请大家支持下吧。\r\n　　下午、晚上还有章节。\r\n　　\f\t\n","hasContent":1}}

### 小说 女生版 banner
GET https://scxs.pigqq.com/prov8/base/banner_lady.html HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
Content-Type: application/x-www-form-urlencoded
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Host: scxs.pigqq.com
Connection: Keep-Alive
Accept-Encoding: gzip

{
  "status": 1,
  "info": "",
  "data": [
  {
      "type": "book",
      "param": "427365",
      "imgurl": "https://imgapixs.pysmei.com/shudan/images/427365.jpg"
    },
  {
      "type": "book",
      "param": "557381",
      "imgurl": "https://imgapixs.pysmei.com/shudan/images/557381.jpg"
    },
    {
      "type": "book",
      "param": "620406",
      "imgurl": "https://imgapixs.pysmei.com/shudan/images/620406.jpg"
    }
  ]
}

### 小说 女生版 书城
GET https://scxs.pigqq.com/prov8/base/lady2.html HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
Content-Type: application/x-www-form-urlencoded
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Host: scxs.pigqq.com
Connection: Keep-Alive
Accept-Encoding: gzip

{
	"status": 1,
	"info": "success",
	"data": [{
		"Category": "热门连载",
		"ChangeFlag": "no",
		"More": "https://scxs.pysmei.com/top/lady/top/hot/week/{page}.html",
		"MoreFlag": "api",
		"NavIcon": "hhttps://scmh.pysmei.com/pubimgs/recommend5.png",
		"ViewType": "1r3c3c",
		"Books": [{
			"Id": 613928,
			"Name": "今天大佬也不想开门",
			"Area": null,
			"AreaCodde": "",
			"Author": "二谦",
			"Img": "jintiandalaoyebuxiangkaimen.jpg",
			"HostKey": "",
			"Desc": "星际最火的论坛上有一个大热话题：\r\n\r\n 你身边发生的最不可思议的事情是什么？\r\n\r\n 春眠：谢邀，人在家中坐，门从天上来。\r\n\r\n 生活就像是一扇紧闭的大门，\r\n\r\n 在打开之前，你永远也不知道，\r\n\r\n 你将面对的是：\r\n\r\n 一个大活人或是四十米大长刀！\r\n\r\n （快穿，无CP）",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "科幻灵异",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "8.0"
		}, {
			"Id": 591952,
			"Name": "夫人她马甲又轰动全城了",
			"Area": null,
			"AreaCodde": "",
			"Author": "灵小哥",
			"Img": "furentamajiayouhongdongquanchengle.jpg",
			"HostKey": "",
			"Desc": "乔念在乔家生活了18年，亲生父母找上门来，一时之间，绕城豪门都知道乔家出了个假千金！\r\n\r\n 真千金多才多艺，温柔善良。\r\n\r\n 假千金不学无术，一事无成。\r\n\r\n 所有人都想看她被赶出豪门后，回到山沟沟过得有多惨！\r\n\r\n 乔念也以为自己亲生父母来自漯河县，是个一穷二白的穷老师。\r\n\r\n 谁知道哥哥开的车是辉腾，裸车300万！\r\n\r\n 亲爸教书的地方在清大，老师还有个别称是教授！\r\n\r\n 渣渣们一家跪",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "女生频道",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "7.8"
		}, {
			"Id": 580372,
			"Name": "首辅娇娘",
			"Area": null,
			"AreaCodde": "",
			"Author": "偏方方",
			"Img": "shoufujiaoniang.jpg",
			"HostKey": "",
			"Desc": "本是侯府千金，却因出生时抱错沦为农家女。\r\n\r\n 好不容易长到如花似玉的年纪，却无人上门娶她。\r\n\r\n 说她容颜丑陋，天生痴傻，还是克父克母的小灾星？\r\n\r\n 可她半路捡来的夫君，是未来首辅。\r\n\r\n 她上山领养的小和尚，是六国神将。\r\n\r\n 就连随手救下的老太太，竟然也是当朝太后。\r\n\r\n 某男恶狠狠道：“娘子，谁敢欺负你，为夫把他办了！”\r\n\r\n 神将道：“姐",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "女生频道",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "8.3"
		}, {
			"Id": 560185,
			"Name": "全能千金燃翻天",
			"Area": null,
			"AreaCodde": "",
			"Author": "德音不忘",
			"Img": "quannengqianjinranfantian.jpg",
			"HostKey": "",
			"Desc": "【本文爽爽爽，强强强！男主妻管严，女主第一美，虐渣+宠文】\r\n\r\n 异世界科技大佬叶灼重生了。\r\n\r\n 重生成豪门假千金。\r\n\r\n 假千金鸠占鹊巢，在圈子里人人厌恶，臭名昭著，不但是大字不识几个的草包，还是个见不得光的私生女。\r\n\r\n 被人嘲讽：“连真千金的小拇指都比不上！”\r\n\r\n “私生女！不要脸！”\r\n\r\n 对此，叶大佬轻笑一声。\r\n\r\n 呵呵......",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "女生频道",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "8.8"
		}, {
			"Id": 533696,
			"Name": "公主她在现代星光璀璨",
			"Area": null,
			"AreaCodde": "",
			"Author": "一船梦",
			"Img": "gongzhutazaixiandaixingguangcuican.jpg",
			"HostKey": "",
			"Desc": "（甜宠，古穿今，公主重生征服娱乐圈文）\r\n\r\n 于乱世中将众弟妹抚养长大，文能招聚天下贤士，武能挂帅出征开拓疆土。\r\n\r\n 终于一步步将胞弟送上皇帝位置的夏挽沅，是夏朝历史上最为传奇的长公主。\r\n\r\n 而这位长公主一睁眼，却发现自己身处千年以后。\r\n\r\n 老公儿子都有了，还有不争气的弟弟妹妹。\r\n\r\n 只不过老公把她当空气，儿子与她无交集。\r\n\r\n 这回自己倒是依然被称为“公主”，但都是别人讽刺她在娱乐圈仗着",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "女生频道",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "8.9"
		}, {
			"Id": 398795,
			"Name": "八零甜妻萌宝宝",
			"Area": null,
			"AreaCodde": "",
			"Author": "席祯",
			"Img": "balingtianqimengbaobao.jpg",
			"HostKey": "",
			"Desc": "【重生甜宠：肤白貌美软妹纸，发家致富养包子】\r\n\r\n 随珠的抽奖系统老牛逼了，不仅送她海岛度假全装备，还在空难时送她回了过去，成了嗷嗷待哺奶娃儿的娘，娃爹名叫——父不详！！！\r\n\r\n 身处小渔村，磨刀霍霍向……海洋！\r\n\r\n 星际牌万能鱼竿不用饵就能钓大龙虾；多功能防护服升级后能潜水找沉船……\r\n\r\n 系统带她发家致富；系统带她逆袭人生；\r\n\r\n 系统带她……儿砸喂！找你爹就算了，咱娘俩相依为命挺好的！",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "女生频道",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "8.8"
		}, {
			"Id": 257206,
			"Name": "嘉平关纪事",
			"Area": null,
			"AreaCodde": "",
			"Author": "浩烨乐",
			"Img": "jiapingguanjishi.jpg",
			"HostKey": "",
			"Desc": "一场尘封十年的旧事，让嘉平关城笼罩在阴霾之下，家国之情、兄弟之谊、恋人之爱该如何取舍，面对家国安危，众人的命运又该何去何从......",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "女生频道",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "6.0"
		}]
	}, {
		"Category": "抖音热书",
		"ChangeFlag": "no",
		"More": "https://scxs.pysmei.com/top/lady/top/collect/week/{page}.html",
		"MoreFlag": "api",
		"NavIcon": "https://scmh.pysmei.com/pubimgs/recommend5.png",
		"ViewType": "3c3c",
		"Books":  [{
			"Id": 626635,
			"Name": "绝世葫宝要翻天",
			"Area": null,
			"AreaCodde": "",
			"Author": "叶楚月夜墨寒",
			"Img": "jueshihubaoyaofantian.jpg",
			"HostKey": "",
			"Desc": "叶楚月，神武帝国臭名昭著的痴傻丑女，与人“苟且”，生下野孩子。未婚夫成亲之日，身穿喜袍从城墙跳下，为情而死。美眸初睁，来自21世纪的古武门主将掀起血雨腥风，一雪前耻！废物？素手撼帝国，乾坤足下踏！痴傻？运筹帷幄，决胜千里外。野孩子？帝尊之子，天皇血脉，放眼八荒谁敢放肆？“娘亲，外面有个俊俏的大哥哥，说是我的爹爹。”“让他带着钱到后面排队去。”某日，帝尊大人邪魅一笑：听说，你到处跟人说我死了？",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "女生频道",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "6.0"
		}, {
			"Id": 626577,
			"Name": "九公主她又美又飒",
			"Area": null,
			"AreaCodde": "",
			"Author": "拈花惹笑",
			"Img": "jiugongzhutayoumeiyousa.jpg",
			"HostKey": "",
			"Desc": "新婚夜，被夫君亲手掐死，还被下令埋了？楚倾歌睁眼，天下风云为之变色！来自二十一世纪的强悍灵魂，她是鬼医，是药神，是谋师，是战部史上最年轻最貌美的总指挥官！前世权谋诡计，她被最信任的人背叛，今生穿越成废物九公主，原只想安安静静过一生。奈何朝堂风起云涌，步步惊心，招招夺命！既然世人不允许她平凡，那就将这万里河山，狠狠踩在脚下！",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "女生频道",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "6.0"
		}, {
			"Id": 622324,
			"Name": "霍太太是隐形大佬",
			"Area": null,
			"AreaCodde": "",
			"Author": "舒情霍云城",
			"Img": "huotaitaishiyinxingdalao.jpg",
			"HostKey": "",
			"Desc": "传闻，霍少的未婚妻是乡下长大的，长得很丑，没有学问，跟个草包一样。宴会上，舒情露面，众人纷纷都惊了！“这哪里丑了！”“据说影帝是她小弟！”“她爹是世界第一首富！”“神秘的loe服装设计师就是她！”一个个马甲掉光，众人都惊呆了，不过那又怎样，霍云城又不喜欢她。当天，霍氏集团官方发了条微博。“感情很好，即将准备结婚。”众人：“……”！！！",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "女生频道",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "6.0"
		}, {
			"Id": 619494,
			"Name": "重生毒妃娇又甜",
			"Area": null,
			"AreaCodde": "",
			"Author": "苏洛江殊",
			"Img": "zhongshengdufeijiaoyoutian.jpg",
			"HostKey": "",
			"Desc": "凄凉惨死后，苏洛才知道身边谁是人，谁是鬼！重活一世，她发誓绝不放过那对狗男女，顺带抱紧前夫大腿。可说好的协议夫妻，不近女色呢？----某世子每日必三省：夫人在哪里？夫人今天有没有更爱我？夫人什么时候才跟我造娃娃？“世子，夫人今天生气，摔了一对镯子！”“带夫人去库房，让她摔到高兴为止！”“世子，夫人今天又闯祸了！”“谁敢惹她？”",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "女生频道",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "6.0"
		}, {
			"Id": 619389,
			"Name": "重生之嫡女美又帅气",
			"Area": null,
			"AreaCodde": "",
			"Author": "白卿言萧容衍",
			"Img": "zhongshengzhidinvmeiyoushuaiqi.jpg",
			"HostKey": "",
			"Desc": "前世，镇国公府，一朝倾塌灰飞烟灭。此生，嫡长女白卿言重生一世，绝不让白家再步前世后尘。白家男儿已死，大都城再无白家立锥之地？大魏国富商萧容衍道：百年将门镇国公府白家，从不出废物，女儿家也不例外。后来……白家大姑娘，是一代战神，成就不败神话。白家二姑娘，是朝堂新贵忠勇侯府手段了得的当家主母。白家三姑娘，是天下第二富商，翻手为云覆手为雨的商界翘楚",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "女生频道",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "6.0"
		}, {
			"Id": 614101,
			"Name": "退婚后她成了真祖宗",
			"Area": null,
			"AreaCodde": "",
			"Author": "病娇猫娘",
			"Img": "tuihunhoutachenglezhenzuzong.jpg",
			"HostKey": "",
			"Desc": "苏家的废物千金苏也，被薄氏集团总裁退婚后疯了！\r\n\r\n 第一天，她摸着父亲的头：“大侄子，我看好一个项目，明天你去竞标。”\r\n\r\n 第二天，她用铁锹把苏家祖坟刨了，嘴里念叨：“我记着是埋在这了呀？”\r\n\r\n 第三天，她拍了拍某洁癖总裁的肩旁：“小薄啊，联姻不成情意还在，这服药我给你打一折，你就给我600万吧。”\r\n\r\n *\r\n\r\n 苏也，40年前死于非命的商界第一女枭雄，机缘巧合重生到同名侄孙女身上",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "女生频道",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "6.0"
		}]
	}, {
		"Category": "高分神作",
		"ChangeFlag": "no",
		"More": "https://scxs.pysmei.com/top/lady/top/vote/week/{page}.html",
		"MoreFlag": "api",
		"NavIcon": "https://scmh.pysmei.com/pubimgs/recommend5.png",
		"ViewType": "3c3c",
		"Books": [{
			"Id": 613369,
			"Name": "分手后我在娱乐圈爆红了",
			"Area": null,
			"AreaCodde": "",
			"Author": "蓝白格子",
			"Img": "fenshouhouwozaiyulequanbaohongle.jpg",
			"HostKey": "",
			"Desc": "洛柠是一本娱乐圈团宠文里的炮灰女配，重来一次，这炮灰她不当了！\r\n\r\n 黑粉叫嚣：“洛柠就是个花瓶，唱歌跳舞演戏干啥啥不行，天天捆绑顶流蹭热度第一名，除了颜值一无是处。”\r\n\r\n 后来当唱歌跳舞俱佳，会琴棋书画、野外求生、烹饪美食，还会画符看相，长得美智商高，演技更是爆表的洛柠出现在大众面前时。\r\n\r\n 黑粉真香：“姐姐，我可以！！！”\r\n\r\n 突然有一天热搜爆了。\r\n\r\n 神秘影帝陆洵亲吻",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "女生频道",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "9.5"
		}, {
			"Id": 606117,
			"Name": "穿书后大佬每天都在崩剧情",
			"Area": null,
			"AreaCodde": "",
			"Author": "浮生若朝露",
			"Img": "chuanshuhoudalaomeitiandouzaibengjuqing.jpg",
			"HostKey": "",
			"Desc": "满级大佬林止风在大战中一着不慎，神格被封印到小说世界，正愁穿书消耗大，不明真相的系统就送上门。\r\n\r\n 结果，居然要她穿成悲情角色，完成角色的圣母使命？\r\n\r\n 系统：请宿主用包容的心热爱每一个世界，终有一天，所有恶毒角色都会被你感化。\r\n\r\n 林止风：呵呵，我选择为所欲为。\r\n\r\n 宽容善良？不可能的！\r\n\r\n 忍辱负重？不存在的！\r\n\r\n 只有打劫系统、有仇马上就报、崩坏圣母剧情才是她的风格。\r\n\r\n 一言",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "女生频道",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "8.7"
		}, {
			"Id": 602178,
			"Name": "致命偏宠",
			"Area": null,
			"AreaCodde": "",
			"Author": "漫西",
			"Img": "zhimingpianchong.jpg",
			"HostKey": "",
			"Desc": "黎家团宠的小千金黎俏，被退婚了。\r\n\r\n 黎家人揭竿而起，全城讨伐，誓要对方好看。\r\n\r\n *\r\n\r\n 后来，黎俏偶遇退婚男的大哥。\r\n\r\n 有人说：他是南洋最神秘的男人，姓商，名郁，字少衍；\r\n\r\n 也有人说：他傲睨万物，且偏执成性，是南洋地下霸主，不可招惹。\r\n\r\n 绵绵细雨中，黎俏望着杀伐野性的男人，浅浅一笑：“你好，我是黎俏。”\r\n\r\n 做不成夫妻，那就做你长嫂。\r\n\r\n *\r\n\r\n 几个月后，街头相遇，退",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "女生频道",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "9.6"
		}, {
			"Id": 557381,
			"Name": "如意事",
			"Area": null,
			"AreaCodde": "",
			"Author": "非10",
			"Img": "ruyishi.jpg",
			"HostKey": "",
			"Desc": "许明意再次睁开眼睛的时候，回到了十六岁身患怪病的那一年。\r\n\r\n 这时，她那老当益壮的祖父正值凯旋归京——“路上救下的这位年轻人长得颇好，带回家给孙女冲喜再合宜不过。”\r\n\r\n 于是，昏迷中被安排得明明白白的定南王世孙就这么被拐回了京城……",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "女生频道",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "9.6"
		}, {
			"Id": 541089,
			"Name": "被大佬们团宠后我野翻了",
			"Area": null,
			"AreaCodde": "",
			"Author": "苏闲佞",
			"Img": "beidalaomentuanchonghouwoyefanle.jpg",
			"HostKey": "",
			"Desc": "【【‘婚恋文’新媒体向征文大奖赛】参赛作品】\r\n\r\n 重生醒来，她成了被亲哥们送进疯人院的小可怜。亲哥们只疼当年被抱错的假千金‘妹妹’，对她百般厌恶。\r\n\r\n 于是裴允歌作天作地，收拾假千金，等着他们叫她滚。\r\n\r\n 可哥哥们态度诡异。\r\n\r\n 秦总冷笑，“我妹砸店？来，给我把商场买下来，让我妹砸！”\r\n\r\n 秦影帝挑眉，“她送上门潜规则？那我这个哥哥是死了吗？”\r\n\r\n 秦神脸黑，“你三番两次耍心机欺负歌儿",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "女生频道",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "8.6"
		}, {
			"Id": 473048,
			"Name": "星际破烂女王",
			"Area": null,
			"AreaCodde": "",
			"Author": "柳升升",
			"Img": "xingjipolannvwang.jpg",
			"HostKey": "",
			"Desc": "穿越到星际时代的一颗垃圾星上面，季柚穷得都快要刨土吃了，可……这里土有毒不能吃……没办法，她只能放低身段去捡捡垃圾，卖卖破烂啥的……\r\n\r\n 比如这么漂亮的草籽果然竟没人要，捡起来车个珠子，能挂网上卖。\r\n\r\n 可一挂上网，就有人打差评：“草籽果都拿来卖，想钱想疯了吧？”\r\n\r\n 数日后，这人就后悔的直捶墙：“跪求卖我一个颗草籽果，就一颗！一颗就好了。”\r\n\r\n 季柚高冷道：“不卖！”\r\n\r\n 再比",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "女生频道",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "9.1"
		}]
	}, {
		"Category": "微信热书",
		"ChangeFlag": "no",
		"More": "https://scxs.pysmei.com/top/lady/top/commend/week/{page}.html",
		"MoreFlag": "api",
		"NavIcon": "https://scmh.pysmei.com/pubimgs/recommend5.png",
		"ViewType": "3c3c",
		"Books": [{
			"Id": 617962,
			"Name": "总裁追妻休要逃",
			"Area": null,
			"AreaCodde": "",
			"Author": "沈蔓歌叶南弦",
			"Img": "zongcaizhuiqixiuyaotao.jpg",
			"HostKey": "",
			"Desc": "一场大火烧掉了沈蔓歌对叶南弦所有的爱。五年后她华丽回归，势必为当年的自己讨回一个公道。却没想到带回来的小正太比她更有手段。某宝站在叶南弦面前，很无辜的说：“叔叔帮我一个忙可以吗？求你了。”叶南弦觉得无法抵挡这孩子的恳求，蹲下身子打算帮忙，却没想到被喷了一脸。某天，叶南弦对着小正太说：“臭小子，这是我的房间！”“可是我想跟妈咪睡，我们都睡了五年了。”某男人泪奔……追个妻子回来而已，为什么儿子如此难搞",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "女生频道",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "6.0"
		}, {
			"Id": 602096,
			"Name": "顾少的独家挚爱",
			"Area": null,
			"AreaCodde": "",
			"Author": "白雅顾凌峰",
			"Img": "gushaodedujiazhiai.jpg",
			"HostKey": "",
			"Desc": "她在逃跑途中，和神秘男人扯上关系。没想到他居然是高高在上，冷酷腹黑，且不近女色的顾凌擎……",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "都市言情",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "6.0"
		}, {
			"Id": 602075,
			"Name": "一胎双宝：总裁大人请克制",
			"Area": null,
			"AreaCodde": "",
			"Author": "宁浠战北爵",
			"Img": "yitaishuangbao：zongcaidarenqingkezhi.jpg",
			"HostKey": "",
			"Desc": "家道中落，为了拯救入狱的父亲，她不得已献身未婚夫，不料误惹神秘总裁，十月怀胎，生下一对可爱的双胞胎！\\n四年后，她携子归来，却被他抵在墙角——\\n“带着我的孩子逃了这么久，终于舍得出现了？”",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "都市言情",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "6.0"
		}, {
			"Id": 563829,
			"Name": "替嫁新娘:亿万老公宠上天",
			"Area": null,
			"AreaCodde": "",
			"Author": "琉璃雪雪",
			"Img": "563829.jpg",
			"HostKey": "",
			"Desc": "主角夏夕绾陆寒霆一场阴谋，她从乡下被接回，替嫁给他冲喜。貌丑无盐，医学废才？且看她如何妙手回春，绝丽风姿！脸被打肿的海城名媛们向他告状，陆少…等等，她嫁的竟然是只手遮天的商界巨子，她扑过去抱紧他的大腿，老公，你不是快不行了么？他一副要吃了她的表情，看来我要身体力行让你看看我究竟行不行！",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "女生频道",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "6.0"
		}, {
			"Id": 522370,
			"Name": "隐婚总裁:女人,这次来真的",
			"Area": null,
			"AreaCodde": "",
			"Author": "卡卡西",
			"Img": "522370.jpg",
			"HostKey": "",
			"Desc": "因为妹妹的嫉妒，封筱筱被设计和陌生男人春风一度……走投无路的时候，聂铮将她捡回了家。聂铮需要一个妻子，而她需要一个安生之处。他们的婚姻各取所需，封筱筱并不委屈。四年协议婚期一到，男人递给她一纸离婚协议。签字离婚后，封筱筱才知道，她小心翼翼、战战兢兢的那几年不过是场笑话！求助：离婚后前夫纠缠不休怎么办？在线等，挺急的！聂铮：“老婆，没有你我睡不着。”封筱筱跳脚：“我们已经离婚了！”聂铮检讨：“我算计",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "女生频道",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "6.0"
		}, {
			"Id": 465061,
			"Name": "跟乔爷撒个娇",
			"Area": null,
			"AreaCodde": "",
			"Author": "罗衣对雪",
			"Img": "genqiaoyesagejiao.jpg",
			"HostKey": "",
			"Desc": "京城出了大新闻：乔爷养了十二年的小媳妇跑了，跑了！连儿子都不要了！\r\n\r\n 一时间流言四起：听说是乔爷腹黑又高冷、婚后生活不和谐；听说是小媳妇和别人好上了；听说是儿子太丑。\r\n\r\n 某天，小奶娃找到了叶佳期，委屈巴巴：“七七，爸爸说我是宠物店买的。”\r\n\r\n “宠物店怎么能买到这么漂亮的儿子。”叶佳期呵呵笑，“明明是……摸奖中的。”\r\n\r\n 小奶娃望天：“……”\r\n\r\n 某禽兽眯起眼睛：“我喜欢天天",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "女生频道",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "6.0"
		}]
	}, {
		"Category": "豆瓣高分",
		"ChangeFlag": "no",
		"More": "https://scxs.pysmei.com/top/lady/top/new/week/{page}.html",
		"MoreFlag": "api",
		"NavIcon": "https://scmh.pysmei.com/pubimgs/recommend5.png",
		"ViewType": "1r3c3c",
		"Books":  [{
			"Id": 597016,
			"Name": "锦衣玉令",
			"Area": null,
			"AreaCodde": "",
			"Author": "姒锦",
			"Img": "jinyiyuling.jpg",
			"HostKey": "",
			"Desc": "时雍上辈子为了男人肝脑涂地，拼到最后得了个“女魔头”的恶名惨死诏狱，这才明白穿越必有爱情是个笑话。\r\n\r\n 重生到阿拾身上，她决定做个平平无奇的女差役混吃等死。\r\n\r\n 可从此以后，\r\n\r\n 锦衣卫大都督靠她续命。\r\n\r\n 东厂大太监叫她姑姑。\r\n\r\n 太子爷是她看着长大的。\r\n\r\n 一桩桩诡案奇案逼她出手。\r\n\r\n 这该死的人设，非让她做残暴无情的绝代妖姬？\r\n\r\n 【小剧场】\r\n\r\n 时雍露胳膊露小脚丫，人说：",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "女生频道",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "7.8"
		}, {
			"Id": 591096,
			"Name": "墨桑",
			"Area": null,
			"AreaCodde": "",
			"Author": "闲听落花",
			"Img": "mosang.jpg",
			"HostKey": "",
			"Desc": "心狠手辣的李桑柔，遇到骄横跋扈的顾睎，就象王八看绿豆……",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "女生频道",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "9.0"
		}, {
			"Id": 586407,
			"Name": "他从地狱里来",
			"Area": null,
			"AreaCodde": "",
			"Author": "顾南西",
			"Img": "tacongdiyulilai.jpg",
			"HostKey": "",
			"Desc": "有严重的共情障碍、轻微的述情障碍，趋近于0度负面p型人格，与罪犯只差了一条道德线。\r\n\r\n 这是心理医生对戎黎的诊断。\r\n\r\n 有人见过他满手是血的样子，有人见过他在枪林弹雨里抽烟的样子，也有人见过他漠然冰冷地踩着残肢断臂从火光里走来的样子。\r\n\r\n 这些人都说，戎黎是个恶魔。\r\n\r\n 但只有徐檀兮见过他因为夜盲而跌跌撞撞的样子，见过他发起床气的样子，见过他落地成盒后踢桌子的样子，见过他趴在她肩上",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "女生频道",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "8.5"
		}, {
			"Id": 582114,
			"Name": "藏珠",
			"Area": null,
			"AreaCodde": "",
			"Author": "云芨",
			"Img": "zangzhu.jpg",
			"HostKey": "",
			"Desc": "云芨最新作品《藏珠》将于7月22日在起点发布。",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "女生频道",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "8.0"
		}, {
			"Id": 520289,
			"Name": "席爷每天都想官宣",
			"Area": null,
			"AreaCodde": "",
			"Author": "公子安爷",
			"Img": "xiyemeitiandouxiangguanxuan.jpg",
			"HostKey": "",
			"Desc": "【宠文、无虐、女强、团宠！】\r\n\r\n 阮柒爆红之后。\r\n\r\n 黑粉：再漂亮也没文化。\r\n\r\n 当天下午，华夏最高等学府发博——介绍一下，我院最年轻博士生导师，阮柒教授。\r\n\r\n 黑粉：炒学霸人设有什么用？最后也得向金主低头。\r\n\r\n 第二天，阮柒现身国际经济会议，名牌落款——柒木制药集团董事长。\r\n\r\n 黑粉：赚这么多钱，也不知道为国家做点贡献。\r\n\r\n 三天后，官方发布新闻——最新型核潜艇问世，感谢总",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "女生频道",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "9.4"
		}, {
			"Id": 510236,
			"Name": "全能大佬又被拆马甲了",
			"Area": null,
			"AreaCodde": "",
			"Author": "兜兜有铜钱",
			"Img": "quannengdalaoyoubeichaimajiale.jpg",
			"HostKey": "",
			"Desc": "【双强双洁互宠扒马，男帅女拽】\r\n\r\n 听闻帝国墨爷的太太是个不学无术的小霸王，各路人马暗中看笑话。\r\n\r\n 学习垃圾？陆眠甩出理科状元的高考成绩单。\r\n\r\n 没有才艺？陆眠一手弹琴一手作画，现场表演一心二用。\r\n\r\n 只会败家？两天净赚一个小目标了解下。\r\n\r\n 拳击、围棋、鉴宝、赛车……来来来，比个够。\r\n\r\n 斯文的萧祁墨扶着眼镜，引以为傲：“谁还有话说？”\r\n\r\n 下属小心翼翼的举起手：“墨爷，",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "女生频道",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "8.4"
		}, {
			"Id": 325270,
			"Name": "穿越星际：妻荣夫贵",
			"Area": null,
			"AreaCodde": "",
			"Author": "一见我珍",
			"Img": "chuanyuexingji：qirongfugui.jpg",
			"HostKey": "",
			"Desc": "穿越到以武为尊的未来星际，为了避开勾心斗角，罗碧隐瞒了自己觉醒异能的事。\r\n\r\n 谁知有人不长眼非要找事，堂妹先是抢她的未婚夫，接着还想抢属于她的东西。罗碧一怒之下跑去测试，结果吓人一跳······",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "女生频道",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "9.2"
		}]
	}, {
		"Category": "完本精选",
		"ChangeFlag": "no",
		"More": "https://scxs.pysmei.com/top/lady/top/over/week/{page}.html",
		"MoreFlag": "api",
		"NavIcon": "https://scmh.pysmei.com/pubimgs/recommend5.png",
		"ViewType": "3c3c",
		"Books": [{
			"Id": 624847,
			"Name": "你是我的城池营垒",
			"Area": null,
			"AreaCodde": "",
			"Author": "沐清雨",
			"Img": "nishiwodechengchiyinglei.jpg",
			"HostKey": "",
			"Desc": "【全文更新完毕，锁章与正文无关，不影响阅读】\r\n\r\n 【即将连载《星火微芒》预收已开，专栏可见】\r\n\r\n 如果你确定，如果我决定，没有什么可以阻挡我走向你。\r\n\r\n 初相见，她是绑匪利刃之下的孱弱少女，他是破除困局的制胜筹码。\r\n\r\n 一场迅捷有效的营救，一双坚强有力的臂膀，让她永远记住了那抹军绿色。\r\n\r\n 再相遇，他在他的世界金戈铁马，她为她的信念攻城略地。\r\n\r\n 身为少校教官，",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "女生频道",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "8.7"
		}, {
			"Id": 580422,
			"Name": "四界柳楚传",
			"Area": null,
			"AreaCodde": "",
			"Author": "青木北恒",
			"Img": "sijieliuchuchuan.jpg",
			"HostKey": "",
			"Desc": "“妖女战神”楚灵犀绝境重生，与“废柴上仙”柳芽灵躯合体，以女二人设，上演女一大戏，可在魔界为后，能在妖界称帝，敢与仙界为敌，闲去人间闯祸，纵横四界，肆意畅快。",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "玄幻奇幻",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "6.0"
		}, {
			"Id": 567739,
			"Name": "团宠小可爱成了满级大佬",
			"Area": null,
			"AreaCodde": "",
			"Author": "安向暖",
			"Img": "tuanchongxiaokeaichenglemanjidalao.jpg",
			"HostKey": "",
			"Desc": "【【云起书院“我们的2020”创意征文大赛】参赛作品】\r\n\r\n //一屋两人三餐四季小甜饼//\r\n\r\n 【1】\r\n\r\n 娱乐圈著名花瓶相宜，一场车祸之后，突然宣布：自个儿要回家种田了。\r\n\r\n 众黑粉：嘻嘻，活该。\r\n\r\n 翌日，星辰APP开始直播相宜的田园生活。\r\n\r\n 咦，顶尖律师为什么来吃饭了？\r\n\r\n 咦，医学博士为什么来养鸡了？\r\n\r\n 咦，知名设计师为什么来染布了？\r\n\r\n 咦，电竞大神为什么来装秋千了",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "女生频道",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "9.2"
		}, {
			"Id": 508561,
			"Name": "失业后我回去继承亿万家产",
			"Area": null,
			"AreaCodde": "",
			"Author": "一米小白",
			"Img": "shiyehouwohuiqujichengyiwanjiachan.jpg",
			"HostKey": "",
			"Desc": "当红小花罗俏因疑似倒贴顶流而被对方女友粉疯狂辱骂了三个月，人气骤降，终于在娱乐圈混不下去了。\r\n\r\n 网友们纷纷表示喜闻乐见。\r\n\r\n 然而不久后，那些黑过她的明星爱豆导演突然发现本该回家种地的罗俏重新站到了他们面前。\r\n\r\n 罗·超级有钱大佬·俏，微笑：乖，你们现在可以称呼我为……甲方爸爸。\r\n\r\n 本书又名#我只想当小明星你们却非逼着我当大佬#",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "女生频道",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "9.2"
		}, {
			"Id": 368091,
			"Name": "全球高考",
			"Area": null,
			"AreaCodde": "",
			"Author": "木苏里",
			"Img": "quanqiugaokao.jpg",
			"HostKey": "",
			"Desc": "全球大型高危险性统一考试，简称全球高考。真身刷题，及格活命。考制一月一改革，偶尔随机。\r\n\r\n 梗概：两位大佬对着骚。\r\n\r\n 1v1，HE，通篇鬼扯。",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "女生频道",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "9.2"
		}, {
			"Id": 227435,
			"Name": "乘鸾",
			"Area": null,
			"AreaCodde": "",
			"Author": "云芨",
			"Img": "chengluan.jpg",
			"HostKey": "",
			"Desc": "天下玄士之首，方为命师。\r\n\r\n 七十年后的命师明微，为救师父回到永嘉十八年。\r\n\r\n 从此，这个世界的玄门就没规矩了……\r\n\r\n 诸君：阁下何不乘风起，扶摇直上九万里。\r\n\r\n 明微：正有此意。",
			"BookStatus": null,
			"LastChapterId": null,
			"LastChapter": null,
			"CName": "女生频道",
			"HitCount": null,
			"CollectCount": null,
			"CommendCount": null,
			"UpdateTimeForChapterContent": null,
			"UpdateTime": null,
			"FirstChapterId": null,
			"Score": "8.2"
		}]
	}]
}

### 小说 推荐周榜
GET https://scxs.pigqq.com/top/man/top/commend/week/1.html HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
Content-Type: application/x-www-form-urlencoded
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Host: scxs.pigqq.com
Connection: Keep-Alive
Accept-Encoding: gzip

{"status":1,"info":"success","data":{"BookList":[{"Id":147613,"Name":"轮回乐园","Author":"那一只蚊子","Img":"lunhuileyuan.jpg","Desc":"机遇与危险共存，只要豁出性命，在轮回乐园中就能得到一切。\r\n　　被轮回乐园选中成为猎杀者的那一刻，苏晓就明白，他将与所有人为敌。\r\n　　乐园虽然残酷，但无所不能……。","CName":"玄幻奇幻","Score":6.3},{"Id":626204,"Name":"夜的命名术","Author":"会说话的肘子","Img":"yedemingmingshu.jpg","Desc":"蓝与紫的霓虹中，浓密的钢铁苍穹下，数据洪流的前端，是科技革命之后的世界，也是现实与虚幻的分界。钢铁与身体，过去与未来。这里，表世界与里世界并存，面前的一切，像是时间之墙近在眼前。黑暗逐渐笼罩。可你要明白啊我的朋友，我们不能用温柔去应对黑暗，要用火。","CName":"玄幻奇幻","Score":8.7},{"Id":632295,"Name":"奥特赘婿","Author":"鸣愿","Img":"aotezhuixu.jpg","Desc":"战神佐菲为了报恩，隐藏身份入赘方家，一路扮猪吃老虎。\\n只是他总是感觉，自己的这位老婆，有亿点点诡异。\\n主角：佐菲。反派：方长/叶紫\\n（本书又名《正义奥特曼必胜！如果结局不好，说明没到结局》）","CName":"玄幻奇幻","Score":8.3},{"Id":631387,"Name":"开局：一个民国位面","Author":"龙升云霄","Img":"kaijuyigeminguoweimian.jpg","Desc":"如果你能往返一个‘特殊’的民国世界，你会做什么？\r\n　　富甲天下，妻妾成群？\r\n　　提笔报国，文压天下？\r\n　　秣马厉兵，封王拜将？\r\n　　还是...\r\n　　练得身形似鹤形，千株松下两函经。\r\n　　我来问道无余说，云在青天水在瓶。\r\n　　ps：本书又名《诸天：从民国开始》。","CName":"科幻灵异","Score":8.8},{"Id":623334,"Name":"斗罗大陆5重生唐三","Author":"唐家三少","Img":"douluodalu5zhongshengtangsan.jpg","Desc":"一代神王唐三，因为妻子的死而选择了殉情，带着一点神识在宇宙中遨游，寻找妻子转世重生的世界。在神识的牵引下，他来到了一个叫作妖精大陆的地方，寻找他的妻子小舞。而他却发现，这是一个人类为刍狗的世界······","CName":"玄幻奇幻","Score":1.4},{"Id":480889,"Name":"世界树的游戏","Author":"咯嘣","Img":"shijieshudeyouxi.jpg","Desc":"“虚拟现实游戏”《精灵国度》中人气最高的NPC，世界树的化身，自然之母，生命女神，精灵主宰——\r\n　　伊芙·尤克特拉希尔高坐在自己的神座上，微笑地看着台下的玩家们：\r\n　　“欢迎来到剑与魔法的世界。”\r\n　　穿越是个技术活。\r\n　　如果不是两界通道和人类玩家，这将是个正经的龙傲娇奇幻故事。","CName":"玄幻奇幻","Score":8.6},{"Id":521014,"Name":"大奉打更人","Author":"卖报小郎君","Img":"dafengdagengren.jpg","Desc":"这个世界，有儒；有道；有佛；有妖；有术士。\r\n　　警校毕业的许七安幽幽醒来，发现自己身处牢狱之中，三日后流放边陲.....\r\n　　他起初的目的只是自保，顺便在这个没有人权的社会里当个富家翁悠闲度日。\r\n　　......\r\n　　多年后，许七安回首前尘，身后是早已逝去的敌人和朋友，以及累累白骨。\r\n　　滚滚长江东逝水，浪花淘尽英雄，是非成败转头空。\r\n　　青山依旧在，几度夕阳红。\r\n　　PS：本书不悲","CName":"武侠仙侠","Score":9.0},{"Id":478397,"Name":"大唐补习班","Author":"危险的世界","Img":"datangbuxiban.jpg","Desc":"柴米油盐酱醋茶，当年样样不离它。如今七事以改变，琴棋书画诗酒花。\r\n　　李昊穿越了，在古代的大唐。\r\n　　文人之中我武力值最高；武将里面我最有文化。\r\n　　大唐将因我而改变……。\r\n　　因为……我们不一样！","CName":"历史军事","Score":6.0},{"Id":630009,"Name":"星门","Author":"老鹰吃小鸡","Img":"xingmen.jpg","Desc":"传说，在那古老的星空深处，伫立着一道血与火侵染的红色之门。\r\n　　传奇与神话，黑暗与光明，无尽传说皆在这古老的门户中流淌。\r\n　　俯瞰星门，热血照耀天地，黑暗终将离去！","CName":"玄幻奇幻","Score":8.8},{"Id":633495,"Name":"我绑架了时间线","Author":"一刀斩斩斩","Img":"wobangjialeshijianxian.jpg","Desc":"一觉醒来，封棋发现世界已经发生了翻天覆地的变化。\r\n　　目之所及满地枯骨，生命凋零。\r\n　　在脑海中声音的指引下，他开始穿梭于现实与未来，逐渐了解了世界的真相，也开始探寻改变世界的方法。\r\n　　正因为见过了黑暗，所以无限向往光明。","CName":"科幻灵异","Score":6.0},{"Id":626648,"Name":"全职之职业欧皇","Author":"闪光哈士奇","Img":"quanzhizhizhiyeouhuang.jpg","Desc":"记者：请问你们兴欣战队的成员对你们的副队长唐银的看法是怎么样的？\r\n　　叶修：他用事实告诉我们，不玩战术的心也脏。以及让人绝望的运气.....\r\n　　苏沐橙：最佳队友，僚机中的战斗机，以及让人羡慕的运气。\r\n　　魏琛：论没下线，我愿称他为最强。还有他绝对和幸运女神有一腿！\r\n　　........\r\n　　唐银：我只不过是运气使然的职业选手。\r\n　　二哈新作：全职高手同人\r\n　　二哈书友群：10467","CName":"玄幻奇幻","Score":8.0},{"Id":31439,"Name":"我当阴阳先生的那几年","Author":"崔走召","Img":"wodangyinyangxianshengdeneijinian.jpg","Desc":"我们的故事是从一个死亡后进入阴间的少年身上开始的。你是否听说过很多民间流传的离奇故事？是否对故事里的那些身怀异术的能人心生过仰慕和向往？本书所讲的就是那些散落在民间的身怀异术之人的故事。他们精通卜卦方术，知晓驱鬼画符，身怀奇门遁甲。当他们的本领已经不被这个时代所承认的时候，他们又该怎么去抉择？\r\n　　\r\n　　    －－－－－－－－－－－－－－－－－－－－－－－－－－－－－－－－－－－－－－－－－－－－－","CName":"科幻灵异","Score":8.9},{"Id":526486,"Name":"剑道第一仙","Author":"萧瑾瑜","Img":"jiandaodiyixian.jpg","Desc":"我是万古人间一剑修，诸天之上第一仙。已有完本作品《符皇》《天骄战纪》公众号：xiaojinyu233","CName":"玄幻奇幻","Score":6.9},{"Id":59334,"Name":"极度尸寒","Author":"全雨","Img":"jidushihan.jpg","Desc":"一个人总能见到鬼，你猜他活的开心吗？\r\n　　\r\n　　    嗯，来点善意的提醒吧。这本书充斥着暴戾、黑暗、血腥、变态，没有一点正能量，压抑的感觉贯穿全书。这本书不适合普通人看，不适合正常人看，更不适合卫道士和正人君子看。当然，得看到后面才能发现这些问题，只看前面的章节是体会不到的。\r\n　　\r\n　　    鄙人最喜欢做的事就是挖坑，而且只管挖不管埋。这本书里的大坑套小坑，一脚陷进去就不好拔出来，大家一定要慎入。","CName":"科幻灵异","Score":7.5},{"Id":627409,"Name":"云边有个小卖部","Author":"张嘉佳","Img":"yunbianyougexiaomaibu.jpg","Desc":"张嘉佳全新作品。畅销千万现象级作品《从你的全世界路过》后，暌违五年，写给离开我们的人，写给陪伴我们的人，写给每个人心中的山和海。\\n希望和悲伤，都是一缕光。总有一天，我们会再相遇。\\n让刘十三陪着你，走进云边镇的春夏秋冬，见证每一场相遇与离别。“有些人刻骨铭心，没几年会遗忘。有些人不论生死，都陪在身旁。”\\n满镇开着桔梗，蒲公英飞得比石榴树还高，一直飘进山","CName":"都市言情","Score":9.5},{"Id":377500,"Name":"斗罗大陆IV终极斗罗","Author":"唐家三少","Img":"douluodaluIVzhongjidouluo.jpg","Desc":"一万年后，冰化了。\r\n　　斗罗联邦科考队在极北之地科考时发现了一个有着金银双色花纹的蛋，用仪器探察之后，发现里面居然有生命体征，赶忙将其带回研究所进行孵化。蛋孵化出来了，可孵出来的却是一个婴儿，和人类一模一样的婴儿，一个蛋生的孩子。","CName":"玄幻奇幻","Score":2.8},{"Id":384854,"Name":"死在火星上","Author":"天瑞说符","Img":"sizaihuoxingshang.jpg","Desc":"我叫唐跃，我在火星上。\r\n　　我刚刚看到地球炸了。","CName":"科幻灵异","Score":8.9},{"Id":607413,"Name":"全球高武之我的系统送错了","Author":"英俊追梦人","Img":"quanqiugaowuzhiwodexitongsongcuole.jpg","Desc":"穿越的那一刻，苏北觉得自己是最幸运的人，尤其是自己穿越的地方叫地球，有个系统叫穿越武侠系统，这是要逆袭的节奏啊。\r\n　　可是整理下记忆，为什么有个职业叫武者，有个爷爷叫苏展，有个学校叫京武？\r\n　　全球高武的世界，小李飞刀，能否一刀戳破源地？降龙十八掌，是否真的能降伏龙皇？我就是把武功练到极致、练到破碎虚空的境界，有用么？","CName":"玄幻奇幻","Score":6.0},{"Id":628100,"Name":"当青春幻想具现后","Author":"转角吻猪","Img":"dangqingchunhuanxiangjuxianhou.jpg","Desc":"当时间停止一小时，只有你可以自由移动时，你会做什么？\r\n　　谢邀，这问题别问我啊！你问她——\r\n　　对！就是这个趁着时间停止来到我身边，朝我伸出手的女孩！\r\n　　------\r\n　　时间停止、返老还童、时空电话、猫的报恩……当青春里出现一件又一件荒唐而又神奇的事件时，我们的故事开始了。\r\n　　（关键词：幻想具现、日常、恋爱）","CName":"都市言情","Score":9.2},{"Id":625913,"Name":"万相之王","Author":"天蚕土豆","Img":"wanxiangzhiwang.jpg","Desc":"天地间，有万相。而我李洛，终将成为这万相之王。","CName":"玄幻奇幻","Score":4.7},{"Id":146769,"Name":"剑来","Author":"烽火戏诸侯","Img":"jianlai.jpg","Desc":"大千世界，无奇不有。我陈平安，唯有一剑，可搬山，倒海，降妖，镇魔，敕神，摘星，断江，摧城，开天！","CName":"玄幻奇幻","Score":8.2}],"Page":1,"HasNext":true}}

### 小说推荐 月榜
GET https://scxs.pigqq.com/top/man/top/commend/month/1.html HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
Content-Type: application/x-www-form-urlencoded
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Host: scxs.pigqq.com
Connection: Keep-Alive
Accept-Encoding: gzip

{"status":1,"info":"success","data":{"BookList":[{"Id":632295,"Name":"奥特赘婿","Author":"鸣愿","Img":"aotezhuixu.jpg","Desc":"战神佐菲为了报恩，隐藏身份入赘方家，一路扮猪吃老虎。\\n只是他总是感觉，自己的这位老婆，有亿点点诡异。\\n主角：佐菲。反派：方长/叶紫\\n（本书又名《正义奥特曼必胜！如果结局不好，说明没到结局》）","CName":"玄幻奇幻","Score":8.3},{"Id":147613,"Name":"轮回乐园","Author":"那一只蚊子","Img":"lunhuileyuan.jpg","Desc":"机遇与危险共存，只要豁出性命，在轮回乐园中就能得到一切。\r\n　　被轮回乐园选中成为猎杀者的那一刻，苏晓就明白，他将与所有人为敌。\r\n　　乐园虽然残酷，但无所不能……。","CName":"玄幻奇幻","Score":6.3},{"Id":626204,"Name":"夜的命名术","Author":"会说话的肘子","Img":"yedemingmingshu.jpg","Desc":"蓝与紫的霓虹中，浓密的钢铁苍穹下，数据洪流的前端，是科技革命之后的世界，也是现实与虚幻的分界。钢铁与身体，过去与未来。这里，表世界与里世界并存，面前的一切，像是时间之墙近在眼前。黑暗逐渐笼罩。可你要明白啊我的朋友，我们不能用温柔去应对黑暗，要用火。","CName":"玄幻奇幻","Score":8.7},{"Id":631387,"Name":"开局：一个民国位面","Author":"龙升云霄","Img":"kaijuyigeminguoweimian.jpg","Desc":"如果你能往返一个‘特殊’的民国世界，你会做什么？\r\n　　富甲天下，妻妾成群？\r\n　　提笔报国，文压天下？\r\n　　秣马厉兵，封王拜将？\r\n　　还是...\r\n　　练得身形似鹤形，千株松下两函经。\r\n　　我来问道无余说，云在青天水在瓶。\r\n　　ps：本书又名《诸天：从民国开始》。","CName":"科幻灵异","Score":8.8},{"Id":628100,"Name":"当青春幻想具现后","Author":"转角吻猪","Img":"dangqingchunhuanxiangjuxianhou.jpg","Desc":"当时间停止一小时，只有你可以自由移动时，你会做什么？\r\n　　谢邀，这问题别问我啊！你问她——\r\n　　对！就是这个趁着时间停止来到我身边，朝我伸出手的女孩！\r\n　　------\r\n　　时间停止、返老还童、时空电话、猫的报恩……当青春里出现一件又一件荒唐而又神奇的事件时，我们的故事开始了。\r\n　　（关键词：幻想具现、日常、恋爱）","CName":"都市言情","Score":9.2},{"Id":521014,"Name":"大奉打更人","Author":"卖报小郎君","Img":"dafengdagengren.jpg","Desc":"这个世界，有儒；有道；有佛；有妖；有术士。\r\n　　警校毕业的许七安幽幽醒来，发现自己身处牢狱之中，三日后流放边陲.....\r\n　　他起初的目的只是自保，顺便在这个没有人权的社会里当个富家翁悠闲度日。\r\n　　......\r\n　　多年后，许七安回首前尘，身后是早已逝去的敌人和朋友，以及累累白骨。\r\n　　滚滚长江东逝水，浪花淘尽英雄，是非成败转头空。\r\n　　青山依旧在，几度夕阳红。\r\n　　PS：本书不悲","CName":"武侠仙侠","Score":9.0},{"Id":630009,"Name":"星门","Author":"老鹰吃小鸡","Img":"xingmen.jpg","Desc":"传说，在那古老的星空深处，伫立着一道血与火侵染的红色之门。\r\n　　传奇与神话，黑暗与光明，无尽传说皆在这古老的门户中流淌。\r\n　　俯瞰星门，热血照耀天地，黑暗终将离去！","CName":"玄幻奇幻","Score":8.8},{"Id":623334,"Name":"斗罗大陆5重生唐三","Author":"唐家三少","Img":"douluodalu5zhongshengtangsan.jpg","Desc":"一代神王唐三，因为妻子的死而选择了殉情，带着一点神识在宇宙中遨游，寻找妻子转世重生的世界。在神识的牵引下，他来到了一个叫作妖精大陆的地方，寻找他的妻子小舞。而他却发现，这是一个人类为刍狗的世界······","CName":"玄幻奇幻","Score":1.4},{"Id":627409,"Name":"云边有个小卖部","Author":"张嘉佳","Img":"yunbianyougexiaomaibu.jpg","Desc":"张嘉佳全新作品。畅销千万现象级作品《从你的全世界路过》后，暌违五年，写给离开我们的人，写给陪伴我们的人，写给每个人心中的山和海。\\n希望和悲伤，都是一缕光。总有一天，我们会再相遇。\\n让刘十三陪着你，走进云边镇的春夏秋冬，见证每一场相遇与离别。“有些人刻骨铭心，没几年会遗忘。有些人不论生死，都陪在身旁。”\\n满镇开着桔梗，蒲公英飞得比石榴树还高，一直飘进山","CName":"都市言情","Score":9.5},{"Id":628547,"Name":"不科学御兽","Author":"轻泉流响","Img":"bukexueyushou.jpg","Desc":"这是一个以御兽为主流的异世界。\r\n　　当时宇携带技能图鉴穿越到这里，并培育出一堆奇葩宠兽后，所有御兽师的三观都破碎了……\r\n　　关键词：御兽、宠兽、宠物、召唤。","CName":"玄幻奇幻","Score":9.0},{"Id":625913,"Name":"万相之王","Author":"天蚕土豆","Img":"wanxiangzhiwang.jpg","Desc":"天地间，有万相。而我李洛，终将成为这万相之王。","CName":"玄幻奇幻","Score":4.7},{"Id":513562,"Name":"柯南之我不是蛇精病","Author":"烟火酒颂","Img":"kenanzhiwobushishejingbing.jpg","Desc":"穿越名侦探柯南的世界，池非迟被送进了医院。\r\n　　周二。\r\n　　医生：“明天周几？”\r\n　　池非迟：“周三。”\r\n　　医生：“咳，明天周五。”\r\n　　池非迟：“……”\r\n　　8月21日。\r\n　　医生：“明天几月几日？”\r\n　　池非迟：“8月22日。”\r\n　　医生：“咳，明天1月1日。”\r\n　　池非迟：“……”\r\n　　当所有人都认为混乱的时间是正确的，而其中一人无法正确辩识并融入其中，那这个人就是异","CName":"玄幻奇幻","Score":6.0},{"Id":436,"Name":"蛊真人","Author":"蛊真人","Img":"436.jpg","Desc":"蛊真人最新章节列：小说《蛊真人》蛊真人/著,蛊真人全文阅读人是万物之灵，蛊是天地真精。三观不正，枭魔重生。昔日旧梦，同名新作。一个穿越者不断重生的故事。(本站郑重提醒：本故事纯属虚构，如有雷同，纯属巧......","CName":"武侠仙侠","Score":9.0},{"Id":630046,"Name":"我就是神！","Author":"历史里吹吹风","Img":"wojiushishen_.jpg","Desc":"尹神的名字叫神。\r\n　　他从来没有想过，有一天自己会真的成为神。","CName":"玄幻奇幻","Score":8.3},{"Id":630133,"Name":"机械炼金术士","Author":"盲候","Img":"jixielianjinshushi.jpg","Desc":"幽暗的地下城，这里埋藏了数之不尽的古代遗迹和宝藏。\r\n　　诡异，畸变，诅咒物...\r\n　　深渊，地窟，古神，神话种族...\r\n　　机械师，咒印植装，巨城黑塔...\r\n　　千奇百怪炼金术，添一勺蒸汽朋克，两勺诡秘超凡，杂糅出了一个缤纷多彩的奇幻世界。\r\n　　我，傀儡炼金术士。\r\n　　一人，便是军团！","CName":"网游竞技","Score":9.6},{"Id":618211,"Name":"我的治愈系游戏","Author":"我会修空调","Img":"wodezhiyuxiyouxi.jpg","Desc":"警察同志，如果我说这是一款休闲治愈系游戏，你们信吗？","CName":"玄幻奇幻","Score":9.1},{"Id":8975,"Name":"全职法师","Author":"乱","Img":"quanzhifashi.jpg","Desc":"一觉醒来，世界大变。\r\n　　\r\n　　    熟悉的高中传授的是魔法，告诉大家要成为一名出色的魔法师。\r\n　　\r\n　　    居住的都市之外游荡着袭击人类的魔物妖兽，虎视眈眈。\r\n　　\r\n　　    崇尚科学的世界变成了崇尚魔法，偏偏有着一样以学渣看待自己的老师，一样目光异样的同学，一样社会底层挣扎的爸爸，一样纯美却不能走路的非血缘妹妹……\r\n　　\r\n　　    不过，莫凡发现绝大多数人都只能够主修一系魔法，自己却","CName":"玄幻奇幻","Score":8.6},{"Id":626698,"Name":"深空彼岸","Author":"辰东","Img":"shenkongbian.jpg","Desc":"浩瀚的宇宙中，一片星系的生灭，也不过是刹那的斑驳流光。仰望星空，总有种结局已注定的伤感，千百年后你我在哪里？家国，文明火光，地球，都不过是深空中的一粒尘埃。星空一瞬，人间千年。虫鸣一世不过秋，你我一样在争渡。深空尽头到底有什么？","CName":"玄幻奇幻","Score":8.5},{"Id":627854,"Name":"大秦：不装了，你爹我是秦始皇","Author":"头顶一只喵喵","Img":"daqin_buzhuangle_nidiewoshiqinshihuang.jpg","Desc":"赵浪一觉醒来，发现自己来到了秦朝。\r\n　　好在家境还算富裕。\r\n　　只是算了算时间，大秦只有三年的寿命，赵浪便鼓起勇气，和自己那几个月才回来一次的便宜老爹说道，\r\n　　“爹，始皇帝三年之后必死，大秦将亡，到时候天下大乱，我们早做准备造反吧！”\r\n　　便宜老爹先是一愣，随后点头同意。\r\n　　赵浪顿时兴教育，练新军。\r\n　　就当他羽翼丰满，准备天下争雄时。\r\n　　便宜老爹突然来到了他的面前，\r\n　　“","CName":"历史军事","Score":7.3},{"Id":191327,"Name":"穷鬼的上下两千年","Author":"非玩家角色","Img":"qiongguideshangxialiangqiannian.jpg","Desc":"她曾经历了长平之战，鉴证了数十万人的坑杀。她曾率领大秦铁骑，与六国逐鹿天下。她见过天下三分，山河破碎。也听过那袅袅的隆中琴音。贞观盛世她曾一醉今朝，那千古女帝又是如何芳华？她鲜衣怒马过，也曾羽扇纶巾。做过田舍农，也为过教书生。却没人知道，这么一个人，活了两千年。嘛，比较轻松悠哉的历史文吧，因为个人原因可能并不能做到完全符合历史，经得起考证。但我会尽力查全资料来写的。第一次写这种文章，我还是希望写的","CName":"历史军事","Score":9.1},{"Id":146769,"Name":"剑来","Author":"烽火戏诸侯","Img":"jianlai.jpg","Desc":"大千世界，无奇不有。我陈平安，唯有一剑，可搬山，倒海，降妖，镇魔，敕神，摘星，断江，摧城，开天！","CName":"玄幻奇幻","Score":8.2}],"Page":1,"HasNext":true}}

### 小说推荐总榜
GET https://scxs.pigqq.com/top/man/top/commend/total/1.html HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
Content-Type: application/x-www-form-urlencoded
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Host: scxs.pigqq.com
Connection: Keep-Alive
Accept-Encoding: gzip


{"status":1,"info":"success","data":{"BookList":[{"Id":412435,"Name":"第一序列","Author":"会说话的肘子","Img":"diyixulie.jpg","Desc":"这是任小粟大魔王出现了吗？画风都不带变的吗？是新一代话题终结者吗？肘星人准备好了吗？想知道大魔王是如何练成的吗？让我们在2019年4月15日一起迎接新的世界吧，看看肘子如何喷翻全场！！","CName":"玄幻奇幻","Score":8.7},{"Id":247586,"Name":"最强狂兵","Author":"就为活着","Img":"zuiqiangkuangbing.jpg","Desc":"王猛，华夏最神秘特种部队的大头兵，被誉为最强最狠辣的狂兵。暴王，大凶，义气兄弟，居家好男人，这些，都是他的代名词。他在敌人眼里就是杀人不眨眼的魔王，但在兄弟和女人眼里，他是义薄云天、柔肠百转的铮铮铁汉......因违抗军令，王猛被部队开除，凶兵回归都市，策马江湖，再搅风云......","CName":"都市言情","Score":6.0},{"Id":140456,"Name":"超神机械师","Author":"齐佩甲","Img":"chaoshenjixieshi.jpg","Desc":"韩萧，《星海》骨灰级代练，被来自东（zuo）方(zhe)的神秘力量扔进穿越大军，携带玩家面板变成NPC，回到《星海》公测之前，毅然选择难度最高的机械系。\r\n　　战舰列队纵横星海，星辰机甲夭矫如龙，幽能炮毁天灭地，还有无边无际的机械大军，静静待在随身仓库里。\r\n　　一人，即是军团！\r\n　　如果不是玩家出现，本书就是正经严肃的穿越异界题材……\r\n　　作为NPC，正常NPC对玩家功能一应俱全……发布任务","CName":"网游竞技","Score":9.4},{"Id":623579,"Name":"王妃投湖","Author":"云若月楚玄辰","Img":"wangfeitouhu.jpg","Desc":"她是21世纪的天才神医，却穿越成不受宠的弃妃，冷面王爷纳妾来恶心她，洞房花烛夜，居然让她这个王妃去伺候，想羞辱她是吧？冷王威胁她，“要想本王不休你，你就老老实实的听话。”她笑道，“王爷，我已经向皇上请旨和离，还会带着孩子再嫁，你千万别担心。”看丑女如何变身为貌美的天才神医，惊艳天下。","CName":"玄幻奇幻","Score":6.0},{"Id":333522,"Name":"转生眼中的火影世界","Author":"空想之龙","Img":"zhuanshengyanzhongdehuoyingshijie.jpg","Desc":"战战兢兢的日向镜，终于得到了梦寐以求的宝物...\r\n　　在宝蓝色的转生眼中，火影的世界究竟是什么样的呢？","CName":"玄幻奇幻","Score":9.2},{"Id":7892,"Name":"误惹妖孽王爷：废材逆天四小姐","Author":"苏小暖","Img":"wureyaoniewangye：feicainitiansixiaojie.jpg","Desc":"误惹妖孽王爷：废材逆天四小姐最新章节列：小说《误惹妖孽王爷：废材逆天四小姐》苏小暖/著,误惹妖孽王爷：废材逆天四小姐全文阅读误惹妖孽王爷：废材逆天四小姐是苏小暖写的浪漫言情类小说....她，21世纪金牌杀手，却穿为苏府最无用的废柴四小姐身上。他，帝国晋王殿下，冷酷邪魅强势霸道，武道天赋更是无与伦比。世人皆知她是草包废柴女，人人唯恐避之不及，唯独他强势霸道死命纠缠她，誓死不放手。且看他们如何强者与强","CName":"都市言情","Score":4.3},{"Id":604124,"Name":"极品全能学生","Author":"夏天叶清雪","Img":"jipinquannengxuesheng.jpg","Desc":"重生过去、畅想未来、梦幻现实，再塑传奇人生！","CName":"都市言情","Score":4.5},{"Id":604123,"Name":"极品全能高手","Author":"夏天叶清雪","Img":"jipinquannenggaoshou.jpg","Desc":"重生过去、畅想未来、梦幻现实，再塑传奇人生！","CName":"都市言情","Score":6.0},{"Id":564789,"Name":"极品全能高手","Author":"花都大少","Img":"jipinquannenggaoshou.jpg","Desc":"【最火爆畅销书】一场车祸改变了我的屌丝人生。各种奇遇接连而来。考试满分，刮刮乐必中，篮球天才，游泳健将选一个？不，老子就是全能。QQ群：203799451【花都出品，必定精品。】","CName":"都市言情","Score":8.0},{"Id":604055,"Name":"有钱就了不起吗","Author":"夏天叶清雪","Img":"youqianjiulebuqima.jpg","Desc":"重生过去、畅想未来、梦幻现实，再塑传奇人生！","CName":"都市言情","Score":6.0},{"Id":8881,"Name":"极品全能学生","Author":"花都大少","Img":"jipinquannengxuesheng.jpg","Desc":"一场车祸让夏天获得了透视功能，从此他踏上了一条与众不同的道路。\r\n　　\r\n　　    打篮球？一个挑五个。\r\n　　\r\n　　    围棋国手？让你三颗子。\r\n　　\r\n　　    鉴宝，我有能看穿一切的透视眼。\r\n　　\r\n　　    极品学姐，温柔学妹，还有冷冷的美女班长，制服小护士，商界女强人，一个都跑不掉。\r\n　　\r\n　　    本书新群：203799451，私人微信：huadu325,\r\n　　\r\n　　    新浪微博：http://weibo","CName":"都市言情","Score":6.2},{"Id":1406,"Name":"捡个杀手做老婆","Author":"花刺1913","Img":"1406.jpg","Desc":"捡个杀手做老婆最新章节列：小说《捡个杀手做老婆》花刺1913/著,捡个杀手做老婆全文阅读月黑风高的夜晚他捡到一个漂亮妩媚性感妖艳的美女，于是他那风骚起伏波澜壮阔的人生开始了……（花花新书，求基友，骚年，大虾......","CName":"网游竞技","Score":6.5},{"Id":68,"Name":"带着农场混异界","Author":"明宇","Img":"68.jpg","Desc":"带着农场混异界最新章节列：小说《带着农场混异界》明宇/著,带着农场混异界全文阅读他横任他横，我自种我田，若要来惹我，过不了明年。宅男赵海带着qq农场穿越到了异界，附身到了一个落迫的小贵族身上，他的封地是一......","CName":"玄幻奇幻","Score":6.6},{"Id":457704,"Name":"御魂者传奇","Author":"沙之愚者","Img":"yuhunzhechuanqi.jpg","Desc":"本书的每个分卷都是独立故事，全新人物、全新设定、全新世界！\r\n　　第一卷【美漫英雄】已完结\r\n　　第二卷【奇幻大陆】已完结\r\n　　第三卷【历史长河：上古篇】连载中……\r\n　　**********************\r\n　　本书互动沙窝扣：【四七零八四二二四三（4－7－0－8－4－2－2－4－3）】欢迎各方朋友来畅所欲言！\r\n　　感谢阅文书评团提供书评支持","CName":"玄幻奇幻","Score":6.0},{"Id":46234,"Name":"驱尸赶鬼纵横美漫","Author":"沙之愚者","Img":"qushiganguizonghengmeiman.jpg","Desc":"美漫世界遭遇最危急的毁灭时期！！\r\n　　\r\n　　    面对僵尸反派、鬼魅邪魔，超级英雄们束手无策？！\r\n　　\r\n　　    雷神满脸是泪：我用手里的锤子和裆里的锤子拼命揍他，可丫愣是无限复活！\r\n　　\r\n　　    钢铁侠垂头丧气：我又被鬼魅附身了！别靠近我，对不起，惊奇女士，不是我想摸你屁股，是鬼……\r\n　　\r\n　　    危急时刻，托尼和几个金主拼命砸钱，造出了平行世界穿越机！\r\n　　\r\n　　    “听说在古老的华夏，有一种很牛","CName":"科幻灵异","Score":3.0},{"Id":47589,"Name":"御鬼者传奇","Author":"沙之愚者","Img":"yuguizhechuanqi.jpg","Desc":"【老沙的话;94天更新百万字目标达成！下一个目标：200天更新200万字，请大家多多支持，老沙拜谢↖(^ω^)↗】\r\n　　\r\n　　    **********************\r\n　　\r\n　　    玄幻、奇幻、武侠、仙侠、都市职场、历史长河、游戏、竞技、科幻、灵异，御鬼者的足迹与冒险将留在这些世界的每一个角落！\r\n　　\r\n　　    一个分卷，就是一场新的传奇！！\r\n　　\r\n　　    抱歉，这本书不是什么灵异的小众文…","CName":"科幻灵异","Score":6.0},{"Id":721,"Name":"我的贴身校花","Author":"带玉","Img":"721.jpg","Desc":"我的贴身校花最新章节列：小说《我的贴身校花》带玉/著,我的贴身校花全文阅读一个普通的高中生，无意间得到一瓶丹药，让他身怀数种异能。追校花，被校花追。清纯校花，傲娇校花，野辣校花，都来贴身。此外，还有靓丽......","CName":"玄幻奇幻","Score":6.9},{"Id":579844,"Name":"龙王婿陆榆纪凝雪","Author":"会说话的香烟","Img":"longwangxuluyujiningxue.jpg","Desc":"我是他人眼中一无是处的废物赘婿；但，上门女婿，未必不能翱翔九天！倘若她要，我就可以，给她整个世界。","CName":"都市言情","Score":6.0},{"Id":515807,"Name":"狂龙在都","Author":"会说话的香烟","Img":"kuanglongzaidou.jpg","Desc":"我是他人眼中一无是处的废物赘婿；但，上门女婿，未必不能翱翔九天！倘若她要，我就可以，给她整个世界。","CName":"都市言情","Score":6.0},{"Id":592006,"Name":"陆枫纪雪雨","Author":"会说话的香烟","Img":"lufengjixueyu.jpg","Desc":"我是他人眼中一无是处的废物赘婿；但，上门女婿，未必不能翱翔九天！倘若她要，我就可以，给她整个世界。","CName":"都市言情","Score":6.0},{"Id":602263,"Name":"陆鸣陆瑶","Author":"陆鸣陆瑶","Img":"lumingluyao.jpg","Desc":"〔暴爽玄幻，最热爽文〕少年陆鸣，血脉被夺，沦为废人，受尽屈辱。幸得至尊神殿，重生无上血脉，从此脚踏天才，一路逆袭，踏上热血辉煌之路。噬无尽生灵，融诸天血脉，跨千山万水，闯九天十地，败尽天下英豪，修战龙真诀，成就万道龙皇。","CName":"都市言情","Score":6.0}],"Page":1,"HasNext":true}}

### 小说推荐总榜 分页
GET https://scxs.pigqq.com/top/man/top/commend/total/2.html HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
Content-Type: application/x-www-form-urlencoded
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Host: scxs.pigqq.com
Connection: Keep-Alive
Accept-Encoding: gzip

{"status":1,"info":"success","data":{"BookList":[{"Id":602275,"Name":"血脉重生","Author":"陆鸣陆瑶","Img":"xuemaizhongsheng.jpg","Desc":"〔暴爽玄幻，最热爽文〕少年陆鸣，血脉被夺，沦为废人，受尽屈辱。幸得至尊神殿，重生无上血脉，从此脚踏天才，一路逆袭，踏上热血辉煌之路。噬无尽生灵，融诸天血脉，跨千山万水，闯九天十地，败尽天下英豪，修战龙真诀，成就万道龙皇。","CName":"都市言情","Score":6.0},{"Id":602262,"Name":"气运大会上元婴期一桌","Author":"陆鸣陆瑶","Img":"qiyundahuishangyuanyingqiyizhuo.jpg","Desc":"〔暴爽玄幻，最热爽文〕少年陆鸣，血脉被夺，沦为废人，受尽屈辱。幸得至尊神殿，重生无上血脉，从此脚踏天才，一路逆袭，踏上热血辉煌之路。噬无尽生灵，融诸天血脉，跨千山万水，闯九天十地，败尽天下英豪，修战龙真诀，成就万道龙皇。","CName":"都市言情","Score":6.0},{"Id":598042,"Name":"至尊神殿陆鸣","Author":"陆鸣陆瑶","Img":"zhizunshendianluming.jpg","Desc":"〔暴爽玄幻，最热爽文〕少年陆鸣，血脉被夺，沦为废人，受尽屈辱。幸得至尊神殿，重生无上血脉，从此脚踏天才，一路逆袭，踏上热血辉煌之路。噬无尽生灵，融诸天血脉，跨千山万水，闯九天十地，败尽天下英豪，修战龙真诀，成就万道龙皇。群号：570274770","CName":"玄幻奇幻","Score":6.0},{"Id":602267,"Name":"夕阳西下,霞光漫天。风火城外,翠云峰上","Author":"陆鸣陆瑶","Img":"xiyangxixia,xiaguangmantian。fenghuochengwai,cuiyunfengshang.jpg","Desc":"〔暴爽玄幻，最热爽文〕少年陆鸣，血脉被夺，沦为废人，受尽屈辱。幸得至尊神殿，重生无上血脉，从此脚踏天才，一路逆袭，踏上热血辉煌之路。噬无尽生灵，融诸天血脉，跨千山万水，闯九天十地，败尽天下英豪，修战龙真诀，成就万道龙皇。","CName":"都市言情","Score":6.0},{"Id":602325,"Name":"万道龙皇","Author":"陆鸣陆瑶","Img":"wandaolonghuang.jpg","Desc":"〔暴爽玄幻，最热爽文〕少年陆鸣，血脉被夺，沦为废人，受尽屈辱。幸得至尊神殿，重生无上血脉，从此脚踏天才，一路逆袭，踏上热血辉煌之路。噬无尽生灵，融诸天血脉，跨千山万水，闯九天十地，败尽天下英豪，修战龙真诀，成就万道龙皇。","CName":"都市言情","Score":4.0},{"Id":604887,"Name":"重犯监狱","Author":"陈六合沈清舞","Img":"zhongfanjianyu.jpg","Desc":"国之重器，猛虎出笼！亦正亦邪的他注定有着无法平淡的命运！身负枷锁执掌生杀命轮！他身立潮头一生高唱大风！只装最牛的逼，只踩最狠的人！他一生辉煌，彪悍铸就，舞练长空！！！","CName":"都市言情","Score":6.0},{"Id":605675,"Name":"陈六合苏婉玥","Author":"陈六合沈清舞","Img":"chenliuhesuwanyue.jpg","Desc":"国之重器，猛虎出笼！亦正亦邪的他注定有着无法平淡的命运！身负枷锁执掌生杀命轮！他身立潮头一生高唱大风！只装最牛的逼，只踩最狠的人！他一生辉煌，彪悍铸就，舞练长空！！！","CName":"都市言情","Score":6.0},{"Id":602201,"Name":"江城高铁站，夏日炎炎","Author":"叶辰夏若雪","Img":"jiangchenggaotiezhan，xiariyanyan.jpg","Desc":"【火爆爽文】五年前，废物叶辰犹如地上蠕虫般被人耻笑！但是五年后，他带着一百位上古大能回来了！吊打一切，谁与争锋！","CName":"都市言情","Score":6.0},{"Id":602193,"Name":"嗜血狂龙叶辰","Author":"叶辰夏若雪","Img":"shixuekuanglongyechen.jpg","Desc":"【火爆爽文】五年前，废物叶辰犹如地上蠕虫般被人耻笑！但是五年后，他带着一百位上古大能回来了！吊打一切，谁与争锋！","CName":"都市言情","Score":6.0},{"Id":606875,"Name":"仙魔同修","Author":"流浪","Img":"xianmotongxiu.jpg","Desc":"云海缥缈，苍穹无限。芸芸众生，谁不心向往之？天道虚幻，无人得窥。万丈红尘，何人不欲长生？三生七世的怨侣，正道与魔教数千年的恩怨情仇。一个人，一柄古剑，他将如何面对整个世界……","CName":"玄幻奇幻","Score":6.0},{"Id":671,"Name":"校花的贴身高手","Author":"鱼人二代","Img":"671.jpg","Desc":"校花的贴身高手最新章节列：小说《校花的贴身高手》鱼人二代/著,校花的贴身高手全文阅读一个大山里走出来的绝世高手，一块能预知未来的神秘玉佩……林逸是一名普通学生，不过，他还身负另外一个重任，那就是追校花！......","CName":"玄幻奇幻","Score":2.5},{"Id":625837,"Name":"林逸楚梦瑶","Author":"鱼人二代","Img":"linyichumengyao.jpg","Desc":"一个大山里走出来的绝世高手，一块能预知未来的神秘玉佩……林逸是一名普通学生，不过，他还身负另外一个重任，那就是追校花！而且还是奉校花老爸之命！虽然林逸很不想跟这位难伺候的大小姐打交道，但是长辈之命难违抗，他不得不千里迢迢的转学到了松山市，给大小姐鞍前马后的当跟班……于是，史上最牛的跟班出现了——大小姐的贴身高手！","CName":"玄幻奇幻","Score":6.0},{"Id":520472,"Name":"叶辰夏若雪","Author":"风会笑","Img":"yechenxiaruoxue.jpg","Desc":"“古武者？地狱归来？华夏第一人？我惹不起？不好意思，在我面前，都要跪下！”五年前，家族覆灭，废物叶辰犹如地上蠕虫般被人耻笑！但是五年后，他带着一身逆天术法强势回归！更可怕的是，他背后还站着一百位曾屹立于世界之巅的上古大能！PS：此书精品保证！另有400万字畅销火书正在连载！","CName":"都市言情","Score":3.5},{"Id":602200,"Name":"都市极品医神","Author":"叶辰夏若雪","Img":"doushijipinyishen.jpg","Desc":"【火爆爽文】五年前，废物叶辰犹如地上蠕虫般被人耻笑！但是五年后，他带着一百位上古大能回来了！吊打一切，谁与争锋！","CName":"都市言情","Score":6.0},{"Id":606807,"Name":"叶小川云乞幽","Author":"流浪","Img":"yexiaochuanyunqiyou.jpg","Desc":"云海缥缈，苍穹无限。芸芸众生，谁不心向往之？天道虚幻，无人得窥。万丈红尘，何人不欲长生？三生七世的怨侣，正道与魔教数千年的恩怨情仇。一个人，一柄古剑，他将如何面对整个世界……","CName":"玄幻奇幻","Score":6.0},{"Id":605676,"Name":"都市狂枭","Author":"陈六合沈清舞","Img":"doushikuangxiao.jpg","Desc":"国之重器，猛虎出笼！亦正亦邪的他注定有着无法平淡的命运！身负枷锁执掌生杀命轮！他身立潮头一生高唱大风！只装最牛的逼，只踩最狠的人！他一生辉煌，彪悍铸就，舞练长空！！！","CName":"都市言情","Score":6.0},{"Id":250332,"Name":"都市之最强狂兵","Author":"大红大紫","Img":"doushizhizuiqiangkuangbing.jpg","Desc":"国之重器，猛虎出笼！亦正亦邪的他注定有着无法平淡的命运！身负枷锁执掌生杀命轮！他身立潮头一生高唱大风！\r\n　　只装最牛的逼，只踩最狠的人！然而这样一个牛人还偏偏魅力十足，女校长、女总裁、女大佬、还有御姐萝莉纷踏而来！这也是一种极大的负担！\r\n　　大红大紫出品必属精品，有多本完本经验，请放心阅读！！！\r\n　　书友1群（都市狂人）：611213735","CName":"玄幻奇幻","Score":8.5},{"Id":512140,"Name":"都市狂枭","Author":"大红大紫","Img":"doushikuangxiao.jpg","Desc":"国之重器，猛虎出笼！亦正亦邪的他注定有着无法平淡的命运！身负枷锁执掌生杀命轮！他身立潮头一生高唱大风！只装最牛的逼，只踩最狠的人！他一生辉煌，彪悍铸就，舞练长空！！！大红大紫出品必属精品，有多本完本经验，请放心阅读！！！","CName":"都市言情","Score":8.0},{"Id":600293,"Name":"陈六合沈清舞","Author":"大红大紫","Img":"chenliuheshenqingwu.jpg","Desc":"国之重器，猛虎出笼！亦正亦邪的他注定有着无法平淡的命运！身负枷锁执掌生杀命轮！他身立潮头一生高唱大风！然而这样一个牛人还偏偏魅力十足！这也是一种极大的负担！","CName":"都市言情","Score":6.0},{"Id":605677,"Name":"都市之最强狂兵","Author":"陈六合沈清舞","Img":"doushizhizuiqiangkuangbing.jpg","Desc":"国之重器，猛虎出笼！亦正亦邪的他注定有着无法平淡的命运！身负枷锁执掌生杀命轮！他身立潮头一生高唱大风！只装最牛的逼，只踩最狠的人！他一生辉煌，彪悍铸就，舞练长空！！！","CName":"都市言情","Score":6.0}],"Page":2,"HasNext":true}}

### 小说搜索
GET https://souxs.pigqq.com/search.aspx?key=%E6%88%91%E4%BB%80%E4%B9%88%E6%97%B6%E5%80%99%E6%97%A0%E6%95%8C%E4%BA%86&page=1&siteid=app2 HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
Content-Type: application/x-www-form-urlencoded
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Host: souxs.pigqq.com
Connection: Keep-Alive
Accept-Encoding: gzip

{"status":1,"info":"success","data":[{"Id":"618328","Name":"\u6211\u4ec0\u4e48\u65f6\u5019\u65e0\u654c\u4e86","Author":"\u620f\u67f3\u5148\u751f","Img":"https:\/\/imgapixs.pysmei.com\/bookfiles\/bookimages\/woshenmeshihouwudile.jpg","Desc":"\u3010\u65e0\u654c+\u641e\u7b11+\u5355\u5973\u4e3b+\u8fea\u5316\u3011\u4ed6\u4e00\u76f4\u4ee5\u4e3a\u81ea\u5df1\u662f\u51e1\u4eba\uff0c\u5374\u4e0d\u77e5\u9662\u5b50\u91cc\u5806\u6ee1\u4e86\u795e\u5668\uff0c\u517b\u7684\u9e21\u66f4\u662f\u51e4\u51f0\uff01\u76f4\u5230\u5728\u51e1\u4eba\u5c0f\u9547\u751f\u6d3b\u4e86\u4e94\u5e74\uff0c\u7cfb\u7edf\u7ec8\u4e8e\u8ba9\u4ed6\u53bb\u63a5\u89e6\u4fee\u70bc\u8005\u3002\u8fd9\u65f6\u5019\u4ed6\u624d\u53d1\u73b0\uff0c\u4e0d\u7ba1\u591a\u5f3a\u7684\u4eba\uff0c\u89c1\u5230\u4ed6\u90a3\u523b\uff0c\u90fd\u4f1a\u5413\u5f97\u817f\u8f6f\uff0c\u558a\u4ed6\u524d\u8f88\u3002\u6709\u751a\u8005\uff0c\u8fd8\u8dea\u5730\u671d\u62dc......\u6b64\u4e66\u504f\u6c99\u96d5\u65e0\u5398\u5934\uff0c\u4e13\u6cbb\u4e0d\u5f00\u5fc3\uff0c\u98ce\u683c\u5947\u7279\uff0c\u770b\u5b8c\u6709\u60ca\u559c\u54e6\uff01","BookStatus":"\u8fde\u8f7d","LastChapterId":"4186141","LastChapter":"\u7b2c1037\u7ae0 \u62e5\u6709\u6240\u6709\u5927\u9053\u4e4b\u5370","CName":"\u7384\u5e7b\u5947\u5e7b","UpdateTime":"2021-09-20 00:00:00","weekHitCount":"25172","monthHitCount":"177068","hitCount":"1506726"},{"Id":"627464","Name":"\u7384\u5e7b\uff1a\u6211\u4ec0\u4e48\u65f6\u5019\u65e0\u654c\u4e86","Author":"\u620f\u67f3\u5148\u751f","Img":"https:\/\/imgapixs.pysmei.com\/bookfiles\/bookimages\/xuanhuan_woshenmeshihouwudile.jpg","Desc":"\u3010\u65e0\u654c+\u641e\u7b11+\u5355\u5973\u4e3b+\u8fea\u5316\u3011\\n\u4ed6\u4e00\u76f4\u4ee5\u4e3a\u81ea\u5df1\u662f\u51e1\u4eba\uff0c\u5374\u4e0d\u77e5\u9662\u5b50\u91cc\u5806\u6ee1\u4e86\u795e\u5668\uff0c\u517b\u7684\u9e21\u66f4\u662f\u51e4\u51f0\uff01\\n\u76f4\u5230\u5728\u51e1\u4eba\u5c0f\u9547\u751f\u6d3b\u4e86\u4e94\u5e74\uff0c\u7cfb\u7edf\u7ec8\u4e8e\u8ba9\u4ed6\u53bb\u63a5\u89e6\u4fee\u70bc\u8005\u3002\\n\u8fd9\u65f6\u5019\u4ed6\u624d\u53d1\u73b0\uff0c\u4e0d\u7ba1\u591a\u5f3a\u7684\u4eba\uff0c\u89c1\u5230\u4ed6\u90a3\u523b\uff0c\u90fd\u4f1a\u5413\u5f97\u817f\u8f6f\uff0c\u558a\u4ed6\u524d\u8f88\u3002\u6709\u751a\u8005\uff0c\u8fd8\u8dea\u5730\u671d\u62dc......\\n\u6b64\u4e66\u504f\u6c99\u96d5\u65e0\u5398\u5934\uff0c\u4e13\u6cbb\u4e0d\u5f00\u5fc3\uff0c\u98ce\u683c\u5947\u7279\uff0c\u770b\u5b8c\u6709\u60ca\u559c\u54e6\uff01","BookStatus":"\u8fde\u8f7d","LastChapterId":"4220198","LastChapter":"\u7b2c1037\u7ae0 \u62e5\u6709\u6240\u6709\u5927\u9053\u4e4b\u5370","CName":"\u7384\u5e7b\u5947\u5e7b","UpdateTime":"2021-09-20 00:00:00","weekHitCount":"592","monthHitCount":"3135","hitCount":"36541"}]}

### 小说收藏周榜
GET https://scxs.pigqq.com/top/man/top/collect/week/1.html HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
Content-Type: application/x-www-form-urlencoded
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Host: scxs.pigqq.com
Connection: Keep-Alive
Accept-Encoding: gzip

{"status":1,"info":"success","data":{"BookList":[{"Id":625913,"Name":"万相之王","Author":"天蚕土豆","Img":"wanxiangzhiwang.jpg","Desc":"天地间，有万相。而我李洛，终将成为这万相之王。","CName":"玄幻奇幻","Score":4.7},{"Id":521014,"Name":"大奉打更人","Author":"卖报小郎君","Img":"dafengdagengren.jpg","Desc":"这个世界，有儒；有道；有佛；有妖；有术士。\r\n　　警校毕业的许七安幽幽醒来，发现自己身处牢狱之中，三日后流放边陲.....\r\n　　他起初的目的只是自保，顺便在这个没有人权的社会里当个富家翁悠闲度日。\r\n　　......\r\n　　多年后，许七安回首前尘，身后是早已逝去的敌人和朋友，以及累累白骨。\r\n　　滚滚长江东逝水，浪花淘尽英雄，是非成败转头空。\r\n　　青山依旧在，几度夕阳红。\r\n　　PS：本书不悲","CName":"武侠仙侠","Score":9.0},{"Id":620881,"Name":"这个人仙太过正经","Author":"言归正传","Img":"zheigerenxiantaiguozhengjing.jpg","Desc":"2月5号，新书《这个人仙太过正经》就要跟各位读者老爷见面了！半神之躯，比肩凡人！正经人仙，在线薅神！","CName":"玄幻奇幻","Score":8.3},{"Id":618328,"Name":"我什么时候无敌了","Author":"戏柳先生","Img":"woshenmeshihouwudile.jpg","Desc":"【无敌+搞笑+单女主+迪化】他一直以为自己是凡人，却不知院子里堆满了神器，养的鸡更是凤凰！直到在凡人小镇生活了五年，系统终于让他去接触修炼者。这时候他才发现，不管多强的人，见到他那刻，都会吓得腿软，喊他前辈。有甚者，还跪地朝拜......此书偏沙雕无厘头，专治不开心，风格奇特，看完有惊喜哦！","CName":"玄幻奇幻","Score":3.3},{"Id":624842,"Name":"我顿悟了混沌体","Author":"萧云席春雨","Img":"wodunwulehundunti.jpg","Desc":"萧云的系统只会一个功能——顿悟！体质平凡？顿悟混沌体！功法难修？顿悟圆满境界！神通难修？顿悟圆满境界！没有什么是顿悟不能解决的，如果有，那就顿悟十次，百次……","CName":"玄幻奇幻","Score":4.8},{"Id":622896,"Name":"弃宇宙","Author":"鹅是老五","Img":"qiyuzhou.jpg","Desc":"地球元气复苏了，但这真不是地球灵气复苏的故事，\r\n　　而是一个流浪宇宙的故事。","CName":"武侠仙侠","Score":5.3},{"Id":620826,"Name":"我的七个姐姐风华绝代","Author":"无言会语","Img":"wodeqigejiejiefenghuajuedai.jpg","Desc":"大姐莫向晚，霸道总裁……二姐白吟霜，国际杀手……三姐沈冰，国际空姐……四姐顾心怡，拥有绝世医术……五姐罗晓，有名的警花……六姐罗娜，拥有神秘的身份……七姐叶凝云，绝代影后……","CName":"都市言情","Score":2.0},{"Id":624757,"Name":"贞观战神","Author":"李文昊李世民","Img":"zhenguanzhanshen.jpg","Desc":"穿越唐朝，成为不存在历史中的李世民长子。天生痴傻的李文昊终于在李元霸的葬礼上觉醒了。民间传说，将不过李，王不过霸，但是开局摸了天下无敌李元霸的尸体，李文昊会有多猛？惹事，他从来不怕。打架，他从来不虚。作死，他更是一流。拼爹？呵呵！李文昊：“我交朋友从来不看他爹厉不厉害，因为无论他爹多厉害都没有我爹厉害”","CName":"玄幻奇幻","Score":2.6},{"Id":5,"Name":"完美世界","Author":"辰东","Img":"5.jpg","Desc":"完美世界最新章节列：小说《完美世界》辰东/著,完美世界全文阅读完美世界是辰东写的东方玄幻类小说..........","CName":"玄幻奇幻","Score":9.0},{"Id":8975,"Name":"全职法师","Author":"乱","Img":"quanzhifashi.jpg","Desc":"一觉醒来，世界大变。\r\n　　\r\n　　    熟悉的高中传授的是魔法，告诉大家要成为一名出色的魔法师。\r\n　　\r\n　　    居住的都市之外游荡着袭击人类的魔物妖兽，虎视眈眈。\r\n　　\r\n　　    崇尚科学的世界变成了崇尚魔法，偏偏有着一样以学渣看待自己的老师，一样目光异样的同学，一样社会底层挣扎的爸爸，一样纯美却不能走路的非血缘妹妹……\r\n　　\r\n　　    不过，莫凡发现绝大多数人都只能够主修一系魔法，自己却","CName":"玄幻奇幻","Score":8.6},{"Id":3143,"Name":"斗破苍穹","Author":"天蚕土豆","Img":"doupocangqiong.jpg","Desc":"这里是属于斗气的世界，没有花俏艳丽的魔法，有的，仅仅是繁衍到巅峰的斗气！新书刚开，请各位兄弟多多支持，用推荐票和收藏，砸烂偶吧.^_^新书等级制度：斗者，斗师，大斗师，斗灵，斗王，斗皇，斗宗，斗尊，斗圣，斗帝。","CName":"玄幻奇幻","Score":8.1},{"Id":1559,"Name":"斗罗大陆","Author":"唐家三少","Img":"douluodalu.jpg","Desc":"【小三新书《阴阳冕》已经注册】将会在本周日，斗罗大陆结束的同时开始上传更新，麻烦大家先收藏、推荐一下，谢谢。阴阳冕书号：1436015下面的直通车也可以直接点过去。【小三出品，必属精品，全新设定，酬谢书友】target=&_blank&","CName":"玄幻奇幻","Score":4.6},{"Id":623334,"Name":"斗罗大陆5重生唐三","Author":"唐家三少","Img":"douluodalu5zhongshengtangsan.jpg","Desc":"一代神王唐三，因为妻子的死而选择了殉情，带着一点神识在宇宙中遨游，寻找妻子转世重生的世界。在神识的牵引下，他来到了一个叫作妖精大陆的地方，寻找他的妻子小舞。而他却发现，这是一个人类为刍狗的世界······","CName":"玄幻奇幻","Score":1.4},{"Id":628547,"Name":"不科学御兽","Author":"轻泉流响","Img":"bukexueyushou.jpg","Desc":"这是一个以御兽为主流的异世界。\r\n　　当时宇携带技能图鉴穿越到这里，并培育出一堆奇葩宠兽后，所有御兽师的三观都破碎了……\r\n　　关键词：御兽、宠兽、宠物、召唤。","CName":"玄幻奇幻","Score":9.0},{"Id":627854,"Name":"大秦：不装了，你爹我是秦始皇","Author":"头顶一只喵喵","Img":"daqin_buzhuangle_nidiewoshiqinshihuang.jpg","Desc":"赵浪一觉醒来，发现自己来到了秦朝。\r\n　　好在家境还算富裕。\r\n　　只是算了算时间，大秦只有三年的寿命，赵浪便鼓起勇气，和自己那几个月才回来一次的便宜老爹说道，\r\n　　“爹，始皇帝三年之后必死，大秦将亡，到时候天下大乱，我们早做准备造反吧！”\r\n　　便宜老爹先是一愣，随后点头同意。\r\n　　赵浪顿时兴教育，练新军。\r\n　　就当他羽翼丰满，准备天下争雄时。\r\n　　便宜老爹突然来到了他的面前，\r\n　　“","CName":"历史军事","Score":7.3},{"Id":626204,"Name":"夜的命名术","Author":"会说话的肘子","Img":"yedemingmingshu.jpg","Desc":"蓝与紫的霓虹中，浓密的钢铁苍穹下，数据洪流的前端，是科技革命之后的世界，也是现实与虚幻的分界。钢铁与身体，过去与未来。这里，表世界与里世界并存，面前的一切，像是时间之墙近在眼前。黑暗逐渐笼罩。可你要明白啊我的朋友，我们不能用温柔去应对黑暗，要用火。","CName":"玄幻奇幻","Score":8.7},{"Id":630009,"Name":"星门","Author":"老鹰吃小鸡","Img":"xingmen.jpg","Desc":"传说，在那古老的星空深处，伫立着一道血与火侵染的红色之门。\r\n　　传奇与神话，黑暗与光明，无尽传说皆在这古老的门户中流淌。\r\n　　俯瞰星门，热血照耀天地，黑暗终将离去！","CName":"玄幻奇幻","Score":8.8},{"Id":627885,"Name":"迎娶女帝之后","Author":"老狗","Img":"yingqunvdizhihou.jpg","Desc":"李云没有想到，穿越到这个世界后的第一件事，就是被迫卷入造反的大军。大乾九百七十六年，居于大陆之央的大乾终于镇压了这场大陆千年来规模最大，影响力最深的叛乱，平四方，镇气运。同年，大乾老皇帝驾崩，新帝登基，整个世界的命运都被掌握在这位新的至高权力者手上，无人能够逃过。","CName":"玄幻奇幻","Score":8.0},{"Id":630133,"Name":"机械炼金术士","Author":"盲候","Img":"jixielianjinshushi.jpg","Desc":"幽暗的地下城，这里埋藏了数之不尽的古代遗迹和宝藏。\r\n　　诡异，畸变，诅咒物...\r\n　　深渊，地窟，古神，神话种族...\r\n　　机械师，咒印植装，巨城黑塔...\r\n　　千奇百怪炼金术，添一勺蒸汽朋克，两勺诡秘超凡，杂糅出了一个缤纷多彩的奇幻世界。\r\n　　我，傀儡炼金术士。\r\n　　一人，便是军团！","CName":"网游竞技","Score":9.6},{"Id":147613,"Name":"轮回乐园","Author":"那一只蚊子","Img":"lunhuileyuan.jpg","Desc":"机遇与危险共存，只要豁出性命，在轮回乐园中就能得到一切。\r\n　　被轮回乐园选中成为猎杀者的那一刻，苏晓就明白，他将与所有人为敌。\r\n　　乐园虽然残酷，但无所不能……。","CName":"玄幻奇幻","Score":6.3},{"Id":3051,"Name":"遮天","Author":"辰东","Img":"zhetian.jpg","Desc":"冰冷与黑暗并存的宇宙深处，九具庞大的龙尸拉着一口青铜古棺，亘古长存。这是太空探测器在枯寂的宇宙中捕捉到的一幅极其震撼的画面。九龙拉棺，究竟是回到了上古，还是来到了星空的彼岸？一个浩大的仙侠世界，光怪陆离，神秘无尽。热血似火山沸腾，激情若瀚海汹涌，欲望如深渊无止境……登天路，踏歌行，弹指遮天。","CName":"武侠仙侠","Score":8.6}],"Page":1,"HasNext":true}}

### 小说评分榜
GET https://scxs.pigqq.com/top/man/top/vote/week/1.html HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
Content-Type: application/x-www-form-urlencoded
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Host: scxs.pigqq.com
Connection: Keep-Alive
Accept-Encoding: gzip

{"status":1,"info":"success","data":{"BookList":[{"Id":521014,"Name":"大奉打更人","Author":"卖报小郎君","Img":"dafengdagengren.jpg","Desc":"这个世界，有儒；有道；有佛；有妖；有术士。\r\n　　警校毕业的许七安幽幽醒来，发现自己身处牢狱之中，三日后流放边陲.....\r\n　　他起初的目的只是自保，顺便在这个没有人权的社会里当个富家翁悠闲度日。\r\n　　......\r\n　　多年后，许七安回首前尘，身后是早已逝去的敌人和朋友，以及累累白骨。\r\n　　滚滚长江东逝水，浪花淘尽英雄，是非成败转头空。\r\n　　青山依旧在，几度夕阳红。\r\n　　PS：本书不悲","CName":"武侠仙侠","Score":9.4},{"Id":570433,"Name":"我真没想当训练家啊","Author":"北川南海","Img":"wozhenmeixiangdangxunlianjiaa.jpg","Desc":"现在站在你面前的是——\r\n　　得文公司董事会、彩虹火箭队缔造者、逆属性大师、世界锦标赛冠军……\r\n　　传奇训练家陆野，回忆起首次直播时的场景，喟然长叹。\r\n　　“说起来你们可能不信，我最初的愿望只是破十万订阅露个脸而已。”\r\n　　“我只想恰点钱，从一名游戏区UP主做起。”\r\n　　“我真没想当训练家啊！”\r\n　　本书又名：《五等分的陆野》、《青春期训练家不会梦见神奥冠军》、《竹兰大小姐想让我告白》、","CName":"玄幻奇幻","Score":9.3},{"Id":600715,"Name":"我家老婆来自一千年前","Author":"花还没开","Img":"wojialaopolaiziyiqiannianqian.jpg","Desc":"“我想回家。”\r\n　　“你可能回不去了。”\r\n　　“为什么？”\r\n　　“因为这里离你家很远。”\r\n　　“有多远？”\r\n　　“一千二百多年那么远。”\r\n　　许青看着眼前来自唐朝的少女，脸上带有一丝同情：“你所熟悉的一切，都已经变成历史。”\r\n　　亲朋，好友，敌人，全部沉寂在一千二百年前。\r\n　　———\r\n　　日常文，单女主\r\n　　（已有完本精品，质量保证。）","CName":"都市言情","Score":9.3},{"Id":24328,"Name":"非正常人类异闻录","Author":"精分三代","Img":"feizhengchangrenleiyiwenlu.jpg","Desc":"我叫张大道，道号张全道。在第七人民医院被人研究！\r\n　　\r\n　　    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\r\n　　\r\n　　    贫道张全道，专业摸骨批命，棺材翻新,抛光,打蜡。回收二手僵尸,寻龙点穴、批发黑驴蹄、黑狗血。代写1~3年级小学作业，寻找走失猫狗，抓小三。\r\n　　\r\n　　    专业报仇打小人、改风水、妨祖坟！量大从优！有发票！\r\n　　\r\n　　    ~~~~~","CName":"都市言情","Score":9.3},{"Id":488380,"Name":"万界圆梦师","Author":"棉衣卫","Img":"wanjieyuanmengshi.jpg","Desc":"自爆、增发术、断肢求生、被读心术、百分百被空手接白刃……是我的金手指！\r\n　　帮助拆迁女怀上李寻欢的孩子；带十岁小女孩打穿海扁王的世界；协助客户获得步惊云的麒麟臂……是我的日常工作。\r\n　　崩剧情，杀主角，毁灭世界规则……不惜一切代价，即便你自己放弃了梦想，我都不会放弃，是我的职业素养。\r\n　　我是李沐，用着最废物的技能，干着最艰难的工作！\r\n　　我是最强大（邪恶）的圆梦师，擅长帮你实现梦想（更擅","CName":"科幻灵异","Score":9.2},{"Id":618211,"Name":"我的治愈系游戏","Author":"我会修空调","Img":"wodezhiyuxiyouxi.jpg","Desc":"警察同志，如果我说这是一款休闲治愈系游戏，你们信吗？","CName":"玄幻奇幻","Score":9.0},{"Id":630009,"Name":"星门","Author":"老鹰吃小鸡","Img":"xingmen.jpg","Desc":"传说，在那古老的星空深处，伫立着一道血与火侵染的红色之门。\r\n　　传奇与神话，黑暗与光明，无尽传说皆在这古老的门户中流淌。\r\n　　俯瞰星门，热血照耀天地，黑暗终将离去！","CName":"玄幻奇幻","Score":9.0},{"Id":17779,"Name":"万古神帝","Author":"飞天鱼","Img":"wangushendi.jpg","Desc":"【NEXTIDEA暨2015星创奖征文大赏（玄幻）】\r\n　　\r\n　　    八百年前，明帝之子张若尘，被他的未婚妻池瑶公主杀死，一代无上天骄，就此陨落。\r\n　　\r\n　　    八百年后，张若尘重新活了过来，却发现曾经杀死他的未婚妻，已经统一昆仑界，开辟出第一中央帝国，号称“池瑶女皇”。\r\n　　\r\n　　    池瑶女皇——统御天下，威临八方；青春永驻，不死不灭。\r\n　　\r\n　　    张若尘站在诸皇祠堂外，望着池瑶女皇的神像，心中","CName":"玄幻奇幻","Score":9.0},{"Id":632295,"Name":"奥特赘婿","Author":"鸣愿","Img":"aotezhuixu.jpg","Desc":"战神佐菲为了报恩，隐藏身份入赘方家，一路扮猪吃老虎。\\n只是他总是感觉，自己的这位老婆，有亿点点诡异。\\n主角：佐菲。反派：方长/叶紫\\n（本书又名《正义奥特曼必胜！如果结局不好，说明没到结局》）","CName":"玄幻奇幻","Score":9.0},{"Id":251646,"Name":"大魔王","Author":"轻尘大神","Img":"damowang1.jpg","Desc":"卢高斯帝国的突然不宣而战，对曼德帝国可是一大沉重打击，国王希勒下旨，全国紧急总动员，征召大量青壮，组建军队，又从东部战场抽调几个精锐师，以抵御卢高斯帝国的入侵。","CName":"玄幻奇幻","Score":9.0},{"Id":519568,"Name":"泠风浮仙","Author":"方泠然","Img":"lingfengfuxian.jpg","Desc":"夫列子御风而行,泠然善也。\r\n　　且看这风灵少女，踏上仙途，一路披荆斩棘，只为心中执念。","CName":"玄幻奇幻","Score":9.0},{"Id":363483,"Name":"抗日之全能兵王","Author":"寂寞剑客","Img":"kangrizhiquannengbingwang.jpg","Desc":"钟毅，一位来自北部战区天狼突击队的全能兵王，在朱日和的一次演习中，因为遭到己方远程炮火的误伤，灵魂穿越到1937年的淞沪战场，成为金山卫保安队队长，且看钟毅如何带着他的炮灰团，利用现代的作战理念及特战技巧，杀得小鬼子尸横遍野、血流成河！","CName":"历史军事","Score":9.0},{"Id":248872,"Name":"诡秘之主","Author":"爱潜水的乌贼","Img":"guimizhizhu.jpg","Desc":"蒸汽与机械的浪潮中，谁能触及非凡？历史和黑暗的迷雾里，又是谁在耳语？我从诡秘中醒来，睁眼看见这个世界：枪械，大炮，巨舰，飞空艇，差分机；魔药，占卜，诅咒，倒吊人，封印物……光明依旧照耀，神秘从未远离，这是一段“愚者”的传说。","CName":"玄幻奇幻","Score":9.0},{"Id":148025,"Name":"鬼吹灯","Author":"天下霸唱","Img":"guichuideng.jpg","Desc":"鬼吹灯是一个系列形式的文字冒险故事，以一本家传的秘书残卷为引。小说中作者首创历史上四大盗墓门派——摸金、卸岭、发丘、搬山，其中摸金是技术含量最高，规矩最多的门派。“人点烛，鬼吹灯”是传说中摸金派的不传之秘，意为进入古墓之中先在东南角点燃一支蜡烛才能开棺，如果蜡烛熄灭，须速速退出，不可取一物。相传这是祖师爷所定的一条活人与死人的契约，千年传承，不得破。有谚为证：发丘印，摸金符，搬山卸岭寻龙诀；人点烛","CName":"科幻灵异","Score":9.0},{"Id":61,"Name":"雪中悍刀行","Author":"烽火戏诸侯","Img":"61.jpg","Desc":"雪中悍刀行最新章节列：小说《雪中悍刀行》烽火戏诸侯/著,雪中悍刀行全文阅读这个江湖。有武夫自称天下第二一甲子。有剑仙一剑破甲两千六。有胆小的骑牛道士肩扛两道。但一样是这个江湖，可能是江湖儿郎江湖死，才初......","CName":"玄幻奇幻","Score":8.9},{"Id":560093,"Name":"白骨大圣","Author":"咬火","Img":"baigudasheng.jpg","Desc":"死人沾地，活人娶尸，老狗刨坟，吃活人饭，阴人问路，知道碰上其中一个意味着什么吗？\r\n　　「已有2万均订作品《这里有妖气》」\r\n　　「《这里有妖气》漫画改编版权已卖出」\r\n　　「《这里有妖气》漫画已上线，可在腾讯动漫、起点漫画、B站漫画阅读」\r\n　　书友①群：608548874；\r\n　　书友②群：760859432。","CName":"玄幻奇幻","Score":8.7},{"Id":573941,"Name":"没钱上大学的我只能去屠龙了","Author":"宇宙无敌水哥","Img":"meiqianshangdaxuedewozhinengqutulongle.jpg","Desc":"总之岁月漫长，然而值得等待。\r\n　　林年等了十六年，等到了卡塞尔之门的召唤，等来荒诞无稽、热血放纵的青春。","CName":"玄幻奇幻","Score":8.7},{"Id":626204,"Name":"夜的命名术","Author":"会说话的肘子","Img":"yedemingmingshu.jpg","Desc":"蓝与紫的霓虹中，浓密的钢铁苍穹下，数据洪流的前端，是科技革命之后的世界，也是现实与虚幻的分界。钢铁与身体，过去与未来。这里，表世界与里世界并存，面前的一切，像是时间之墙近在眼前。黑暗逐渐笼罩。可你要明白啊我的朋友，我们不能用温柔去应对黑暗，要用火。","CName":"玄幻奇幻","Score":8.7},{"Id":630600,"Name":"黎明之劫","Author":"花还没开","Img":"limingzhijie.jpg","Desc":"在做了很久奇怪的梦之后，陆安以为自己病了。\r\n　　……直到这天，有一个莫名其妙的少女出现在他家中，到处嫌弃了一番“古代”生活，她说自己来自未来。\r\n　　然后陆安报警把她抓了。","CName":"科幻灵异","Score":8.7},{"Id":601830,"Name":"十方武圣","Author":"滚开","Img":"shifangwusheng.jpg","Desc":"末日荒土，世宗三年，天下大乱，民不聊生。\r\n　　中央皇朝崩坏，各地群雄割据，门派独立。魔门妖党隐于暗处作乱，帮派相互征伐，混乱不堪。\r\n　　天灾连连，大旱，酷寒，暴雨，虫灾，人民苦苦挣扎，渴求希望与救赎。\r\n　　大乱之中，各门各派纷纷出世，争夺资源地盘，建立独属于自己的统治。\r\n　　有野心者试图席卷天下，建立王朝，也有大义者，意图挽救苍生，重建家园。\r\n　　肌肉，武道，仙法，一位位武道极限强者，在","CName":"玄幻奇幻","Score":8.7},{"Id":624733,"Name":"道友，买把加特林吗？","Author":"驿路羁旅","Img":"daoyou，maibajiatelinma？.jpg","Desc":"“墨家机关术很好很棒，但可惜它已经跟不上这个时代的变化了。”\r\n　　差点重生失败，又经历了神奇故事的前军火商，现墨家制器师江夏，提着自己手制废土版魔改猎巫重机枪，对自己的师兄师姐们说：\r\n　　“这小可爱，才象征着未来！”\r\n　　“道友，来把加特林不？”","CName":"网游竞技","Score":8.7}],"Page":1,"HasNext":true}}

### 小说完结榜
GET https://scxs.pigqq.com/top/man/top/over/week/1.html HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
Content-Type: application/x-www-form-urlencoded
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Host: scxs.pigqq.com
Connection: Keep-Alive
Accept-Encoding: gzip

{"status":1,"info":"success","data":{"BookList":[{"Id":521014,"Name":"大奉打更人","Author":"卖报小郎君","Img":"dafengdagengren.jpg","Desc":"这个世界，有儒；有道；有佛；有妖；有术士。\r\n　　警校毕业的许七安幽幽醒来，发现自己身处牢狱之中，三日后流放边陲.....\r\n　　他起初的目的只是自保，顺便在这个没有人权的社会里当个富家翁悠闲度日。\r\n　　......\r\n　　多年后，许七安回首前尘，身后是早已逝去的敌人和朋友，以及累累白骨。\r\n　　滚滚长江东逝水，浪花淘尽英雄，是非成败转头空。\r\n　　青山依旧在，几度夕阳红。\r\n　　PS：本书不悲","CName":"武侠仙侠","Score":9.0},{"Id":5,"Name":"完美世界","Author":"辰东","Img":"5.jpg","Desc":"完美世界最新章节列：小说《完美世界》辰东/著,完美世界全文阅读完美世界是辰东写的东方玄幻类小说..........","CName":"玄幻奇幻","Score":9.0},{"Id":627409,"Name":"云边有个小卖部","Author":"张嘉佳","Img":"yunbianyougexiaomaibu.jpg","Desc":"张嘉佳全新作品。畅销千万现象级作品《从你的全世界路过》后，暌违五年，写给离开我们的人，写给陪伴我们的人，写给每个人心中的山和海。\\n希望和悲伤，都是一缕光。总有一天，我们会再相遇。\\n让刘十三陪着你，走进云边镇的春夏秋冬，见证每一场相遇与离别。“有些人刻骨铭心，没几年会遗忘。有些人不论生死，都陪在身旁。”\\n满镇开着桔梗，蒲公英飞得比石榴树还高，一直飘进山","CName":"都市言情","Score":9.5},{"Id":584678,"Name":"全球迈入神话时代","Author":"最终永恒","Img":"quanqiumairushenhuashidai.jpg","Desc":"平静的生活中，陆一鸣突然拥有了超能力，原本以为自己即将迈向人生巅峰，却发现整个世界已经发生了翻天覆地的变化！\r\n　　古老的传说成为现实，神秘的预言被不断验证，武功、魔法、修仙、妖魔、鬼怪等各种超自然现象依次出现在世人面前。\r\n　　旧有的秩序崩塌了，人类即将迎来一个全新的时代……神话时代！","CName":"科幻灵异","Score":7.6},{"Id":8975,"Name":"全职法师","Author":"乱","Img":"quanzhifashi.jpg","Desc":"一觉醒来，世界大变。\r\n　　\r\n　　    熟悉的高中传授的是魔法，告诉大家要成为一名出色的魔法师。\r\n　　\r\n　　    居住的都市之外游荡着袭击人类的魔物妖兽，虎视眈眈。\r\n　　\r\n　　    崇尚科学的世界变成了崇尚魔法，偏偏有着一样以学渣看待自己的老师，一样目光异样的同学，一样社会底层挣扎的爸爸，一样纯美却不能走路的非血缘妹妹……\r\n　　\r\n　　    不过，莫凡发现绝大多数人都只能够主修一系魔法，自己却","CName":"玄幻奇幻","Score":8.6},{"Id":600715,"Name":"我家老婆来自一千年前","Author":"花还没开","Img":"wojialaopolaiziyiqiannianqian.jpg","Desc":"“我想回家。”\r\n　　“你可能回不去了。”\r\n　　“为什么？”\r\n　　“因为这里离你家很远。”\r\n　　“有多远？”\r\n　　“一千二百多年那么远。”\r\n　　许青看着眼前来自唐朝的少女，脸上带有一丝同情：“你所熟悉的一切，都已经变成历史。”\r\n　　亲朋，好友，敌人，全部沉寂在一千二百年前。\r\n　　———\r\n　　日常文，单女主\r\n　　（已有完本精品，质量保证。）","CName":"都市言情","Score":9.7},{"Id":412435,"Name":"第一序列","Author":"会说话的肘子","Img":"diyixulie.jpg","Desc":"这是任小粟大魔王出现了吗？画风都不带变的吗？是新一代话题终结者吗？肘星人准备好了吗？想知道大魔王是如何练成的吗？让我们在2019年4月15日一起迎接新的世界吧，看看肘子如何喷翻全场！！","CName":"玄幻奇幻","Score":8.7},{"Id":3196,"Name":"死人经","Author":"冰临神下","Img":"sirenjing.jpg","Desc":"为不善乎显明之中者，人得而诛之；为不善于幽闭之中者，鬼得而诛之。人鬼不诛，神得而诛之。一本死人经，半部无道书。斩尽千人头，啖吞百身骨。你要么忍受世界的不公，要么成为世界的主宰。他选择成为杀手，和仇人一样的杀手，但是更加冷酷更无情。刀光剑影中，他要寻求真理——杀生者不死，生生者不生。","CName":"武侠仙侠","Score":8.9},{"Id":630195,"Name":"我于世间全无敌","Author":"陆鹏","Img":"woyushijianquanwudi.jpg","Desc":"路一平是个上古修士，亲眼见证了诸神大战中，无数强大的神灵殒落的情景。自此之后，他便躲在深山老林，日夜修炼，发誓没有强大到对抗天地大劫的实力时，便不出来。一个时代又一个时代过去了。他身边的一头小蛇，成为了龙族之祖。他收养过的一个小女孩，成了无敌女帝。他指点过的一个剑客，成了名响万古的剑神。他随意种下的一棵老树，成了史上最强神国的守护之神。沧海桑","CName":"玄幻奇幻","Score":3.7},{"Id":3143,"Name":"斗破苍穹","Author":"天蚕土豆","Img":"doupocangqiong.jpg","Desc":"这里是属于斗气的世界，没有花俏艳丽的魔法，有的，仅仅是繁衍到巅峰的斗气！新书刚开，请各位兄弟多多支持，用推荐票和收藏，砸烂偶吧.^_^新书等级制度：斗者，斗师，大斗师，斗灵，斗王，斗皇，斗宗，斗尊，斗圣，斗帝。","CName":"玄幻奇幻","Score":8.1},{"Id":1559,"Name":"斗罗大陆","Author":"唐家三少","Img":"douluodalu.jpg","Desc":"【小三新书《阴阳冕》已经注册】将会在本周日，斗罗大陆结束的同时开始上传更新，麻烦大家先收藏、推荐一下，谢谢。阴阳冕书号：1436015下面的直通车也可以直接点过去。【小三出品，必属精品，全新设定，酬谢书友】target=&_blank&","CName":"玄幻奇幻","Score":4.6},{"Id":140456,"Name":"超神机械师","Author":"齐佩甲","Img":"chaoshenjixieshi.jpg","Desc":"韩萧，《星海》骨灰级代练，被来自东（zuo）方(zhe)的神秘力量扔进穿越大军，携带玩家面板变成NPC，回到《星海》公测之前，毅然选择难度最高的机械系。\r\n　　战舰列队纵横星海，星辰机甲夭矫如龙，幽能炮毁天灭地，还有无边无际的机械大军，静静待在随身仓库里。\r\n　　一人，即是军团！\r\n　　如果不是玩家出现，本书就是正经严肃的穿越异界题材……\r\n　　作为NPC，正常NPC对玩家功能一应俱全……发布任务","CName":"网游竞技","Score":9.4},{"Id":627885,"Name":"迎娶女帝之后","Author":"老狗","Img":"yingqunvdizhihou.jpg","Desc":"李云没有想到，穿越到这个世界后的第一件事，就是被迫卷入造反的大军。大乾九百七十六年，居于大陆之央的大乾终于镇压了这场大陆千年来规模最大，影响力最深的叛乱，平四方，镇气运。同年，大乾老皇帝驾崩，新帝登基，整个世界的命运都被掌握在这位新的至高权力者手上，无人能够逃过。","CName":"玄幻奇幻","Score":8.0},{"Id":377500,"Name":"斗罗大陆IV终极斗罗","Author":"唐家三少","Img":"douluodaluIVzhongjidouluo.jpg","Desc":"一万年后，冰化了。\r\n　　斗罗联邦科考队在极北之地科考时发现了一个有着金银双色花纹的蛋，用仪器探察之后，发现里面居然有生命体征，赶忙将其带回研究所进行孵化。蛋孵化出来了，可孵出来的却是一个婴儿，和人类一模一样的婴儿，一个蛋生的孩子。","CName":"玄幻奇幻","Score":2.8},{"Id":24328,"Name":"非正常人类异闻录","Author":"精分三代","Img":"feizhengchangrenleiyiwenlu.jpg","Desc":"我叫张大道，道号张全道。在第七人民医院被人研究！\r\n　　\r\n　　    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\r\n　　\r\n　　    贫道张全道，专业摸骨批命，棺材翻新,抛光,打蜡。回收二手僵尸,寻龙点穴、批发黑驴蹄、黑狗血。代写1~3年级小学作业，寻找走失猫狗，抓小三。\r\n　　\r\n　　    专业报仇打小人、改风水、妨祖坟！量大从优！有发票！\r\n　　\r\n　　    ~~~~~","CName":"都市言情","Score":9.5},{"Id":3051,"Name":"遮天","Author":"辰东","Img":"zhetian.jpg","Desc":"冰冷与黑暗并存的宇宙深处，九具庞大的龙尸拉着一口青铜古棺，亘古长存。这是太空探测器在枯寂的宇宙中捕捉到的一幅极其震撼的画面。九龙拉棺，究竟是回到了上古，还是来到了星空的彼岸？一个浩大的仙侠世界，光怪陆离，神秘无尽。热血似火山沸腾，激情若瀚海汹涌，欲望如深渊无止境……登天路，踏歌行，弹指遮天。","CName":"武侠仙侠","Score":8.6},{"Id":292949,"Name":"我有一座恐怖屋","Author":"我会修空调","Img":"woyouyizuokongbuwu.jpg","Desc":"散发异味的灵车停在了门口，天花板传来弹珠碰撞的声音，走廊里有人来回踱步，隔壁房间好像在切割什么东西。\r\n　　卧室的门锁轻轻颤动，卫生间里水龙头已经拧紧，却还是滴答滴答个不停。\r\n　　床底下隐隐约约，似乎有个皮球滚来滚去。\r\n　　一个个沾染水渍的脚印不断在地板上浮现，正慢慢逼近。\r\n　　凌晨三点，陈歌握着菜刀躲在暖气片旁边，手里的电话刚刚拨通。\r\n　　“房东！这就是你说的晚上有点热闹？！”","CName":"科幻灵异","Score":9.5},{"Id":78031,"Name":"一念永恒","Author":"耳根","Img":"yinianyongheng.jpg","Desc":"一念成沧海，一念化桑田。一念斩千魔，一念诛万仙。唯我念……永恒","CName":"武侠仙侠","Score":8.3},{"Id":248872,"Name":"诡秘之主","Author":"爱潜水的乌贼","Img":"guimizhizhu.jpg","Desc":"蒸汽与机械的浪潮中，谁能触及非凡？历史和黑暗的迷雾里，又是谁在耳语？我从诡秘中醒来，睁眼看见这个世界：枪械，大炮，巨舰，飞空艇，差分机；魔药，占卜，诅咒，倒吊人，封印物……光明依旧照耀，神秘从未远离，这是一段“愚者”的传说。","CName":"玄幻奇幻","Score":9.2},{"Id":512195,"Name":"万族之劫","Author":"老鹰吃小鸡","Img":"wanzuzhijie.jpg","Desc":"我是这诸天万族的劫！\r\n　　已有完本作品《全球高武》《重生之财源滚滚》，没看过的书友可以去看看，新书收藏一下慢慢养。","CName":"都市言情","Score":8.1},{"Id":2802,"Name":"星辰变","Author":"我吃西红柿","Img":"xingchenbian.jpg","Desc":"一名孩童，天生无法修炼内功。为了得到父亲的重视关注，他毅然选择了修炼痛苦艰难的外功。春去秋来，时光如梭，这个孩童长大了……变成了一名青年，真正改变他的命运，是一颗流星化作的神秘晶石——流星泪。这颗流星泪在青年无所觉中，融入了青年的体内，青年他也仿佛破茧化蝶一般蜕变……而随之而来的，一切都发生了变化。而他的父亲也终于知道了他从来没有真正倾注心力的儿子的惊人实力……《星辰变》将改编成网游《星","CName":"武侠仙侠","Score":8.1}],"Page":1,"HasNext":true}}

### 小说热更榜
GET https://scxs.pigqq.com/top/man/top/hot/week/1.html HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
Content-Type: application/x-www-form-urlencoded
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Host: scxs.pigqq.com
Connection: Keep-Alive
Accept-Encoding: gzip

{"status":1,"info":"success","data":{"BookList":[{"Id":628547,"Name":"不科学御兽","Author":"轻泉流响","Img":"bukexueyushou.jpg","Desc":"这是一个以御兽为主流的异世界。\r\n　　当时宇携带技能图鉴穿越到这里，并培育出一堆奇葩宠兽后，所有御兽师的三观都破碎了……\r\n　　关键词：御兽、宠兽、宠物、召唤。","CName":"玄幻奇幻","Score":9.0},{"Id":630046,"Name":"我就是神！","Author":"历史里吹吹风","Img":"wojiushishen_.jpg","Desc":"尹神的名字叫神。\r\n　　他从来没有想过，有一天自己会真的成为神。","CName":"玄幻奇幻","Score":8.3},{"Id":630009,"Name":"星门","Author":"老鹰吃小鸡","Img":"xingmen.jpg","Desc":"传说，在那古老的星空深处，伫立着一道血与火侵染的红色之门。\r\n　　传奇与神话，黑暗与光明，无尽传说皆在这古老的门户中流淌。\r\n　　俯瞰星门，热血照耀天地，黑暗终将离去！","CName":"玄幻奇幻","Score":8.8},{"Id":623334,"Name":"斗罗大陆5重生唐三","Author":"唐家三少","Img":"douluodalu5zhongshengtangsan.jpg","Desc":"一代神王唐三，因为妻子的死而选择了殉情，带着一点神识在宇宙中遨游，寻找妻子转世重生的世界。在神识的牵引下，他来到了一个叫作妖精大陆的地方，寻找他的妻子小舞。而他却发现，这是一个人类为刍狗的世界······","CName":"玄幻奇幻","Score":1.4},{"Id":628100,"Name":"当青春幻想具现后","Author":"转角吻猪","Img":"dangqingchunhuanxiangjuxianhou.jpg","Desc":"当时间停止一小时，只有你可以自由移动时，你会做什么？\r\n　　谢邀，这问题别问我啊！你问她——\r\n　　对！就是这个趁着时间停止来到我身边，朝我伸出手的女孩！\r\n　　------\r\n　　时间停止、返老还童、时空电话、猫的报恩……当青春里出现一件又一件荒唐而又神奇的事件时，我们的故事开始了。\r\n　　（关键词：幻想具现、日常、恋爱）","CName":"都市言情","Score":9.2},{"Id":631387,"Name":"开局：一个民国位面","Author":"龙升云霄","Img":"kaijuyigeminguoweimian.jpg","Desc":"如果你能往返一个‘特殊’的民国世界，你会做什么？\r\n　　富甲天下，妻妾成群？\r\n　　提笔报国，文压天下？\r\n　　秣马厉兵，封王拜将？\r\n　　还是...\r\n　　练得身形似鹤形，千株松下两函经。\r\n　　我来问道无余说，云在青天水在瓶。\r\n　　ps：本书又名《诸天：从民国开始》。","CName":"科幻灵异","Score":8.8},{"Id":620881,"Name":"这个人仙太过正经","Author":"言归正传","Img":"zheigerenxiantaiguozhengjing.jpg","Desc":"2月5号，新书《这个人仙太过正经》就要跟各位读者老爷见面了！半神之躯，比肩凡人！正经人仙，在线薅神！","CName":"玄幻奇幻","Score":8.3},{"Id":627854,"Name":"大秦：不装了，你爹我是秦始皇","Author":"头顶一只喵喵","Img":"daqin_buzhuangle_nidiewoshiqinshihuang.jpg","Desc":"赵浪一觉醒来，发现自己来到了秦朝。\r\n　　好在家境还算富裕。\r\n　　只是算了算时间，大秦只有三年的寿命，赵浪便鼓起勇气，和自己那几个月才回来一次的便宜老爹说道，\r\n　　“爹，始皇帝三年之后必死，大秦将亡，到时候天下大乱，我们早做准备造反吧！”\r\n　　便宜老爹先是一愣，随后点头同意。\r\n　　赵浪顿时兴教育，练新军。\r\n　　就当他羽翼丰满，准备天下争雄时。\r\n　　便宜老爹突然来到了他的面前，\r\n　　“","CName":"历史军事","Score":7.3},{"Id":626204,"Name":"夜的命名术","Author":"会说话的肘子","Img":"yedemingmingshu.jpg","Desc":"蓝与紫的霓虹中，浓密的钢铁苍穹下，数据洪流的前端，是科技革命之后的世界，也是现实与虚幻的分界。钢铁与身体，过去与未来。这里，表世界与里世界并存，面前的一切，像是时间之墙近在眼前。黑暗逐渐笼罩。可你要明白啊我的朋友，我们不能用温柔去应对黑暗，要用火。","CName":"玄幻奇幻","Score":8.7},{"Id":630133,"Name":"机械炼金术士","Author":"盲候","Img":"jixielianjinshushi.jpg","Desc":"幽暗的地下城，这里埋藏了数之不尽的古代遗迹和宝藏。\r\n　　诡异，畸变，诅咒物...\r\n　　深渊，地窟，古神，神话种族...\r\n　　机械师，咒印植装，巨城黑塔...\r\n　　千奇百怪炼金术，添一勺蒸汽朋克，两勺诡秘超凡，杂糅出了一个缤纷多彩的奇幻世界。\r\n　　我，傀儡炼金术士。\r\n　　一人，便是军团！","CName":"网游竞技","Score":9.6},{"Id":626698,"Name":"深空彼岸","Author":"辰东","Img":"shenkongbian.jpg","Desc":"浩瀚的宇宙中，一片星系的生灭，也不过是刹那的斑驳流光。仰望星空，总有种结局已注定的伤感，千百年后你我在哪里？家国，文明火光，地球，都不过是深空中的一粒尘埃。星空一瞬，人间千年。虫鸣一世不过秋，你我一样在争渡。深空尽头到底有什么？","CName":"玄幻奇幻","Score":8.5},{"Id":625913,"Name":"万相之王","Author":"天蚕土豆","Img":"wanxiangzhiwang.jpg","Desc":"天地间，有万相。而我李洛，终将成为这万相之王。","CName":"玄幻奇幻","Score":4.7},{"Id":17779,"Name":"万古神帝","Author":"飞天鱼","Img":"wangushendi.jpg","Desc":"【NEXTIDEA暨2015星创奖征文大赏（玄幻）】\r\n　　\r\n　　    八百年前，明帝之子张若尘，被他的未婚妻池瑶公主杀死，一代无上天骄，就此陨落。\r\n　　\r\n　　    八百年后，张若尘重新活了过来，却发现曾经杀死他的未婚妻，已经统一昆仑界，开辟出第一中央帝国，号称“池瑶女皇”。\r\n　　\r\n　　    池瑶女皇——统御天下，威临八方；青春永驻，不死不灭。\r\n　　\r\n　　    张若尘站在诸皇祠堂外，望着池瑶女皇的神像，心中","CName":"玄幻奇幻","Score":8.1},{"Id":623345,"Name":"顶级气运，悄悄修炼千年","Author":"任我笑","Img":"dingjiqiyun，qiaoqiaoxiulianqiannian.jpg","Desc":"转世来到修仙世界，韩绝发现自己带着游戏属性，竟然可以摇骰子刷新灵根资质与先天气运。\r\n　　于是乎，他花了十一年摇先天气运。\r\n　　【绝世无双：仙姿，魅力顶级】\r\n　　【天命剑痴：剑道资质顶级，剑道悟性顶级】\r\n　　【身法绝尘：身法资质顶级】\r\n　　【仙帝后裔：获得一部绝世修仙功法、一千块上品灵石】\r\n　　韩绝为了长生，决定悄悄修炼，不出风头。\r\n　　千年后，修真界一代换一代。\r\n　　当仙界清理凡间","CName":"武侠仙侠","Score":7.2},{"Id":632295,"Name":"奥特赘婿","Author":"鸣愿","Img":"aotezhuixu.jpg","Desc":"战神佐菲为了报恩，隐藏身份入赘方家，一路扮猪吃老虎。\\n只是他总是感觉，自己的这位老婆，有亿点点诡异。\\n主角：佐菲。反派：方长/叶紫\\n（本书又名《正义奥特曼必胜！如果结局不好，说明没到结局》）","CName":"玄幻奇幻","Score":8.3},{"Id":622896,"Name":"弃宇宙","Author":"鹅是老五","Img":"qiyuzhou.jpg","Desc":"地球元气复苏了，但这真不是地球灵气复苏的故事，\r\n　　而是一个流浪宇宙的故事。","CName":"武侠仙侠","Score":5.3},{"Id":620826,"Name":"我的七个姐姐风华绝代","Author":"无言会语","Img":"wodeqigejiejiefenghuajuedai.jpg","Desc":"大姐莫向晚，霸道总裁……二姐白吟霜，国际杀手……三姐沈冰，国际空姐……四姐顾心怡，拥有绝世医术……五姐罗晓，有名的警花……六姐罗娜，拥有神秘的身份……七姐叶凝云，绝代影后……","CName":"都市言情","Score":2.0},{"Id":3230,"Name":"逆天邪神","Author":"火星引力","Img":"nitianxieshen.jpg","Desc":"掌天毒之珠，承邪神之血，修逆天之力，一代邪神，君临天下！【添加微信公众号：火星引力】【我们的YY频道：49554】......","CName":"玄幻奇幻","Score":8.0},{"Id":147613,"Name":"轮回乐园","Author":"那一只蚊子","Img":"lunhuileyuan.jpg","Desc":"机遇与危险共存，只要豁出性命，在轮回乐园中就能得到一切。\r\n　　被轮回乐园选中成为猎杀者的那一刻，苏晓就明白，他将与所有人为敌。\r\n　　乐园虽然残酷，但无所不能……。","CName":"玄幻奇幻","Score":6.3},{"Id":618211,"Name":"我的治愈系游戏","Author":"我会修空调","Img":"wodezhiyuxiyouxi.jpg","Desc":"警察同志，如果我说这是一款休闲治愈系游戏，你们信吗？","CName":"玄幻奇幻","Score":9.1},{"Id":616967,"Name":"我在斩妖司除魔三十年","Author":"贰更","Img":"wozaizhanyaosichumosanshinian.jpg","Desc":"一觉醒来，周易成了大乾斩妖司的行刑官。\r\n　　恰逢妖魔乱世，鬼怪横行，乾坤剧变。\r\n　　周易躲在斩妖司，每天行刑妖魔获得各种奖励。\r\n　　黄庭道经、紫郢仙剑、蟠桃灵根、五色神牛、天罡法术、地煞神通……\r\n　　九天十地，漫漫仙道，吾当掌教尊！","CName":"武侠仙侠","Score":7.8}],"Page":1,"HasNext":true}}

### 小说 热门连载 更多
GET https://scxs.pysmei.com/top/man/top/hot/week/1.html HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
Content-Type: application/x-www-form-urlencoded
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Host: scxs.pysmei.com
Connection: Keep-Alive
Accept-Encoding: gzip

{"status":1,"info":"success","data":{"BookList":[{"Id":628547,"Name":"不科学御兽","Author":"轻泉流响","Img":"bukexueyushou.jpg","Desc":"这是一个以御兽为主流的异世界。\r\n　　当时宇携带技能图鉴穿越到这里，并培育出一堆奇葩宠兽后，所有御兽师的三观都破碎了……\r\n　　关键词：御兽、宠兽、宠物、召唤。","CName":"玄幻奇幻","Score":9.0},{"Id":630046,"Name":"我就是神！","Author":"历史里吹吹风","Img":"wojiushishen_.jpg","Desc":"尹神的名字叫神。\r\n　　他从来没有想过，有一天自己会真的成为神。","CName":"玄幻奇幻","Score":8.3},{"Id":630009,"Name":"星门","Author":"老鹰吃小鸡","Img":"xingmen.jpg","Desc":"传说，在那古老的星空深处，伫立着一道血与火侵染的红色之门。\r\n　　传奇与神话，黑暗与光明，无尽传说皆在这古老的门户中流淌。\r\n　　俯瞰星门，热血照耀天地，黑暗终将离去！","CName":"玄幻奇幻","Score":8.8},{"Id":623334,"Name":"斗罗大陆5重生唐三","Author":"唐家三少","Img":"douluodalu5zhongshengtangsan.jpg","Desc":"一代神王唐三，因为妻子的死而选择了殉情，带着一点神识在宇宙中遨游，寻找妻子转世重生的世界。在神识的牵引下，他来到了一个叫作妖精大陆的地方，寻找他的妻子小舞。而他却发现，这是一个人类为刍狗的世界······","CName":"玄幻奇幻","Score":1.4},{"Id":628100,"Name":"当青春幻想具现后","Author":"转角吻猪","Img":"dangqingchunhuanxiangjuxianhou.jpg","Desc":"当时间停止一小时，只有你可以自由移动时，你会做什么？\r\n　　谢邀，这问题别问我啊！你问她——\r\n　　对！就是这个趁着时间停止来到我身边，朝我伸出手的女孩！\r\n　　------\r\n　　时间停止、返老还童、时空电话、猫的报恩……当青春里出现一件又一件荒唐而又神奇的事件时，我们的故事开始了。\r\n　　（关键词：幻想具现、日常、恋爱）","CName":"都市言情","Score":9.2},{"Id":631387,"Name":"开局：一个民国位面","Author":"龙升云霄","Img":"kaijuyigeminguoweimian.jpg","Desc":"如果你能往返一个‘特殊’的民国世界，你会做什么？\r\n　　富甲天下，妻妾成群？\r\n　　提笔报国，文压天下？\r\n　　秣马厉兵，封王拜将？\r\n　　还是...\r\n　　练得身形似鹤形，千株松下两函经。\r\n　　我来问道无余说，云在青天水在瓶。\r\n　　ps：本书又名《诸天：从民国开始》。","CName":"科幻灵异","Score":8.8},{"Id":620881,"Name":"这个人仙太过正经","Author":"言归正传","Img":"zheigerenxiantaiguozhengjing.jpg","Desc":"2月5号，新书《这个人仙太过正经》就要跟各位读者老爷见面了！半神之躯，比肩凡人！正经人仙，在线薅神！","CName":"玄幻奇幻","Score":8.3},{"Id":627854,"Name":"大秦：不装了，你爹我是秦始皇","Author":"头顶一只喵喵","Img":"daqin_buzhuangle_nidiewoshiqinshihuang.jpg","Desc":"赵浪一觉醒来，发现自己来到了秦朝。\r\n　　好在家境还算富裕。\r\n　　只是算了算时间，大秦只有三年的寿命，赵浪便鼓起勇气，和自己那几个月才回来一次的便宜老爹说道，\r\n　　“爹，始皇帝三年之后必死，大秦将亡，到时候天下大乱，我们早做准备造反吧！”\r\n　　便宜老爹先是一愣，随后点头同意。\r\n　　赵浪顿时兴教育，练新军。\r\n　　就当他羽翼丰满，准备天下争雄时。\r\n　　便宜老爹突然来到了他的面前，\r\n　　“","CName":"历史军事","Score":7.3},{"Id":626204,"Name":"夜的命名术","Author":"会说话的肘子","Img":"yedemingmingshu.jpg","Desc":"蓝与紫的霓虹中，浓密的钢铁苍穹下，数据洪流的前端，是科技革命之后的世界，也是现实与虚幻的分界。钢铁与身体，过去与未来。这里，表世界与里世界并存，面前的一切，像是时间之墙近在眼前。黑暗逐渐笼罩。可你要明白啊我的朋友，我们不能用温柔去应对黑暗，要用火。","CName":"玄幻奇幻","Score":8.7},{"Id":630133,"Name":"机械炼金术士","Author":"盲候","Img":"jixielianjinshushi.jpg","Desc":"幽暗的地下城，这里埋藏了数之不尽的古代遗迹和宝藏。\r\n　　诡异，畸变，诅咒物...\r\n　　深渊，地窟，古神，神话种族...\r\n　　机械师，咒印植装，巨城黑塔...\r\n　　千奇百怪炼金术，添一勺蒸汽朋克，两勺诡秘超凡，杂糅出了一个缤纷多彩的奇幻世界。\r\n　　我，傀儡炼金术士。\r\n　　一人，便是军团！","CName":"网游竞技","Score":9.6},{"Id":626698,"Name":"深空彼岸","Author":"辰东","Img":"shenkongbian.jpg","Desc":"浩瀚的宇宙中，一片星系的生灭，也不过是刹那的斑驳流光。仰望星空，总有种结局已注定的伤感，千百年后你我在哪里？家国，文明火光，地球，都不过是深空中的一粒尘埃。星空一瞬，人间千年。虫鸣一世不过秋，你我一样在争渡。深空尽头到底有什么？","CName":"玄幻奇幻","Score":8.5},{"Id":625913,"Name":"万相之王","Author":"天蚕土豆","Img":"wanxiangzhiwang.jpg","Desc":"天地间，有万相。而我李洛，终将成为这万相之王。","CName":"玄幻奇幻","Score":4.7},{"Id":17779,"Name":"万古神帝","Author":"飞天鱼","Img":"wangushendi.jpg","Desc":"【NEXTIDEA暨2015星创奖征文大赏（玄幻）】\r\n　　\r\n　　    八百年前，明帝之子张若尘，被他的未婚妻池瑶公主杀死，一代无上天骄，就此陨落。\r\n　　\r\n　　    八百年后，张若尘重新活了过来，却发现曾经杀死他的未婚妻，已经统一昆仑界，开辟出第一中央帝国，号称“池瑶女皇”。\r\n　　\r\n　　    池瑶女皇——统御天下，威临八方；青春永驻，不死不灭。\r\n　　\r\n　　    张若尘站在诸皇祠堂外，望着池瑶女皇的神像，心中","CName":"玄幻奇幻","Score":8.1},{"Id":623345,"Name":"顶级气运，悄悄修炼千年","Author":"任我笑","Img":"dingjiqiyun，qiaoqiaoxiulianqiannian.jpg","Desc":"转世来到修仙世界，韩绝发现自己带着游戏属性，竟然可以摇骰子刷新灵根资质与先天气运。\r\n　　于是乎，他花了十一年摇先天气运。\r\n　　【绝世无双：仙姿，魅力顶级】\r\n　　【天命剑痴：剑道资质顶级，剑道悟性顶级】\r\n　　【身法绝尘：身法资质顶级】\r\n　　【仙帝后裔：获得一部绝世修仙功法、一千块上品灵石】\r\n　　韩绝为了长生，决定悄悄修炼，不出风头。\r\n　　千年后，修真界一代换一代。\r\n　　当仙界清理凡间","CName":"武侠仙侠","Score":7.2},{"Id":632295,"Name":"奥特赘婿","Author":"鸣愿","Img":"aotezhuixu.jpg","Desc":"战神佐菲为了报恩，隐藏身份入赘方家，一路扮猪吃老虎。\\n只是他总是感觉，自己的这位老婆，有亿点点诡异。\\n主角：佐菲。反派：方长/叶紫\\n（本书又名《正义奥特曼必胜！如果结局不好，说明没到结局》）","CName":"玄幻奇幻","Score":8.3},{"Id":622896,"Name":"弃宇宙","Author":"鹅是老五","Img":"qiyuzhou.jpg","Desc":"地球元气复苏了，但这真不是地球灵气复苏的故事，\r\n　　而是一个流浪宇宙的故事。","CName":"武侠仙侠","Score":5.3},{"Id":620826,"Name":"我的七个姐姐风华绝代","Author":"无言会语","Img":"wodeqigejiejiefenghuajuedai.jpg","Desc":"大姐莫向晚，霸道总裁……二姐白吟霜，国际杀手……三姐沈冰，国际空姐……四姐顾心怡，拥有绝世医术……五姐罗晓，有名的警花……六姐罗娜，拥有神秘的身份……七姐叶凝云，绝代影后……","CName":"都市言情","Score":2.0},{"Id":3230,"Name":"逆天邪神","Author":"火星引力","Img":"nitianxieshen.jpg","Desc":"掌天毒之珠，承邪神之血，修逆天之力，一代邪神，君临天下！【添加微信公众号：火星引力】【我们的YY频道：49554】......","CName":"玄幻奇幻","Score":8.0},{"Id":147613,"Name":"轮回乐园","Author":"那一只蚊子","Img":"lunhuileyuan.jpg","Desc":"机遇与危险共存，只要豁出性命，在轮回乐园中就能得到一切。\r\n　　被轮回乐园选中成为猎杀者的那一刻，苏晓就明白，他将与所有人为敌。\r\n　　乐园虽然残酷，但无所不能……。","CName":"玄幻奇幻","Score":6.3},{"Id":618211,"Name":"我的治愈系游戏","Author":"我会修空调","Img":"wodezhiyuxiyouxi.jpg","Desc":"警察同志，如果我说这是一款休闲治愈系游戏，你们信吗？","CName":"玄幻奇幻","Score":9.1},{"Id":616967,"Name":"我在斩妖司除魔三十年","Author":"贰更","Img":"wozaizhanyaosichumosanshinian.jpg","Desc":"一觉醒来，周易成了大乾斩妖司的行刑官。\r\n　　恰逢妖魔乱世，鬼怪横行，乾坤剧变。\r\n　　周易躲在斩妖司，每天行刑妖魔获得各种奖励。\r\n　　黄庭道经、紫郢仙剑、蟠桃灵根、五色神牛、天罡法术、地煞神通……\r\n　　九天十地，漫漫仙道，吾当掌教尊！","CName":"武侠仙侠","Score":7.8}],"Page":1,"HasNext":true}}

### 小说 抖音热书 更多
GET https://scxs.pysmei.com/top/man/top/collect/week/1.html HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
Content-Type: application/x-www-form-urlencoded
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Host: scxs.pysmei.com
Connection: Keep-Alive
Accept-Encoding: gzip

{"status":1,"info":"success","data":{"BookList":[{"Id":625913,"Name":"万相之王","Author":"天蚕土豆","Img":"wanxiangzhiwang.jpg","Desc":"天地间，有万相。而我李洛，终将成为这万相之王。","CName":"玄幻奇幻","Score":4.7},{"Id":521014,"Name":"大奉打更人","Author":"卖报小郎君","Img":"dafengdagengren.jpg","Desc":"这个世界，有儒；有道；有佛；有妖；有术士。\r\n　　警校毕业的许七安幽幽醒来，发现自己身处牢狱之中，三日后流放边陲.....\r\n　　他起初的目的只是自保，顺便在这个没有人权的社会里当个富家翁悠闲度日。\r\n　　......\r\n　　多年后，许七安回首前尘，身后是早已逝去的敌人和朋友，以及累累白骨。\r\n　　滚滚长江东逝水，浪花淘尽英雄，是非成败转头空。\r\n　　青山依旧在，几度夕阳红。\r\n　　PS：本书不悲","CName":"武侠仙侠","Score":9.0},{"Id":620881,"Name":"这个人仙太过正经","Author":"言归正传","Img":"zheigerenxiantaiguozhengjing.jpg","Desc":"2月5号，新书《这个人仙太过正经》就要跟各位读者老爷见面了！半神之躯，比肩凡人！正经人仙，在线薅神！","CName":"玄幻奇幻","Score":8.3},{"Id":618328,"Name":"我什么时候无敌了","Author":"戏柳先生","Img":"woshenmeshihouwudile.jpg","Desc":"【无敌+搞笑+单女主+迪化】他一直以为自己是凡人，却不知院子里堆满了神器，养的鸡更是凤凰！直到在凡人小镇生活了五年，系统终于让他去接触修炼者。这时候他才发现，不管多强的人，见到他那刻，都会吓得腿软，喊他前辈。有甚者，还跪地朝拜......此书偏沙雕无厘头，专治不开心，风格奇特，看完有惊喜哦！","CName":"玄幻奇幻","Score":3.3},{"Id":624842,"Name":"我顿悟了混沌体","Author":"萧云席春雨","Img":"wodunwulehundunti.jpg","Desc":"萧云的系统只会一个功能——顿悟！体质平凡？顿悟混沌体！功法难修？顿悟圆满境界！神通难修？顿悟圆满境界！没有什么是顿悟不能解决的，如果有，那就顿悟十次，百次……","CName":"玄幻奇幻","Score":4.8},{"Id":622896,"Name":"弃宇宙","Author":"鹅是老五","Img":"qiyuzhou.jpg","Desc":"地球元气复苏了，但这真不是地球灵气复苏的故事，\r\n　　而是一个流浪宇宙的故事。","CName":"武侠仙侠","Score":5.3},{"Id":620826,"Name":"我的七个姐姐风华绝代","Author":"无言会语","Img":"wodeqigejiejiefenghuajuedai.jpg","Desc":"大姐莫向晚，霸道总裁……二姐白吟霜，国际杀手……三姐沈冰，国际空姐……四姐顾心怡，拥有绝世医术……五姐罗晓，有名的警花……六姐罗娜，拥有神秘的身份……七姐叶凝云，绝代影后……","CName":"都市言情","Score":2.0},{"Id":624757,"Name":"贞观战神","Author":"李文昊李世民","Img":"zhenguanzhanshen.jpg","Desc":"穿越唐朝，成为不存在历史中的李世民长子。天生痴傻的李文昊终于在李元霸的葬礼上觉醒了。民间传说，将不过李，王不过霸，但是开局摸了天下无敌李元霸的尸体，李文昊会有多猛？惹事，他从来不怕。打架，他从来不虚。作死，他更是一流。拼爹？呵呵！李文昊：“我交朋友从来不看他爹厉不厉害，因为无论他爹多厉害都没有我爹厉害”","CName":"玄幻奇幻","Score":2.6},{"Id":5,"Name":"完美世界","Author":"辰东","Img":"5.jpg","Desc":"完美世界最新章节列：小说《完美世界》辰东/著,完美世界全文阅读完美世界是辰东写的东方玄幻类小说..........","CName":"玄幻奇幻","Score":9.0},{"Id":8975,"Name":"全职法师","Author":"乱","Img":"quanzhifashi.jpg","Desc":"一觉醒来，世界大变。\r\n　　\r\n　　    熟悉的高中传授的是魔法，告诉大家要成为一名出色的魔法师。\r\n　　\r\n　　    居住的都市之外游荡着袭击人类的魔物妖兽，虎视眈眈。\r\n　　\r\n　　    崇尚科学的世界变成了崇尚魔法，偏偏有着一样以学渣看待自己的老师，一样目光异样的同学，一样社会底层挣扎的爸爸，一样纯美却不能走路的非血缘妹妹……\r\n　　\r\n　　    不过，莫凡发现绝大多数人都只能够主修一系魔法，自己却","CName":"玄幻奇幻","Score":8.6},{"Id":3143,"Name":"斗破苍穹","Author":"天蚕土豆","Img":"doupocangqiong.jpg","Desc":"这里是属于斗气的世界，没有花俏艳丽的魔法，有的，仅仅是繁衍到巅峰的斗气！新书刚开，请各位兄弟多多支持，用推荐票和收藏，砸烂偶吧.^_^新书等级制度：斗者，斗师，大斗师，斗灵，斗王，斗皇，斗宗，斗尊，斗圣，斗帝。","CName":"玄幻奇幻","Score":8.1},{"Id":1559,"Name":"斗罗大陆","Author":"唐家三少","Img":"douluodalu.jpg","Desc":"【小三新书《阴阳冕》已经注册】将会在本周日，斗罗大陆结束的同时开始上传更新，麻烦大家先收藏、推荐一下，谢谢。阴阳冕书号：1436015下面的直通车也可以直接点过去。【小三出品，必属精品，全新设定，酬谢书友】target=&_blank&","CName":"玄幻奇幻","Score":4.6},{"Id":623334,"Name":"斗罗大陆5重生唐三","Author":"唐家三少","Img":"douluodalu5zhongshengtangsan.jpg","Desc":"一代神王唐三，因为妻子的死而选择了殉情，带着一点神识在宇宙中遨游，寻找妻子转世重生的世界。在神识的牵引下，他来到了一个叫作妖精大陆的地方，寻找他的妻子小舞。而他却发现，这是一个人类为刍狗的世界······","CName":"玄幻奇幻","Score":1.4},{"Id":628547,"Name":"不科学御兽","Author":"轻泉流响","Img":"bukexueyushou.jpg","Desc":"这是一个以御兽为主流的异世界。\r\n　　当时宇携带技能图鉴穿越到这里，并培育出一堆奇葩宠兽后，所有御兽师的三观都破碎了……\r\n　　关键词：御兽、宠兽、宠物、召唤。","CName":"玄幻奇幻","Score":9.0},{"Id":627854,"Name":"大秦：不装了，你爹我是秦始皇","Author":"头顶一只喵喵","Img":"daqin_buzhuangle_nidiewoshiqinshihuang.jpg","Desc":"赵浪一觉醒来，发现自己来到了秦朝。\r\n　　好在家境还算富裕。\r\n　　只是算了算时间，大秦只有三年的寿命，赵浪便鼓起勇气，和自己那几个月才回来一次的便宜老爹说道，\r\n　　“爹，始皇帝三年之后必死，大秦将亡，到时候天下大乱，我们早做准备造反吧！”\r\n　　便宜老爹先是一愣，随后点头同意。\r\n　　赵浪顿时兴教育，练新军。\r\n　　就当他羽翼丰满，准备天下争雄时。\r\n　　便宜老爹突然来到了他的面前，\r\n　　“","CName":"历史军事","Score":7.3},{"Id":626204,"Name":"夜的命名术","Author":"会说话的肘子","Img":"yedemingmingshu.jpg","Desc":"蓝与紫的霓虹中，浓密的钢铁苍穹下，数据洪流的前端，是科技革命之后的世界，也是现实与虚幻的分界。钢铁与身体，过去与未来。这里，表世界与里世界并存，面前的一切，像是时间之墙近在眼前。黑暗逐渐笼罩。可你要明白啊我的朋友，我们不能用温柔去应对黑暗，要用火。","CName":"玄幻奇幻","Score":8.7},{"Id":630009,"Name":"星门","Author":"老鹰吃小鸡","Img":"xingmen.jpg","Desc":"传说，在那古老的星空深处，伫立着一道血与火侵染的红色之门。\r\n　　传奇与神话，黑暗与光明，无尽传说皆在这古老的门户中流淌。\r\n　　俯瞰星门，热血照耀天地，黑暗终将离去！","CName":"玄幻奇幻","Score":8.8},{"Id":627885,"Name":"迎娶女帝之后","Author":"老狗","Img":"yingqunvdizhihou.jpg","Desc":"李云没有想到，穿越到这个世界后的第一件事，就是被迫卷入造反的大军。大乾九百七十六年，居于大陆之央的大乾终于镇压了这场大陆千年来规模最大，影响力最深的叛乱，平四方，镇气运。同年，大乾老皇帝驾崩，新帝登基，整个世界的命运都被掌握在这位新的至高权力者手上，无人能够逃过。","CName":"玄幻奇幻","Score":8.0},{"Id":630133,"Name":"机械炼金术士","Author":"盲候","Img":"jixielianjinshushi.jpg","Desc":"幽暗的地下城，这里埋藏了数之不尽的古代遗迹和宝藏。\r\n　　诡异，畸变，诅咒物...\r\n　　深渊，地窟，古神，神话种族...\r\n　　机械师，咒印植装，巨城黑塔...\r\n　　千奇百怪炼金术，添一勺蒸汽朋克，两勺诡秘超凡，杂糅出了一个缤纷多彩的奇幻世界。\r\n　　我，傀儡炼金术士。\r\n　　一人，便是军团！","CName":"网游竞技","Score":9.6},{"Id":147613,"Name":"轮回乐园","Author":"那一只蚊子","Img":"lunhuileyuan.jpg","Desc":"机遇与危险共存，只要豁出性命，在轮回乐园中就能得到一切。\r\n　　被轮回乐园选中成为猎杀者的那一刻，苏晓就明白，他将与所有人为敌。\r\n　　乐园虽然残酷，但无所不能……。","CName":"玄幻奇幻","Score":6.3},{"Id":3051,"Name":"遮天","Author":"辰东","Img":"zhetian.jpg","Desc":"冰冷与黑暗并存的宇宙深处，九具庞大的龙尸拉着一口青铜古棺，亘古长存。这是太空探测器在枯寂的宇宙中捕捉到的一幅极其震撼的画面。九龙拉棺，究竟是回到了上古，还是来到了星空的彼岸？一个浩大的仙侠世界，光怪陆离，神秘无尽。热血似火山沸腾，激情若瀚海汹涌，欲望如深渊无止境……登天路，踏歌行，弹指遮天。","CName":"武侠仙侠","Score":8.6}],"Page":1,"HasNext":true}}

### 小说高分神作 更多
GET https://scxs.pysmei.com/top/man/top/vote/week/1.html HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
Content-Type: application/x-www-form-urlencoded
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Host: scxs.pysmei.com
Connection: Keep-Alive
Accept-Encoding: gzip

{"status":1,"info":"success","data":{"BookList":[{"Id":521014,"Name":"大奉打更人","Author":"卖报小郎君","Img":"dafengdagengren.jpg","Desc":"这个世界，有儒；有道；有佛；有妖；有术士。\r\n　　警校毕业的许七安幽幽醒来，发现自己身处牢狱之中，三日后流放边陲.....\r\n　　他起初的目的只是自保，顺便在这个没有人权的社会里当个富家翁悠闲度日。\r\n　　......\r\n　　多年后，许七安回首前尘，身后是早已逝去的敌人和朋友，以及累累白骨。\r\n　　滚滚长江东逝水，浪花淘尽英雄，是非成败转头空。\r\n　　青山依旧在，几度夕阳红。\r\n　　PS：本书不悲","CName":"武侠仙侠","Score":9.4},{"Id":570433,"Name":"我真没想当训练家啊","Author":"北川南海","Img":"wozhenmeixiangdangxunlianjiaa.jpg","Desc":"现在站在你面前的是——\r\n　　得文公司董事会、彩虹火箭队缔造者、逆属性大师、世界锦标赛冠军……\r\n　　传奇训练家陆野，回忆起首次直播时的场景，喟然长叹。\r\n　　“说起来你们可能不信，我最初的愿望只是破十万订阅露个脸而已。”\r\n　　“我只想恰点钱，从一名游戏区UP主做起。”\r\n　　“我真没想当训练家啊！”\r\n　　本书又名：《五等分的陆野》、《青春期训练家不会梦见神奥冠军》、《竹兰大小姐想让我告白》、","CName":"玄幻奇幻","Score":9.3},{"Id":600715,"Name":"我家老婆来自一千年前","Author":"花还没开","Img":"wojialaopolaiziyiqiannianqian.jpg","Desc":"“我想回家。”\r\n　　“你可能回不去了。”\r\n　　“为什么？”\r\n　　“因为这里离你家很远。”\r\n　　“有多远？”\r\n　　“一千二百多年那么远。”\r\n　　许青看着眼前来自唐朝的少女，脸上带有一丝同情：“你所熟悉的一切，都已经变成历史。”\r\n　　亲朋，好友，敌人，全部沉寂在一千二百年前。\r\n　　———\r\n　　日常文，单女主\r\n　　（已有完本精品，质量保证。）","CName":"都市言情","Score":9.3},{"Id":24328,"Name":"非正常人类异闻录","Author":"精分三代","Img":"feizhengchangrenleiyiwenlu.jpg","Desc":"我叫张大道，道号张全道。在第七人民医院被人研究！\r\n　　\r\n　　    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\r\n　　\r\n　　    贫道张全道，专业摸骨批命，棺材翻新,抛光,打蜡。回收二手僵尸,寻龙点穴、批发黑驴蹄、黑狗血。代写1~3年级小学作业，寻找走失猫狗，抓小三。\r\n　　\r\n　　    专业报仇打小人、改风水、妨祖坟！量大从优！有发票！\r\n　　\r\n　　    ~~~~~","CName":"都市言情","Score":9.3},{"Id":488380,"Name":"万界圆梦师","Author":"棉衣卫","Img":"wanjieyuanmengshi.jpg","Desc":"自爆、增发术、断肢求生、被读心术、百分百被空手接白刃……是我的金手指！\r\n　　帮助拆迁女怀上李寻欢的孩子；带十岁小女孩打穿海扁王的世界；协助客户获得步惊云的麒麟臂……是我的日常工作。\r\n　　崩剧情，杀主角，毁灭世界规则……不惜一切代价，即便你自己放弃了梦想，我都不会放弃，是我的职业素养。\r\n　　我是李沐，用着最废物的技能，干着最艰难的工作！\r\n　　我是最强大（邪恶）的圆梦师，擅长帮你实现梦想（更擅","CName":"科幻灵异","Score":9.2},{"Id":618211,"Name":"我的治愈系游戏","Author":"我会修空调","Img":"wodezhiyuxiyouxi.jpg","Desc":"警察同志，如果我说这是一款休闲治愈系游戏，你们信吗？","CName":"玄幻奇幻","Score":9.0},{"Id":630009,"Name":"星门","Author":"老鹰吃小鸡","Img":"xingmen.jpg","Desc":"传说，在那古老的星空深处，伫立着一道血与火侵染的红色之门。\r\n　　传奇与神话，黑暗与光明，无尽传说皆在这古老的门户中流淌。\r\n　　俯瞰星门，热血照耀天地，黑暗终将离去！","CName":"玄幻奇幻","Score":9.0},{"Id":17779,"Name":"万古神帝","Author":"飞天鱼","Img":"wangushendi.jpg","Desc":"【NEXTIDEA暨2015星创奖征文大赏（玄幻）】\r\n　　\r\n　　    八百年前，明帝之子张若尘，被他的未婚妻池瑶公主杀死，一代无上天骄，就此陨落。\r\n　　\r\n　　    八百年后，张若尘重新活了过来，却发现曾经杀死他的未婚妻，已经统一昆仑界，开辟出第一中央帝国，号称“池瑶女皇”。\r\n　　\r\n　　    池瑶女皇——统御天下，威临八方；青春永驻，不死不灭。\r\n　　\r\n　　    张若尘站在诸皇祠堂外，望着池瑶女皇的神像，心中","CName":"玄幻奇幻","Score":9.0},{"Id":632295,"Name":"奥特赘婿","Author":"鸣愿","Img":"aotezhuixu.jpg","Desc":"战神佐菲为了报恩，隐藏身份入赘方家，一路扮猪吃老虎。\\n只是他总是感觉，自己的这位老婆，有亿点点诡异。\\n主角：佐菲。反派：方长/叶紫\\n（本书又名《正义奥特曼必胜！如果结局不好，说明没到结局》）","CName":"玄幻奇幻","Score":9.0},{"Id":251646,"Name":"大魔王","Author":"轻尘大神","Img":"damowang1.jpg","Desc":"卢高斯帝国的突然不宣而战，对曼德帝国可是一大沉重打击，国王希勒下旨，全国紧急总动员，征召大量青壮，组建军队，又从东部战场抽调几个精锐师，以抵御卢高斯帝国的入侵。","CName":"玄幻奇幻","Score":9.0},{"Id":519568,"Name":"泠风浮仙","Author":"方泠然","Img":"lingfengfuxian.jpg","Desc":"夫列子御风而行,泠然善也。\r\n　　且看这风灵少女，踏上仙途，一路披荆斩棘，只为心中执念。","CName":"玄幻奇幻","Score":9.0},{"Id":363483,"Name":"抗日之全能兵王","Author":"寂寞剑客","Img":"kangrizhiquannengbingwang.jpg","Desc":"钟毅，一位来自北部战区天狼突击队的全能兵王，在朱日和的一次演习中，因为遭到己方远程炮火的误伤，灵魂穿越到1937年的淞沪战场，成为金山卫保安队队长，且看钟毅如何带着他的炮灰团，利用现代的作战理念及特战技巧，杀得小鬼子尸横遍野、血流成河！","CName":"历史军事","Score":9.0},{"Id":248872,"Name":"诡秘之主","Author":"爱潜水的乌贼","Img":"guimizhizhu.jpg","Desc":"蒸汽与机械的浪潮中，谁能触及非凡？历史和黑暗的迷雾里，又是谁在耳语？我从诡秘中醒来，睁眼看见这个世界：枪械，大炮，巨舰，飞空艇，差分机；魔药，占卜，诅咒，倒吊人，封印物……光明依旧照耀，神秘从未远离，这是一段“愚者”的传说。","CName":"玄幻奇幻","Score":9.0},{"Id":148025,"Name":"鬼吹灯","Author":"天下霸唱","Img":"guichuideng.jpg","Desc":"鬼吹灯是一个系列形式的文字冒险故事，以一本家传的秘书残卷为引。小说中作者首创历史上四大盗墓门派——摸金、卸岭、发丘、搬山，其中摸金是技术含量最高，规矩最多的门派。“人点烛，鬼吹灯”是传说中摸金派的不传之秘，意为进入古墓之中先在东南角点燃一支蜡烛才能开棺，如果蜡烛熄灭，须速速退出，不可取一物。相传这是祖师爷所定的一条活人与死人的契约，千年传承，不得破。有谚为证：发丘印，摸金符，搬山卸岭寻龙诀；人点烛","CName":"科幻灵异","Score":9.0},{"Id":61,"Name":"雪中悍刀行","Author":"烽火戏诸侯","Img":"61.jpg","Desc":"雪中悍刀行最新章节列：小说《雪中悍刀行》烽火戏诸侯/著,雪中悍刀行全文阅读这个江湖。有武夫自称天下第二一甲子。有剑仙一剑破甲两千六。有胆小的骑牛道士肩扛两道。但一样是这个江湖，可能是江湖儿郎江湖死，才初......","CName":"玄幻奇幻","Score":8.9},{"Id":560093,"Name":"白骨大圣","Author":"咬火","Img":"baigudasheng.jpg","Desc":"死人沾地，活人娶尸，老狗刨坟，吃活人饭，阴人问路，知道碰上其中一个意味着什么吗？\r\n　　「已有2万均订作品《这里有妖气》」\r\n　　「《这里有妖气》漫画改编版权已卖出」\r\n　　「《这里有妖气》漫画已上线，可在腾讯动漫、起点漫画、B站漫画阅读」\r\n　　书友①群：608548874；\r\n　　书友②群：760859432。","CName":"玄幻奇幻","Score":8.7},{"Id":573941,"Name":"没钱上大学的我只能去屠龙了","Author":"宇宙无敌水哥","Img":"meiqianshangdaxuedewozhinengqutulongle.jpg","Desc":"总之岁月漫长，然而值得等待。\r\n　　林年等了十六年，等到了卡塞尔之门的召唤，等来荒诞无稽、热血放纵的青春。","CName":"玄幻奇幻","Score":8.7},{"Id":626204,"Name":"夜的命名术","Author":"会说话的肘子","Img":"yedemingmingshu.jpg","Desc":"蓝与紫的霓虹中，浓密的钢铁苍穹下，数据洪流的前端，是科技革命之后的世界，也是现实与虚幻的分界。钢铁与身体，过去与未来。这里，表世界与里世界并存，面前的一切，像是时间之墙近在眼前。黑暗逐渐笼罩。可你要明白啊我的朋友，我们不能用温柔去应对黑暗，要用火。","CName":"玄幻奇幻","Score":8.7},{"Id":630600,"Name":"黎明之劫","Author":"花还没开","Img":"limingzhijie.jpg","Desc":"在做了很久奇怪的梦之后，陆安以为自己病了。\r\n　　……直到这天，有一个莫名其妙的少女出现在他家中，到处嫌弃了一番“古代”生活，她说自己来自未来。\r\n　　然后陆安报警把她抓了。","CName":"科幻灵异","Score":8.7},{"Id":601830,"Name":"十方武圣","Author":"滚开","Img":"shifangwusheng.jpg","Desc":"末日荒土，世宗三年，天下大乱，民不聊生。\r\n　　中央皇朝崩坏，各地群雄割据，门派独立。魔门妖党隐于暗处作乱，帮派相互征伐，混乱不堪。\r\n　　天灾连连，大旱，酷寒，暴雨，虫灾，人民苦苦挣扎，渴求希望与救赎。\r\n　　大乱之中，各门各派纷纷出世，争夺资源地盘，建立独属于自己的统治。\r\n　　有野心者试图席卷天下，建立王朝，也有大义者，意图挽救苍生，重建家园。\r\n　　肌肉，武道，仙法，一位位武道极限强者，在","CName":"玄幻奇幻","Score":8.7},{"Id":624733,"Name":"道友，买把加特林吗？","Author":"驿路羁旅","Img":"daoyou，maibajiatelinma？.jpg","Desc":"“墨家机关术很好很棒，但可惜它已经跟不上这个时代的变化了。”\r\n　　差点重生失败，又经历了神奇故事的前军火商，现墨家制器师江夏，提着自己手制废土版魔改猎巫重机枪，对自己的师兄师姐们说：\r\n　　“这小可爱，才象征着未来！”\r\n　　“道友，来把加特林不？”","CName":"网游竞技","Score":8.7}],"Page":1,"HasNext":true}}

### 小说微信热书 更多
GET https://scxs.pysmei.com/top/man/top/commend/week/1.html HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
Content-Type: application/x-www-form-urlencoded
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Host: scxs.pysmei.com
Connection: Keep-Alive
Accept-Encoding: gzip

{"status":1,"info":"success","data":{"BookList":[{"Id":147613,"Name":"轮回乐园","Author":"那一只蚊子","Img":"lunhuileyuan.jpg","Desc":"机遇与危险共存，只要豁出性命，在轮回乐园中就能得到一切。\r\n　　被轮回乐园选中成为猎杀者的那一刻，苏晓就明白，他将与所有人为敌。\r\n　　乐园虽然残酷，但无所不能……。","CName":"玄幻奇幻","Score":6.3},{"Id":626204,"Name":"夜的命名术","Author":"会说话的肘子","Img":"yedemingmingshu.jpg","Desc":"蓝与紫的霓虹中，浓密的钢铁苍穹下，数据洪流的前端，是科技革命之后的世界，也是现实与虚幻的分界。钢铁与身体，过去与未来。这里，表世界与里世界并存，面前的一切，像是时间之墙近在眼前。黑暗逐渐笼罩。可你要明白啊我的朋友，我们不能用温柔去应对黑暗，要用火。","CName":"玄幻奇幻","Score":8.7},{"Id":632295,"Name":"奥特赘婿","Author":"鸣愿","Img":"aotezhuixu.jpg","Desc":"战神佐菲为了报恩，隐藏身份入赘方家，一路扮猪吃老虎。\\n只是他总是感觉，自己的这位老婆，有亿点点诡异。\\n主角：佐菲。反派：方长/叶紫\\n（本书又名《正义奥特曼必胜！如果结局不好，说明没到结局》）","CName":"玄幻奇幻","Score":8.3},{"Id":631387,"Name":"开局：一个民国位面","Author":"龙升云霄","Img":"kaijuyigeminguoweimian.jpg","Desc":"如果你能往返一个‘特殊’的民国世界，你会做什么？\r\n　　富甲天下，妻妾成群？\r\n　　提笔报国，文压天下？\r\n　　秣马厉兵，封王拜将？\r\n　　还是...\r\n　　练得身形似鹤形，千株松下两函经。\r\n　　我来问道无余说，云在青天水在瓶。\r\n　　ps：本书又名《诸天：从民国开始》。","CName":"科幻灵异","Score":8.8},{"Id":623334,"Name":"斗罗大陆5重生唐三","Author":"唐家三少","Img":"douluodalu5zhongshengtangsan.jpg","Desc":"一代神王唐三，因为妻子的死而选择了殉情，带着一点神识在宇宙中遨游，寻找妻子转世重生的世界。在神识的牵引下，他来到了一个叫作妖精大陆的地方，寻找他的妻子小舞。而他却发现，这是一个人类为刍狗的世界······","CName":"玄幻奇幻","Score":1.4},{"Id":480889,"Name":"世界树的游戏","Author":"咯嘣","Img":"shijieshudeyouxi.jpg","Desc":"“虚拟现实游戏”《精灵国度》中人气最高的NPC，世界树的化身，自然之母，生命女神，精灵主宰——\r\n　　伊芙·尤克特拉希尔高坐在自己的神座上，微笑地看着台下的玩家们：\r\n　　“欢迎来到剑与魔法的世界。”\r\n　　穿越是个技术活。\r\n　　如果不是两界通道和人类玩家，这将是个正经的龙傲娇奇幻故事。","CName":"玄幻奇幻","Score":8.6},{"Id":521014,"Name":"大奉打更人","Author":"卖报小郎君","Img":"dafengdagengren.jpg","Desc":"这个世界，有儒；有道；有佛；有妖；有术士。\r\n　　警校毕业的许七安幽幽醒来，发现自己身处牢狱之中，三日后流放边陲.....\r\n　　他起初的目的只是自保，顺便在这个没有人权的社会里当个富家翁悠闲度日。\r\n　　......\r\n　　多年后，许七安回首前尘，身后是早已逝去的敌人和朋友，以及累累白骨。\r\n　　滚滚长江东逝水，浪花淘尽英雄，是非成败转头空。\r\n　　青山依旧在，几度夕阳红。\r\n　　PS：本书不悲","CName":"武侠仙侠","Score":9.0},{"Id":478397,"Name":"大唐补习班","Author":"危险的世界","Img":"datangbuxiban.jpg","Desc":"柴米油盐酱醋茶，当年样样不离它。如今七事以改变，琴棋书画诗酒花。\r\n　　李昊穿越了，在古代的大唐。\r\n　　文人之中我武力值最高；武将里面我最有文化。\r\n　　大唐将因我而改变……。\r\n　　因为……我们不一样！","CName":"历史军事","Score":6.0},{"Id":630009,"Name":"星门","Author":"老鹰吃小鸡","Img":"xingmen.jpg","Desc":"传说，在那古老的星空深处，伫立着一道血与火侵染的红色之门。\r\n　　传奇与神话，黑暗与光明，无尽传说皆在这古老的门户中流淌。\r\n　　俯瞰星门，热血照耀天地，黑暗终将离去！","CName":"玄幻奇幻","Score":8.8},{"Id":633495,"Name":"我绑架了时间线","Author":"一刀斩斩斩","Img":"wobangjialeshijianxian.jpg","Desc":"一觉醒来，封棋发现世界已经发生了翻天覆地的变化。\r\n　　目之所及满地枯骨，生命凋零。\r\n　　在脑海中声音的指引下，他开始穿梭于现实与未来，逐渐了解了世界的真相，也开始探寻改变世界的方法。\r\n　　正因为见过了黑暗，所以无限向往光明。","CName":"科幻灵异","Score":6.0},{"Id":626648,"Name":"全职之职业欧皇","Author":"闪光哈士奇","Img":"quanzhizhizhiyeouhuang.jpg","Desc":"记者：请问你们兴欣战队的成员对你们的副队长唐银的看法是怎么样的？\r\n　　叶修：他用事实告诉我们，不玩战术的心也脏。以及让人绝望的运气.....\r\n　　苏沐橙：最佳队友，僚机中的战斗机，以及让人羡慕的运气。\r\n　　魏琛：论没下线，我愿称他为最强。还有他绝对和幸运女神有一腿！\r\n　　........\r\n　　唐银：我只不过是运气使然的职业选手。\r\n　　二哈新作：全职高手同人\r\n　　二哈书友群：10467","CName":"玄幻奇幻","Score":8.0},{"Id":31439,"Name":"我当阴阳先生的那几年","Author":"崔走召","Img":"wodangyinyangxianshengdeneijinian.jpg","Desc":"我们的故事是从一个死亡后进入阴间的少年身上开始的。你是否听说过很多民间流传的离奇故事？是否对故事里的那些身怀异术的能人心生过仰慕和向往？本书所讲的就是那些散落在民间的身怀异术之人的故事。他们精通卜卦方术，知晓驱鬼画符，身怀奇门遁甲。当他们的本领已经不被这个时代所承认的时候，他们又该怎么去抉择？\r\n　　\r\n　　    －－－－－－－－－－－－－－－－－－－－－－－－－－－－－－－－－－－－－－－－－－－－－","CName":"科幻灵异","Score":8.9},{"Id":526486,"Name":"剑道第一仙","Author":"萧瑾瑜","Img":"jiandaodiyixian.jpg","Desc":"我是万古人间一剑修，诸天之上第一仙。已有完本作品《符皇》《天骄战纪》公众号：xiaojinyu233","CName":"玄幻奇幻","Score":6.9},{"Id":59334,"Name":"极度尸寒","Author":"全雨","Img":"jidushihan.jpg","Desc":"一个人总能见到鬼，你猜他活的开心吗？\r\n　　\r\n　　    嗯，来点善意的提醒吧。这本书充斥着暴戾、黑暗、血腥、变态，没有一点正能量，压抑的感觉贯穿全书。这本书不适合普通人看，不适合正常人看，更不适合卫道士和正人君子看。当然，得看到后面才能发现这些问题，只看前面的章节是体会不到的。\r\n　　\r\n　　    鄙人最喜欢做的事就是挖坑，而且只管挖不管埋。这本书里的大坑套小坑，一脚陷进去就不好拔出来，大家一定要慎入。","CName":"科幻灵异","Score":7.5},{"Id":627409,"Name":"云边有个小卖部","Author":"张嘉佳","Img":"yunbianyougexiaomaibu.jpg","Desc":"张嘉佳全新作品。畅销千万现象级作品《从你的全世界路过》后，暌违五年，写给离开我们的人，写给陪伴我们的人，写给每个人心中的山和海。\\n希望和悲伤，都是一缕光。总有一天，我们会再相遇。\\n让刘十三陪着你，走进云边镇的春夏秋冬，见证每一场相遇与离别。“有些人刻骨铭心，没几年会遗忘。有些人不论生死，都陪在身旁。”\\n满镇开着桔梗，蒲公英飞得比石榴树还高，一直飘进山","CName":"都市言情","Score":9.5},{"Id":377500,"Name":"斗罗大陆IV终极斗罗","Author":"唐家三少","Img":"douluodaluIVzhongjidouluo.jpg","Desc":"一万年后，冰化了。\r\n　　斗罗联邦科考队在极北之地科考时发现了一个有着金银双色花纹的蛋，用仪器探察之后，发现里面居然有生命体征，赶忙将其带回研究所进行孵化。蛋孵化出来了，可孵出来的却是一个婴儿，和人类一模一样的婴儿，一个蛋生的孩子。","CName":"玄幻奇幻","Score":2.8},{"Id":384854,"Name":"死在火星上","Author":"天瑞说符","Img":"sizaihuoxingshang.jpg","Desc":"我叫唐跃，我在火星上。\r\n　　我刚刚看到地球炸了。","CName":"科幻灵异","Score":8.9},{"Id":607413,"Name":"全球高武之我的系统送错了","Author":"英俊追梦人","Img":"quanqiugaowuzhiwodexitongsongcuole.jpg","Desc":"穿越的那一刻，苏北觉得自己是最幸运的人，尤其是自己穿越的地方叫地球，有个系统叫穿越武侠系统，这是要逆袭的节奏啊。\r\n　　可是整理下记忆，为什么有个职业叫武者，有个爷爷叫苏展，有个学校叫京武？\r\n　　全球高武的世界，小李飞刀，能否一刀戳破源地？降龙十八掌，是否真的能降伏龙皇？我就是把武功练到极致、练到破碎虚空的境界，有用么？","CName":"玄幻奇幻","Score":6.0},{"Id":628100,"Name":"当青春幻想具现后","Author":"转角吻猪","Img":"dangqingchunhuanxiangjuxianhou.jpg","Desc":"当时间停止一小时，只有你可以自由移动时，你会做什么？\r\n　　谢邀，这问题别问我啊！你问她——\r\n　　对！就是这个趁着时间停止来到我身边，朝我伸出手的女孩！\r\n　　------\r\n　　时间停止、返老还童、时空电话、猫的报恩……当青春里出现一件又一件荒唐而又神奇的事件时，我们的故事开始了。\r\n　　（关键词：幻想具现、日常、恋爱）","CName":"都市言情","Score":9.2},{"Id":625913,"Name":"万相之王","Author":"天蚕土豆","Img":"wanxiangzhiwang.jpg","Desc":"天地间，有万相。而我李洛，终将成为这万相之王。","CName":"玄幻奇幻","Score":4.7},{"Id":146769,"Name":"剑来","Author":"烽火戏诸侯","Img":"jianlai.jpg","Desc":"大千世界，无奇不有。我陈平安，唯有一剑，可搬山，倒海，降妖，镇魔，敕神，摘星，断江，摧城，开天！","CName":"玄幻奇幻","Score":8.2}],"Page":1,"HasNext":true}}

### 小说 豆瓣高分 更多
GET https://scxs.pysmei.com/top/man/top/new/week/1.html HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
Content-Type: application/x-www-form-urlencoded
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Host: scxs.pysmei.com
Connection: Keep-Alive
Accept-Encoding: gzip

{"status":1,"info":"success","data":{"BookList":[{"Id":628547,"Name":"不科学御兽","Author":"轻泉流响","Img":"bukexueyushou.jpg","Desc":"这是一个以御兽为主流的异世界。\r\n　　当时宇携带技能图鉴穿越到这里，并培育出一堆奇葩宠兽后，所有御兽师的三观都破碎了……\r\n　　关键词：御兽、宠兽、宠物、召唤。","CName":"玄幻奇幻","Score":9.0},{"Id":630046,"Name":"我就是神！","Author":"历史里吹吹风","Img":"wojiushishen_.jpg","Desc":"尹神的名字叫神。\r\n　　他从来没有想过，有一天自己会真的成为神。","CName":"玄幻奇幻","Score":8.3},{"Id":630009,"Name":"星门","Author":"老鹰吃小鸡","Img":"xingmen.jpg","Desc":"传说，在那古老的星空深处，伫立着一道血与火侵染的红色之门。\r\n　　传奇与神话，黑暗与光明，无尽传说皆在这古老的门户中流淌。\r\n　　俯瞰星门，热血照耀天地，黑暗终将离去！","CName":"玄幻奇幻","Score":8.8},{"Id":628100,"Name":"当青春幻想具现后","Author":"转角吻猪","Img":"dangqingchunhuanxiangjuxianhou.jpg","Desc":"当时间停止一小时，只有你可以自由移动时，你会做什么？\r\n　　谢邀，这问题别问我啊！你问她——\r\n　　对！就是这个趁着时间停止来到我身边，朝我伸出手的女孩！\r\n　　------\r\n　　时间停止、返老还童、时空电话、猫的报恩……当青春里出现一件又一件荒唐而又神奇的事件时，我们的故事开始了。\r\n　　（关键词：幻想具现、日常、恋爱）","CName":"都市言情","Score":9.2},{"Id":631387,"Name":"开局：一个民国位面","Author":"龙升云霄","Img":"kaijuyigeminguoweimian.jpg","Desc":"如果你能往返一个‘特殊’的民国世界，你会做什么？\r\n　　富甲天下，妻妾成群？\r\n　　提笔报国，文压天下？\r\n　　秣马厉兵，封王拜将？\r\n　　还是...\r\n　　练得身形似鹤形，千株松下两函经。\r\n　　我来问道无余说，云在青天水在瓶。\r\n　　ps：本书又名《诸天：从民国开始》。","CName":"科幻灵异","Score":8.8},{"Id":630133,"Name":"机械炼金术士","Author":"盲候","Img":"jixielianjinshushi.jpg","Desc":"幽暗的地下城，这里埋藏了数之不尽的古代遗迹和宝藏。\r\n　　诡异，畸变，诅咒物...\r\n　　深渊，地窟，古神，神话种族...\r\n　　机械师，咒印植装，巨城黑塔...\r\n　　千奇百怪炼金术，添一勺蒸汽朋克，两勺诡秘超凡，杂糅出了一个缤纷多彩的奇幻世界。\r\n　　我，傀儡炼金术士。\r\n　　一人，便是军团！","CName":"网游竞技","Score":9.6},{"Id":632295,"Name":"奥特赘婿","Author":"鸣愿","Img":"aotezhuixu.jpg","Desc":"战神佐菲为了报恩，隐藏身份入赘方家，一路扮猪吃老虎。\\n只是他总是感觉，自己的这位老婆，有亿点点诡异。\\n主角：佐菲。反派：方长/叶紫\\n（本书又名《正义奥特曼必胜！如果结局不好，说明没到结局》）","CName":"玄幻奇幻","Score":8.3},{"Id":630771,"Name":"不能修仙的我只有去培育魂宠了","Author":"夏竖琴","Img":"bunengxiuxiandewozhiyouqupeiyuhunchongle.jpg","Desc":"前登仙境大修士王澈因渡劫失败，灵魂穿梭到了一个魂兽和人类和平相处的武魂世界。\r\n　　在确定这个世界无法修仙后，生无可恋的他，无奈之下只能适应这个世界。\r\n　　于是…\r\n　　“绿毛虫，百万年进化！”\r\n　　“出来吧！裂空座…哦不，天空龙！”","CName":"玄幻奇幻","Score":9.0},{"Id":630600,"Name":"黎明之劫","Author":"花还没开","Img":"limingzhijie.jpg","Desc":"在做了很久奇怪的梦之后，陆安以为自己病了。\r\n　　……直到这天，有一个莫名其妙的少女出现在他家中，到处嫌弃了一番“古代”生活，她说自己来自未来。\r\n　　然后陆安报警把她抓了。","CName":"科幻灵异","Score":9.5},{"Id":630195,"Name":"我于世间全无敌","Author":"陆鹏","Img":"woyushijianquanwudi.jpg","Desc":"路一平是个上古修士，亲眼见证了诸神大战中，无数强大的神灵殒落的情景。自此之后，他便躲在深山老林，日夜修炼，发誓没有强大到对抗天地大劫的实力时，便不出来。一个时代又一个时代过去了。他身边的一头小蛇，成为了龙族之祖。他收养过的一个小女孩，成了无敌女帝。他指点过的一个剑客，成了名响万古的剑神。他随意种下的一棵老树，成了史上最强神国的守护之神。沧海桑","CName":"玄幻奇幻","Score":3.7},{"Id":629127,"Name":"斗罗之双枪绝世","Author":"禄禄吖","Img":"douluozhishuangqiangjueshi.jpg","Desc":"书友群：901187850\r\n　　【黑化流】【圣母勿入】【高智商】\r\n　　【最好看的斗罗同人，没有之一】\r\n　　自从被那个女人捡到以后，他的一生，都为止改变。\r\n　　武魂觉醒，先天满魂力，双生武魂。\r\n　　从这一刻起，杀神觉醒了。\r\n　　苏逸：比比东，由我来守护。\r\n　　她想要这天下，我就给她这天下。\r\n　　神挡杀神，魔挡屠魔！\r\n　　吾有一枪，混沌至尊枪，披荆斩棘，所向披靡。\r\n　　吾有一枪，天","CName":"玄幻奇幻","Score":6.0},{"Id":630039,"Name":"这游戏也太真实了","Author":"晨星LL","Img":"zheiyouxiyetaizhenshile.jpg","Desc":"不正经的简介：\r\n　　这游戏也太真实了叭！\r\n　　怎么打着打着队友的衣服就没了？\r\n　　什么？你问我这游戏正经不？\r\n　　当然正经了！\r\n　　搬砖、跑腿、捡垃圾、送快递……公司最多能让你体会到996的艰辛，在这里你能体会到超级加倍的007。\r\n　　还有比这更真实的游戏？\r\n　　好了，不废话了，伟大的管理者大人喊我去搬砖了。\r\n　　那位大人说了，只要我们献上自己的肝，下个月他又能换一套全新的动力甲，","CName":"玄幻奇幻","Score":8.7},{"Id":630394,"Name":"我用闲书成圣人","Author":"出走八万里","Img":"woyongxianshuchengshengren.jpg","Desc":"开局一口棺材。\r\n　　陈洛的穿越从灵堂开始。\r\n　　这是一个读书就能获得超凡威力的世界。\r\n　　读儒门经典，可养浩然正气；\r\n　　读道门典藏，可生先天源炁；\r\n　　读佛门经文，可悟轮回真意；\r\n　　偏偏陈洛的金手指却是一堆天道都不允许在这个世界出现的闲书！\r\n　　……\r\n　　什么？《聊斋》被妖国当做天书？\r\n　　什么？《天龙八部》打开了武学天地？\r\n　　什么？《金瓶梅》……\r\n　　别慌别慌，都是小","CName":"武侠仙侠","Score":8.5},{"Id":633556,"Name":"典藏华夏：我打造节目，对话古今","Author":"大肉大鱼","Img":"dianzanghuaxiawodazaojiemuduihuagujin.jpg","Desc":"【飞卢小说网独家签约小说：典藏华夏：我打造节目，对话古今】\r\n　　苏晨穿越之后，发现自己居然成了国家队最年轻的主持人。\r\n　　同时，上级决定让他打造一个对话古今的节目！\r\n　　原本是要请演员来扮演古人，可是这个时候，系统激活！苏晨震惊的发现，原来他居然可以直接到场，并且采访到历朝历代所有真实的人物。\r\n　　面对秦始皇，苏晨：“晚辈拜见，后世文同书，车同轨，万世昌盛！”\r\n　　始皇震撼：“华","CName":"都市言情","Score":6.8},{"Id":628310,"Name":"重生在全是病娇的异世界我想活命","Author":"湳楠喃","Img":"zhongshengzaiquanshibingjiaodeyishijiewoxianghuoming.jpg","Desc":"病娇控狂喜!吧？有一点偏黑暗，但是放心，有刀会给你预告的，做好心理准备就没事了，嗯嗯。。1主角很强的，不会被NTR的，纯爱哦2可能有一些刺激的情节，嗯，不知道让不让我过审，放心没有大尺度3本作品的风格偏向于轻小说，有多人视角的描写，可能和大部分作品风格不一样，主要的是感情描写以及主角升级装逼4如果不喜欢病娇的话，本作品会比较不对口味，对病娇控应该是狂喜，嗯就这样","CName":"小说同人","Score":8.7},{"Id":630129,"Name":"这个明星很想退休","Author":"幼儿园一把手","Img":"zheigemingxinghenxiangtuixiu.jpg","Desc":"众人：“不！你不想！”\r\n　　.........","CName":"都市言情","Score":8.3},{"Id":631543,"Name":"龙王传说：我为原神","Author":"似梦化星辰","Img":"longwangchuanshuowoweiyuanshen.jpg","Desc":"标签：【斗罗大陆】【原神】【巴巴托斯】【钟离】【斗三】【无敌流爽文】\r\n　　简介：穿越来的毫无缘由，只是眼睛一闭一睁……\r\n　　当风离睁开眼睛后，感受着自己的身体，眼睛中闪过一丝错愕。身为风精灵化形的自己，武魂竟然是一枚国际象棋的棋子。\r\n　　那是……神之心？高级魔力外置器官？这玩意在斗罗大陆有个卵子用？\r\n　　什么，神之心被斗罗大陆规则同化，拥有创造神位的能力？\r\n　　嗯，真香！","CName":"玄幻奇幻","Score":6.3},{"Id":628919,"Name":"道长，时代变了","Author":"全金属弹壳","Img":"daozhangshidaibianle.jpg","Desc":"一枚得宝银钱将云松带到了一个风起云涌的大时代。\r\n　　在这里，有洋人坚船利炮、军阀派系四起，朱门纸醉金迷、百姓流离失所。\r\n　　在这里，也有怪、邪，蟒仙、蛟尸，活人坟、死人玉，纸人偷命、石佛买运，老猫夜拜月、野狐盗群棺，古镇阴差日行、旧都阴兵借道，大江断流现老村、十里洋场遍凶宅，万人坑中藏白骨庙、无名城频现千年妖。\r\n　　在这里，得宝银钱有两面，银钱人用、阴钱鬼用。云松亦有两面，是穿道袍的道长，是","CName":"武侠仙侠","Score":7.4},{"Id":631128,"Name":"重生我真没想当暖男","Author":"李远哲","Img":"zhongshengwozhenmeixiangdangnuannan.jpg","Desc":"尝遍了人情冷暖的李哲，一觉醒来回到了2007年的9月1号。\r\n　　这时他刚考上大学，坐在去洪城师范学院报到的火车上。\r\n　　重生的李哲能有什么坏心思呢，他只想多谈几次恋爱罢了！\r\n　　只是后来李哲发现他竟然成了暖男！\r\n　　暖男者，中央空调也。","CName":"都市言情","Score":8.7},{"Id":629134,"Name":"徒弟太勤奋显得师父有点懒","Author":"天狗吃月亮了","Img":"tuditaiqinfenxiandeshifuyoudianlan.jpg","Desc":"李虚收了个女徒弟，饿了徒弟会喂饭，累了徒弟能捏肩，睡觉徒弟帮宽衣。\r\n　　真不是他懒，是徒弟太勤奋显得他有点懒。\r\n　　【轻松，玩梗日常玄幻；普群：192271096】","CName":"玄幻奇幻","Score":8.0},{"Id":633721,"Name":"我家娘子竟然是女帝","Author":"老狗","Img":"wojianiangzijingranshinvdi.jpg","Desc":"我家老婆貌美如花，哪怕是新登基的女帝都比不上！我家老婆厨艺高超，哪怕是女帝的御膳房都比不上！我家老婆很爱我，很关心我，就算是给个女帝我都不换！什么？我家老婆竟然就是女帝！？","CName":"玄幻奇幻","Score":6.0}],"Page":1,"HasNext":true}}

### 小说 完本精选
GET https://scxs.pysmei.com/top/man/top/over/week/1.html HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
Content-Type: application/x-www-form-urlencoded
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Host: scxs.pysmei.com
Connection: Keep-Alive
Accept-Encoding: gzip

{"status":1,"info":"success","data":{"BookList":[{"Id":521014,"Name":"大奉打更人","Author":"卖报小郎君","Img":"dafengdagengren.jpg","Desc":"这个世界，有儒；有道；有佛；有妖；有术士。\r\n　　警校毕业的许七安幽幽醒来，发现自己身处牢狱之中，三日后流放边陲.....\r\n　　他起初的目的只是自保，顺便在这个没有人权的社会里当个富家翁悠闲度日。\r\n　　......\r\n　　多年后，许七安回首前尘，身后是早已逝去的敌人和朋友，以及累累白骨。\r\n　　滚滚长江东逝水，浪花淘尽英雄，是非成败转头空。\r\n　　青山依旧在，几度夕阳红。\r\n　　PS：本书不悲","CName":"武侠仙侠","Score":9.0},{"Id":5,"Name":"完美世界","Author":"辰东","Img":"5.jpg","Desc":"完美世界最新章节列：小说《完美世界》辰东/著,完美世界全文阅读完美世界是辰东写的东方玄幻类小说..........","CName":"玄幻奇幻","Score":9.0},{"Id":627409,"Name":"云边有个小卖部","Author":"张嘉佳","Img":"yunbianyougexiaomaibu.jpg","Desc":"张嘉佳全新作品。畅销千万现象级作品《从你的全世界路过》后，暌违五年，写给离开我们的人，写给陪伴我们的人，写给每个人心中的山和海。\\n希望和悲伤，都是一缕光。总有一天，我们会再相遇。\\n让刘十三陪着你，走进云边镇的春夏秋冬，见证每一场相遇与离别。“有些人刻骨铭心，没几年会遗忘。有些人不论生死，都陪在身旁。”\\n满镇开着桔梗，蒲公英飞得比石榴树还高，一直飘进山","CName":"都市言情","Score":9.5},{"Id":584678,"Name":"全球迈入神话时代","Author":"最终永恒","Img":"quanqiumairushenhuashidai.jpg","Desc":"平静的生活中，陆一鸣突然拥有了超能力，原本以为自己即将迈向人生巅峰，却发现整个世界已经发生了翻天覆地的变化！\r\n　　古老的传说成为现实，神秘的预言被不断验证，武功、魔法、修仙、妖魔、鬼怪等各种超自然现象依次出现在世人面前。\r\n　　旧有的秩序崩塌了，人类即将迎来一个全新的时代……神话时代！","CName":"科幻灵异","Score":7.6},{"Id":8975,"Name":"全职法师","Author":"乱","Img":"quanzhifashi.jpg","Desc":"一觉醒来，世界大变。\r\n　　\r\n　　    熟悉的高中传授的是魔法，告诉大家要成为一名出色的魔法师。\r\n　　\r\n　　    居住的都市之外游荡着袭击人类的魔物妖兽，虎视眈眈。\r\n　　\r\n　　    崇尚科学的世界变成了崇尚魔法，偏偏有着一样以学渣看待自己的老师，一样目光异样的同学，一样社会底层挣扎的爸爸，一样纯美却不能走路的非血缘妹妹……\r\n　　\r\n　　    不过，莫凡发现绝大多数人都只能够主修一系魔法，自己却","CName":"玄幻奇幻","Score":8.6},{"Id":600715,"Name":"我家老婆来自一千年前","Author":"花还没开","Img":"wojialaopolaiziyiqiannianqian.jpg","Desc":"“我想回家。”\r\n　　“你可能回不去了。”\r\n　　“为什么？”\r\n　　“因为这里离你家很远。”\r\n　　“有多远？”\r\n　　“一千二百多年那么远。”\r\n　　许青看着眼前来自唐朝的少女，脸上带有一丝同情：“你所熟悉的一切，都已经变成历史。”\r\n　　亲朋，好友，敌人，全部沉寂在一千二百年前。\r\n　　———\r\n　　日常文，单女主\r\n　　（已有完本精品，质量保证。）","CName":"都市言情","Score":9.7},{"Id":412435,"Name":"第一序列","Author":"会说话的肘子","Img":"diyixulie.jpg","Desc":"这是任小粟大魔王出现了吗？画风都不带变的吗？是新一代话题终结者吗？肘星人准备好了吗？想知道大魔王是如何练成的吗？让我们在2019年4月15日一起迎接新的世界吧，看看肘子如何喷翻全场！！","CName":"玄幻奇幻","Score":8.7},{"Id":3196,"Name":"死人经","Author":"冰临神下","Img":"sirenjing.jpg","Desc":"为不善乎显明之中者，人得而诛之；为不善于幽闭之中者，鬼得而诛之。人鬼不诛，神得而诛之。一本死人经，半部无道书。斩尽千人头，啖吞百身骨。你要么忍受世界的不公，要么成为世界的主宰。他选择成为杀手，和仇人一样的杀手，但是更加冷酷更无情。刀光剑影中，他要寻求真理——杀生者不死，生生者不生。","CName":"武侠仙侠","Score":8.9},{"Id":630195,"Name":"我于世间全无敌","Author":"陆鹏","Img":"woyushijianquanwudi.jpg","Desc":"路一平是个上古修士，亲眼见证了诸神大战中，无数强大的神灵殒落的情景。自此之后，他便躲在深山老林，日夜修炼，发誓没有强大到对抗天地大劫的实力时，便不出来。一个时代又一个时代过去了。他身边的一头小蛇，成为了龙族之祖。他收养过的一个小女孩，成了无敌女帝。他指点过的一个剑客，成了名响万古的剑神。他随意种下的一棵老树，成了史上最强神国的守护之神。沧海桑","CName":"玄幻奇幻","Score":3.7},{"Id":3143,"Name":"斗破苍穹","Author":"天蚕土豆","Img":"doupocangqiong.jpg","Desc":"这里是属于斗气的世界，没有花俏艳丽的魔法，有的，仅仅是繁衍到巅峰的斗气！新书刚开，请各位兄弟多多支持，用推荐票和收藏，砸烂偶吧.^_^新书等级制度：斗者，斗师，大斗师，斗灵，斗王，斗皇，斗宗，斗尊，斗圣，斗帝。","CName":"玄幻奇幻","Score":8.1},{"Id":1559,"Name":"斗罗大陆","Author":"唐家三少","Img":"douluodalu.jpg","Desc":"【小三新书《阴阳冕》已经注册】将会在本周日，斗罗大陆结束的同时开始上传更新，麻烦大家先收藏、推荐一下，谢谢。阴阳冕书号：1436015下面的直通车也可以直接点过去。【小三出品，必属精品，全新设定，酬谢书友】target=&_blank&","CName":"玄幻奇幻","Score":4.6},{"Id":140456,"Name":"超神机械师","Author":"齐佩甲","Img":"chaoshenjixieshi.jpg","Desc":"韩萧，《星海》骨灰级代练，被来自东（zuo）方(zhe)的神秘力量扔进穿越大军，携带玩家面板变成NPC，回到《星海》公测之前，毅然选择难度最高的机械系。\r\n　　战舰列队纵横星海，星辰机甲夭矫如龙，幽能炮毁天灭地，还有无边无际的机械大军，静静待在随身仓库里。\r\n　　一人，即是军团！\r\n　　如果不是玩家出现，本书就是正经严肃的穿越异界题材……\r\n　　作为NPC，正常NPC对玩家功能一应俱全……发布任务","CName":"网游竞技","Score":9.4},{"Id":627885,"Name":"迎娶女帝之后","Author":"老狗","Img":"yingqunvdizhihou.jpg","Desc":"李云没有想到，穿越到这个世界后的第一件事，就是被迫卷入造反的大军。大乾九百七十六年，居于大陆之央的大乾终于镇压了这场大陆千年来规模最大，影响力最深的叛乱，平四方，镇气运。同年，大乾老皇帝驾崩，新帝登基，整个世界的命运都被掌握在这位新的至高权力者手上，无人能够逃过。","CName":"玄幻奇幻","Score":8.0},{"Id":377500,"Name":"斗罗大陆IV终极斗罗","Author":"唐家三少","Img":"douluodaluIVzhongjidouluo.jpg","Desc":"一万年后，冰化了。\r\n　　斗罗联邦科考队在极北之地科考时发现了一个有着金银双色花纹的蛋，用仪器探察之后，发现里面居然有生命体征，赶忙将其带回研究所进行孵化。蛋孵化出来了，可孵出来的却是一个婴儿，和人类一模一样的婴儿，一个蛋生的孩子。","CName":"玄幻奇幻","Score":2.8},{"Id":24328,"Name":"非正常人类异闻录","Author":"精分三代","Img":"feizhengchangrenleiyiwenlu.jpg","Desc":"我叫张大道，道号张全道。在第七人民医院被人研究！\r\n　　\r\n　　    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\r\n　　\r\n　　    贫道张全道，专业摸骨批命，棺材翻新,抛光,打蜡。回收二手僵尸,寻龙点穴、批发黑驴蹄、黑狗血。代写1~3年级小学作业，寻找走失猫狗，抓小三。\r\n　　\r\n　　    专业报仇打小人、改风水、妨祖坟！量大从优！有发票！\r\n　　\r\n　　    ~~~~~","CName":"都市言情","Score":9.5},{"Id":3051,"Name":"遮天","Author":"辰东","Img":"zhetian.jpg","Desc":"冰冷与黑暗并存的宇宙深处，九具庞大的龙尸拉着一口青铜古棺，亘古长存。这是太空探测器在枯寂的宇宙中捕捉到的一幅极其震撼的画面。九龙拉棺，究竟是回到了上古，还是来到了星空的彼岸？一个浩大的仙侠世界，光怪陆离，神秘无尽。热血似火山沸腾，激情若瀚海汹涌，欲望如深渊无止境……登天路，踏歌行，弹指遮天。","CName":"武侠仙侠","Score":8.6},{"Id":292949,"Name":"我有一座恐怖屋","Author":"我会修空调","Img":"woyouyizuokongbuwu.jpg","Desc":"散发异味的灵车停在了门口，天花板传来弹珠碰撞的声音，走廊里有人来回踱步，隔壁房间好像在切割什么东西。\r\n　　卧室的门锁轻轻颤动，卫生间里水龙头已经拧紧，却还是滴答滴答个不停。\r\n　　床底下隐隐约约，似乎有个皮球滚来滚去。\r\n　　一个个沾染水渍的脚印不断在地板上浮现，正慢慢逼近。\r\n　　凌晨三点，陈歌握着菜刀躲在暖气片旁边，手里的电话刚刚拨通。\r\n　　“房东！这就是你说的晚上有点热闹？！”","CName":"科幻灵异","Score":9.5},{"Id":78031,"Name":"一念永恒","Author":"耳根","Img":"yinianyongheng.jpg","Desc":"一念成沧海，一念化桑田。一念斩千魔，一念诛万仙。唯我念……永恒","CName":"武侠仙侠","Score":8.3},{"Id":248872,"Name":"诡秘之主","Author":"爱潜水的乌贼","Img":"guimizhizhu.jpg","Desc":"蒸汽与机械的浪潮中，谁能触及非凡？历史和黑暗的迷雾里，又是谁在耳语？我从诡秘中醒来，睁眼看见这个世界：枪械，大炮，巨舰，飞空艇，差分机；魔药，占卜，诅咒，倒吊人，封印物……光明依旧照耀，神秘从未远离，这是一段“愚者”的传说。","CName":"玄幻奇幻","Score":9.2},{"Id":512195,"Name":"万族之劫","Author":"老鹰吃小鸡","Img":"wanzuzhijie.jpg","Desc":"我是这诸天万族的劫！\r\n　　已有完本作品《全球高武》《重生之财源滚滚》，没看过的书友可以去看看，新书收藏一下慢慢养。","CName":"都市言情","Score":8.1},{"Id":2802,"Name":"星辰变","Author":"我吃西红柿","Img":"xingchenbian.jpg","Desc":"一名孩童，天生无法修炼内功。为了得到父亲的重视关注，他毅然选择了修炼痛苦艰难的外功。春去秋来，时光如梭，这个孩童长大了……变成了一名青年，真正改变他的命运，是一颗流星化作的神秘晶石——流星泪。这颗流星泪在青年无所觉中，融入了青年的体内，青年他也仿佛破茧化蝶一般蜕变……而随之而来的，一切都发生了变化。而他的父亲也终于知道了他从来没有真正倾注心力的儿子的惊人实力……《星辰变》将改编成网游《星","CName":"武侠仙侠","Score":8.1}],"Page":1,"HasNext":true}}

-----------------------------------------精选结束 分类开始-----------------------------------
### 小说 分类 
GET https://scxs.pigqq.com/Categories/BookCategory.html HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
Content-Type: application/x-www-form-urlencoded
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Host: scxs.pigqq.com
Connection: Keep-Alive
Accept-Encoding: gzip

{"status":1,"info":"success","data":[{"Id":"1","Name":"玄幻奇幻","Count":121528,"Image":"https://quapp.yphsy.com/BookFiles/CategorImage/1.png"},{"Id":"2","Name":"武侠仙侠","Count":38126,"Image":"https://quapp.yphsy.com/BookFiles/CategorImage/2.png"},{"Id":"3","Name":"都市言情","Count":68280,"Image":"https://quapp.yphsy.com/BookFiles/CategorImage/3.png"},{"Id":"4","Name":"历史军事","Count":18359,"Image":"https://quapp.yphsy.com/BookFiles/CategorImage/4.png"},{"Id":"5","Name":"科幻灵异","Count":43767,"Image":"https://quapp.yphsy.com/BookFiles/CategorImage/5.png"},{"Id":"6","Name":"网游竞技","Count":13496,"Image":"https://quapp.yphsy.com/BookFiles/CategorImage/6.png"},{"Id":"7","Name":"女生频道","Count":125434,"Image":"https://quapp.yphsy.com/BookFiles/CategorImage/7.png"},{"Id":"66","Name":"同人小说","Count":4842,"Image":"https://quapp.yphsy.com/BookFiles/CategorImage/66.png"}]}

### 小说 分类 最热
GET https://scxs.pigqq.com/Categories/1/hot/1.html HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
Content-Type: application/x-www-form-urlencoded
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Host: scxs.pigqq.com
Connection: Keep-Alive
Accept-Encoding: gzip

{"status":1,"info":"success","data":{"BookList":[{"Id":671,"Name":"校花的贴身高手","Author":"鱼人二代","Img":"671.jpg","Desc":"校花的贴身高手最新章节列：小说《校花的贴身高手》鱼人二代/著,校花的贴身高手全文阅读一个大山里走出来的绝世高手，一块能预知未来的神秘玉佩……林逸是一名普通学生，不过，他还身负另外一个重任，那就是追校花！......","CName":"玄幻奇幻","Score":2.5},{"Id":11,"Name":"武炼巅峰","Author":"莫默","Img":"11.jpg","Desc":"武炼巅峰最新章节列：小说《武炼巅峰》莫默/著,武炼巅峰全文阅读[新人写作季作品]武之巅峰，是孤独，是寂寞，是漫漫求索，是高处不胜寒逆境中成长，绝地里求生，不屈不饶，才能堪破武之极道。凌霄阁试炼弟子兼扫地小......","CName":"玄幻奇幻","Score":7.5},{"Id":3253,"Name":"帝霸","Author":"厌笔萧生","Img":"diba.jpg","Desc":"千万年前，李七夜栽下一株翠竹。八百万年前，李七夜养了一条鲤鱼。五百万年前，李七夜收养一个小女孩。…………………………今天，李七夜一觉醒来，翠竹修练成神灵，鲤鱼化作金龙，小女孩成为九界女帝。这是一个养成的故事，一个不死的人族小子养成了妖神、养成了仙兽、养成了女帝的故事","CName":"玄幻奇幻","Score":4.2},{"Id":1588,"Name":"都市奇门医圣","Author":"一念","Img":"doushiqimenyisheng.jpg","Desc":"实习医生叶皓轩，意外的得到一本古书上的玄术与医道传承，自此开始了不一样的人生，他银针渡人，术法渡鬼，成就济世仁心，都市生活逍遥自在，校花、御姐加熟女，教师、医生和白领！且看叶皓轩如何在这风骚的大都市混迹花丛","CName":"玄幻奇幻","Score":7.4},{"Id":44,"Name":"混沌剑神","Author":"心星逍遥","Img":"44.jpg","Desc":"剑尘，江湖中公认的第一高手，一手快剑法出神入化，无人能破，当他与消失百年的绝世高手独孤求败一战之后，.........","CName":"玄幻奇幻","Score":6.1},{"Id":1717,"Name":"女总裁的贴身兵王","Author":"黑夜不寂寞","Img":"nvzongcaidetieshenbingwang.jpg","Desc":"他是华夏超级兵王，更是让所有势力恐惧的“战龙”老大。他重回都市，游戏人间。身边聚集了女神级美女老婆、暴力警花、熟美的办公室主任、淡雅的大学导师、清纯的小秘书，冷艳的黑道美女等一系列的各色极品美女。最要命的是每一个女人的身上都带着一堆甩不掉的麻烦。","CName":"玄幻奇幻","Score":6.7},{"Id":3230,"Name":"逆天邪神","Author":"火星引力","Img":"nitianxieshen.jpg","Desc":"掌天毒之珠，承邪神之血，修逆天之力，一代邪神，君临天下！【添加微信公众号：火星引力】【我们的YY频道：49554】......","CName":"玄幻奇幻","Score":8.0},{"Id":116,"Name":"傲世丹神","Author":"寂小贼","Img":"116.jpg","Desc":"少年沈翔艳遇神女和魔女，得到她们的无上传承，获得逆天神脉，学得绝世神功，掌握超绝丹术，这使他在武道之.........","CName":"玄幻奇幻","Score":7.0},{"Id":17779,"Name":"万古神帝","Author":"飞天鱼","Img":"wangushendi.jpg","Desc":"【NEXTIDEA暨2015星创奖征文大赏（玄幻）】\r\n　　\r\n　　    八百年前，明帝之子张若尘，被他的未婚妻池瑶公主杀死，一代无上天骄，就此陨落。\r\n　　\r\n　　    八百年后，张若尘重新活了过来，却发现曾经杀死他的未婚妻，已经统一昆仑界，开辟出第一中央帝国，号称“池瑶女皇”。\r\n　　\r\n　　    池瑶女皇——统御天下，威临八方；青春永驻，不死不灭。\r\n　　\r\n　　    张若尘站在诸皇祠堂外，望着池瑶女皇的神像，心中","CName":"玄幻奇幻","Score":8.1},{"Id":23,"Name":"龙血战神","Author":"风青阳","Img":"23.jpg","Desc":"【微信公众平台已开，请用微信添加：风青阳】太初时代，龙祭大陆乃远古神龙之天下。时至今日，神龙灭绝殆.........","CName":"玄幻奇幻","Score":6.9},{"Id":1420,"Name":"绝世邪神","Author":"纯情犀利哥","Img":"1420.jpg","Desc":"绝世邪神绝世邪神是纯情犀利哥写的玄幻异界类小说....重生异世，放荡不羁的叶楚面对众多绝世天才，倾世红颜。他如何踏破苍穹，让或冷艳或性感的佳人随他一起涨姿势？！......","CName":"玄幻奇幻","Score":5.4},{"Id":7818,"Name":"灭世武修","Author":"天上无鱼","Img":"mieshiwuxiu.jpg","Desc":"从一个闪耀之星，跌落到世人白眼。体味人生百态，尝遍世态炎凉。总有一天，神体将会崛起。芸芸众生，皆为我有。乌恒。","CName":"玄幻奇幻","Score":6.4},{"Id":9656,"Name":"武神血脉","Author":"刚大木","Img":"wushenxuemai.jpg","Desc":"【2014星创奖第一季参赛作品】\r\n　　\r\n　　    少年李叶，偶得太古血祖之神瞳，融合成自身神级血脉，从此鲤鱼跃龙门，彗星般崛起！修武道巅峰，踏上成神之路，收各路美女为眷族，笑傲苍穹！\r\n　　\r\n　　    建了一个书友群：168141063","CName":"玄幻奇幻","Score":6.2},{"Id":5071,"Name":"百炼飞升录","Author":"虚眞","Img":"bailianfeishenglu.jpg","Desc":"山村少年，历经种种，加入落霞宗，开始修真路，意外服下的无名朱果，将给他带来怎样的机遇？以赤子之心入道，又将经历怎样的诡异与浮沉？独身闯荡大陆，历经万千艰险，既已选择了非人之路，便永无回头。仙路茫茫，美人如画，朋友？知己？漫漫仙途路，千锤百炼，终飞升仙界巅峰！----------------------------------------------------------作者朋友群（","CName":"玄幻奇幻","Score":8.2},{"Id":10640,"Name":"九阳帝尊","Author":"剑棕","Img":"jiuyangdizun.jpg","Desc":"一场奇遇，一头比山岳还要大的金翅大鹏，成了少年楚晨的分身，从此他获得了进入神墓的资格，神墓中有裸身仙女冰封在玉棺之中，有上古仙器灭天辟魔神梭……无数的丹药法宝，神符圣兵，全部由他随意拾取！","CName":"玄幻奇幻","Score":8.1},{"Id":9172,"Name":"龙纹战神","Author":"苏月夕","Img":"longwenzhanshen.jpg","Desc":"天下第一圣重生百年后，修无上神功，争霸天下。\r\n　　\r\n　　    别跟我比炼丹，十成丹随手就来。\r\n　　\r\n　　    别跟我比晋级速度，羞死你我可不负责。\r\n　　\r\n　　    别跟我比修炼经验，我是老祖。\r\n　　\r\n　　    江尘的存在，注定要羞煞万千天才……\r\n　　\r\n　　    【三本完本记录，人品值饱满，群：102827635】","CName":"玄幻奇幻","Score":7.0},{"Id":52076,"Name":"武道大帝","Author":"忘情至尊","Img":"wudaodadi.jpg","Desc":"少年罗修出身卑微，天赋一般，却意外融合生死法则本源所化至宝，从此身藏诸天生死轮，执掌轮回，开创无上神通，成就一代大帝，傲视古今","CName":"玄幻奇幻","Score":6.8},{"Id":485,"Name":"斗破苍穹之无上之境","Author":"夜雨闻铃0","Img":"485.jpg","Desc":"斗破苍穹之无上之境最新章节列：小说《斗破苍穹之无上之境》夜雨闻铃0/著,斗破苍穹之无上之境全文阅读结束，也是一种开始……《斗破苍穹之无上之境》，这是一本斗破续，在这本斗破当中，你们依然会见到繁衍到巅峰的斗......","CName":"玄幻奇幻","Score":7.0},{"Id":9697,"Name":"九域神皇","Author":"我是多余人","Img":"jiuyushenhuang.jpg","Desc":"【中国梦征文参赛作品】\r\n　　\r\n　　    玄域武医门最年轻的武医王，被师弟偷袭，带着浩然霸体传承重生到凡域一个小家族子弟身上。\r\n　　\r\n　　    浩然霸体，神级传承，最强体质！\r\n　　\r\n　　    浩瀚九域，强者如云，天才横出，佳人绝世，秦川一路高歌猛进，打恶少、打纨绔、打天才、打强者……\r\n　　\r\n　　    这一世他风华绝代，还要身边有风华绝代的女人！","CName":"玄幻奇幻","Score":6.6},{"Id":47879,"Name":"九星霸体诀","Author":"平凡魔术师","Img":"jiuxingbatijue.jpg","Desc":"是丹帝重生？是融合灵魂？被盗走灵根、灵血、灵骨的三无少年——龙尘，凭借着记忆中的炼丹神术，修行神秘功法九星霸体诀，拨开重重迷雾，解开惊天之局。\r\n　　\r\n　　    手掌天地乾坤，脚踏日月星辰，勾搭各色美女，镇压恶鬼邪神。\r\n　　\r\n　　    江湖传闻：龙尘一到，地吼天啸。龙尘一出，鬼泣神哭。\r\n　　\r\n　　    本故事纯属虚构，如有雷同，那就是真事儿，想要对号入座，抓紧时间进群：378037137，老魔QQ:106","CName":"玄幻奇幻","Score":8.0},{"Id":1651,"Name":"逆天武神","Author":"书狂人","Img":"nitianwushen.jpg","Desc":"","CName":"玄幻奇幻","Score":5.7}],"Page":1,"HasNext":true}}

### 小说 分类 最新
GET https://scxs.pigqq.com/Categories/1/new/1.html HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
Content-Type: application/x-www-form-urlencoded
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Host: scxs.pigqq.com
Connection: Keep-Alive
Accept-Encoding: gzip

{"status":1,"info":"success","data":{"BookList":[{"Id":633957,"Name":"重瞳至尊","Author":"石毅","Img":"zhongtongzhizun.jpg","Desc":"刚转世就躺在了一个小黑屋里，旁边是刚被取下骨头的弟弟……等等，他们叫他什么？石昊？快快快，把骨头给他放回去！","CName":"玄幻奇幻","Score":6.0},{"Id":633945,"Name":"林辰","Author":"黑暗火龙","Img":"linchen.jpg","Desc":"天灵大陆，武道为尊！强者可以遨游天地，威震山河，翻手苍穹覆灭，弹指日月变色！\\n\\n神州大地年轻的武学宗师林辰，意外带着一尊神秘小鼎来到这个世界，成为雁南域天极宗的外门弟子。自此，海阔凭鱼跃，天高任鸟飞！且看林辰如何在这异界一步步踏上巅峰，凌九霄，破万劫，终成一代绝世剑神！","CName":"玄幻奇幻","Score":6.0},{"Id":633944,"Name":"无上剑人","Author":"林辰","Img":"wushangjianren.jpg","Desc":"天灵大陆，武道为尊！强者可以遨游天地，威震山河，翻手苍穹覆灭，弹指日月变色！\\n\\n神州大地年轻的武学宗师林辰，意外带着一尊神秘小鼎来到这个世界，成为雁南域天极宗的外门弟子。自此，海阔凭鱼跃，天高任鸟飞！且看林辰如何在这异界一步步踏上巅峰，凌九霄，破万劫，终成一代绝世剑神！","CName":"玄幻奇幻","Score":6.0},{"Id":633943,"Name":"绝世剑神","Author":"林辰","Img":"jueshijianshen.jpg","Desc":"天灵大陆，武道为尊！强者可以遨游天地，威震山河，翻手苍穹覆灭，弹指日月变色！\\n\\n神州大地年轻的武学宗师林辰，意外带着一尊神秘小鼎来到这个世界，成为雁南域天极宗的外门弟子。自此，海阔凭鱼跃，天高任鸟飞！且看林辰如何在这异界一步步踏上巅峰，凌九霄，破万劫，终成一代绝世剑神！","CName":"玄幻奇幻","Score":6.0},{"Id":633942,"Name":"江离","Author":"梦入神机","Img":"jiangli.jpg","Desc":"当人类开始踏入星河时代，古老的修行就焕发出来了新的生命力。修行，无论在任何时代永远不会过时。金刚经中，须菩提问释迦牟尼，“要成佛，如何降服其心？”。一句话，就道尽了修行的真谛，四个字，降服其心。心神通广大，所以孙悟空又叫做心猿。每一个人的心灵就是一尊孙悟空，降服心猿，就可成斗战胜佛。在星河大帝...","CName":"玄幻奇幻","Score":6.0},{"Id":633941,"Name":"星河无敌争霸","Author":"江离","Img":"xinghewudizhengba.jpg","Desc":"当人类开始踏入星河时代，古老的修行就焕发出来了新的生命力。修行，无论在任何时代永远不会过时。金刚经中，须菩提问释迦牟尼，“要成佛，如何降服其心？”。一句话，就道尽了修行的真谛，四个字，降服其心。心神通广大，所以孙悟空又叫做心猿。每一个人的心灵就是一尊孙悟空，降服心猿，就可成斗战胜佛。在星河大帝...","CName":"玄幻奇幻","Score":6.0},{"Id":633940,"Name":"水晶冥想","Author":"江离","Img":"shuijingmingxiang.jpg","Desc":"当人类开始踏入星河时代，古老的修行就焕发出来了新的生命力。修行，无论在任何时代永远不会过时。金刚经中，须菩提问释迦牟尼，“要成佛，如何降服其心？”。一句话，就道尽了修行的真谛，四个字，降服其心。心神通广大，所以孙悟空又叫做心猿。每一个人的心灵就是一尊孙悟空，降服心猿，就可成斗战胜佛。在星河大帝...","CName":"玄幻奇幻","Score":6.0},{"Id":633939,"Name":"星河大帝","Author":"江离","Img":"xinghedadi.jpg","Desc":"当人类开始踏入星河时代，古老的修行就焕发出来了新的生命力。修行，无论在任何时代永远不会过时。金刚经中，须菩提问释迦牟尼，“要成佛，如何降服其心？”。一句话，就道尽了修行的真谛，四个字，降服其心。心神通广大，所以孙悟空又叫做心猿。每一个人的心灵就是一尊孙悟空，降服心猿，就可成斗战胜佛。在星河大帝...","CName":"玄幻奇幻","Score":6.0},{"Id":633930,"Name":"玄幻：万界典狱长","Author":"吃饭睡觉","Img":"xuanhuanwanjiedianyuzhang.jpg","Desc":"“玄霜大帝，再不起来铲屎我就打你屁股了！”“紫霞仙女，快来给本狱长泡个脚按个摩！”“琉光天使，变的再软一点，嗯！舒服！”这是一个万界大佬都被主角关进‘道狱’劳动改造的故事，轻松，欢乐，爽爽爽！","CName":"玄幻奇幻","Score":6.0},{"Id":633922,"Name":"霍格沃茨的考古学家","Author":"压力位","Img":"huogewocidekaoguxuejia.jpg","Desc":"古灵阁最优秀的解咒员，魔法界的考古学家，霍格沃茨的古代魔法教授，纯血统优越主义的破坏者，西弗勒斯·斯内普的克星——\r\n　　托比·海默。","CName":"玄幻奇幻","Score":6.0},{"Id":633921,"Name":"精灵之直播大师","Author":"爱人火枪手","Img":"jinglingzhizhibodashi.jpg","Desc":"“孵蛋一场梦！孵蛋一场梦！”\r\n　　“兄弟萌，我要开始孵蛋了！”\r\n　　……\r\n　　孵蛋区UP主杨诞在河边钓鱼时意外捡到了一枚漂亮的蛋。\r\n　　“兄弟萌，你们有人知道……这是什么蛋吗？”\r\n　　“哈哈哈，这怎么可能是精灵蛋嘛！度娘的搜索有问题！”\r\n　　……\r\n　　然而当蛋里的萌物破壳的那一刻……\r\n　　杨诞冲出了自己家的家门。\r\n　　望着蓝蓝的天空、刺眼的阳光下翱翔者一群只存在于青春记忆里的精灵","CName":"玄幻奇幻","Score":6.0},{"Id":633913,"Name":"我为熊人族！开局伴生重生女帝","Author":"如你初见","Img":"woweixiongrenzu_kaijubanshengzhongshengnvdi.jpg","Desc":"魔前一叩三千年，回首凡尘不做仙！\\n我叫陈梦晨，为救因我而惨死陨落的伴生兽天，踏破九霄，历经千劫，最后耗尽心血而死。\\n重生归来。\\n这一世，不为成仙，只为护你周全！\\n我叫林天，林天的林，林天的天。\\n屌丝一枚，不幸喝水穿越，成为这方玄幻世界唯一的食铁兽！\\n身边时常跟着一枚冰山御姐。\\n她，天骄绝伦，身怀万古凰体。\\n她，身份显赫强大，执掌天道之权柄！\\n然，却对我百依百顺。\\n【叮！宿主当前","CName":"玄幻奇幻","Score":6.0},{"Id":633911,"Name":"娘胎签到三百天，出生渡劫成圣","Author":"踏碎凌霄","Img":"niangtaiqiandaosanbaitianchushengdujiechengsheng.jpg","Desc":"【娘胎修道+开局无敌+爽文】林风没想到自己竟穿成了婴儿，娘胎里辛辛苦苦签到三百天，结果出生时系统却告知：“宿主修为过高，出生奖励为三千道准帝雷劫！”\\n林风：“系统卧槽泥马！”\\n出生准帝，这是要我无敌的节奏啊！\\n桀桀桀……\\n系统竟然如此给力，既然如此，那就别怪我了！\\n……\\n于是，林风被迫走上了一条无敌之路……","CName":"玄幻奇幻","Score":6.0},{"Id":633901,"Name":"碰瓷之王","Author":"周子然","Img":"pengcizhiwang.jpg","Desc":"颜开不过想蹭蹭热度成为天行大陆的名人而已，没想到一发不可收拾，蹭着蹭着就成了碰瓷之王。","CName":"玄幻奇幻","Score":6.0},{"Id":633900,"Name":"万界武尊","Author":"晨弈","Img":"wanjiewuzun.jpg","Desc":"这里拥有力量强大的修武者，实力主宰一切，国度、宗派等大势力独霸一方，然而这只是三界一角，在这方世界之上，更有神阶至强者横行天上地下。且看无法觉醒武脉的废物叶枫，融合诸天武法，一路崛起，上天入地，万界独尊！","CName":"玄幻奇幻","Score":6.0},{"Id":633899,"Name":"万界独尊","Author":"无忧","Img":"wanjieduzun.jpg","Desc":"这一日，林枫正在林府凝聚武魂，不想，他才刚将剑武魂修炼成雏形，未婚妻姬漫夭就趁机夺走了他的武魂，还导致其差点吐血身亡。与此同时，林枫的精神进入到了葬神之地，葬神之地神秘女子告诉林枫，他可以通过磨灭葬身于此的古神，获得庞大的武道力量跟知识。","CName":"玄幻奇幻","Score":6.0},{"Id":633896,"Name":"螟蛉之子","Author":"刘封孟达","Img":"minglingzhizi.jpg","Desc":"三国鼎立之后，吕蒙白衣渡江偷袭荆州，如果关羽被救了，会是怎样的结局？穿越到乱世的刘封还不太习惯地趴伏在奔驰的战马上，星夜赶往麦城！","CName":"玄幻奇幻","Score":6.0},{"Id":633882,"Name":"秦枫城林雯儿","Author":"爱吃大鲨鱼","Img":"qinfengchenglinwener.jpg","Desc":"九个师姐都想嫁给我！大师姐是南境军主，掌管百万雄兵，二师姐第一富豪，挥金如土，三师姐第一药师，救人无数......但这些成就以后都是我的，因为我乃药神！神医下山，救人与万世！！！","CName":"玄幻奇幻","Score":6.0},{"Id":633881,"Name":"我的九个师姐都是大佬","Author":"秦枫城林雯儿","Img":"wodejiugeshijiedoushidalao.jpg","Desc":"九个师姐都想嫁给我！大师姐是南境军主，掌管百万雄兵，二师姐第一富豪，挥金如土，三师姐第一药师，救人无数......但这些成就以后都是我的，因为我乃药神！神医下山，救人与万世！！！","CName":"玄幻奇幻","Score":6.0},{"Id":633869,"Name":"杨霄","Author":"八戒也有爱","Img":"yangxiao.jpg","Desc":"杨霄带着系统穿越到西游，开了一间书店。书店里有各种各样的小说，看了就有几率从里面得到东西，功法，丹药，法宝，天材地宝，统统可以有，只有想不到的，没有书里没有的。灵山，如来一脸懵逼地听观音报告：“佛祖，唐三藏入魔了。”如来：“你逗我？”文殊：“佛祖，孙悟空那猴子和金翅大鹏雕杀上灵山来了。”如来：“阿弥了个巴子的佛！”普贤：“佛祖，灵山上圆寂众古佛的墓被盗了。”佛祖：“……”","CName":"玄幻奇幻","Score":6.0},{"Id":633868,"Name":"看书就能变强","Author":"杨霄","Img":"kanshujiunengbianqiang.jpg","Desc":"杨霄带着系统穿越到西游，开了一间书店。书店里有各种各样的小说，看了就有几率从里面得到东西，功法，丹药，法宝，天材地宝，统统可以有，只有想不到的，没有书里没有的。灵山，如来一脸懵逼地听观音报告：“佛祖，唐三藏入魔了。”如来：“你逗我？”文殊：“佛祖，孙悟空那猴子和金翅大鹏雕杀上灵山来了。”如来：“阿弥了个巴子的佛！”普贤：“佛祖，灵山上圆寂众古佛的墓被盗了。”佛祖：“……”","CName":"玄幻奇幻","Score":6.0}],"Page":1,"HasNext":true}}

### 小说 分类 评分
GET https://scxs.pigqq.com/Categories/1/vote/1.html HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
Content-Type: application/x-www-form-urlencoded
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Host: scxs.pigqq.com
Connection: Keep-Alive
Accept-Encoding: gzip

{"status":1,"info":"success","data":{"BookList":[{"Id":569362,"Name":"黑石密码","Author":"三脚架","Img":"heishimima.jpg","Desc":"这是一种很有趣的东西，它明明黯淡黢黑，却能够散发出金色的光芒，让人为之深深着迷……","CName":"玄幻奇幻","Score":9.7},{"Id":8635,"Name":"原始战记","Author":"陈词懒调","Img":"yuanshizhanji.jpg","Desc":"这坑爹的原始部落！=====================已完结作品《回到过去变成猫》、《星级猎人》。虽然类型不同，题材、书名和简介略坑，但看过前两本喜欢陈词行文风格的朋友可以先收藏。","CName":"玄幻奇幻","Score":9.5},{"Id":279151,"Name":"若仙行","Author":"风于青萍","Img":"ruoxianxing.jpg","Desc":"地球上的修真者一朝跌入空间缝隙，带着木灵空间来到了星华大陆，一个属于修真者的大陆，开启了一段异世修真之旅。\r\n　　杜若握紧拳头，仰天长笑：“虽说这里的修士太残暴，但灵气多，妖兽多，灵植多，对我来说就是最好的时代。”\r\n　　注：女主身穿，非魂穿。","CName":"玄幻奇幻","Score":9.5},{"Id":626850,"Name":"某霍格沃茨的魔文教授","Author":"韩游思","Img":"mouhuogewocidemowenjiaoshou.jpg","Desc":"从霍格沃茨毕业三年后，菲利克斯再次走进这座魔法学校，只不过这一次，他是以教授的身份！\r\n　　麻瓜的智慧与魔法结合，会碰撞出什么样的火花？\r\n　　PS1.教授古代魔文；\r\n　　PS2.时间线，三小只二年级；","CName":"玄幻奇幻","Score":9.4},{"Id":462425,"Name":"光怪陆离侦探社","Author":"吾即正道","Img":"guangguailulizhentanshe.jpg","Desc":"一扇门在眼前展开。\r\n　　邪恶在茁壮生长，窃窃私语声从门内后溢出。\r\n　　怨毒的复眼一闪而逝，想要冲出的存在被阻隔在内，蛊惑的低语耳畔回绕。\r\n　　黏糊糊的粉色脑子嘟囔着什么。披着黄衣斗篷的人影远处注视。带着腥气的墨绿色存在在怒吼。一串奇妙的肥皂泡泡释放出友善——以及许多，许多的客人。\r\n　　它们诚挚邀请陆离，参加这个疯狂的派对。\r\n　　陆离迈步进入，步伐坚定不移。\r\n　　他没有理由拒绝。","CName":"玄幻奇幻","Score":9.4},{"Id":508397,"Name":"诡异降临到我身边","Author":"雀道天凉","Img":"guiyijianglindaowoshenbian.jpg","Desc":"我是一个穿越者，在穿越者职业技术学校学习了厨艺、写作、表演、格斗等课程，四项技能都修习到了高级，穿越的时候还自带了外挂。因为神秘侧天赋很差，所以选择了日常系世界穿越，梦想是依靠学到的技能在日常系世界成为一个文抄公，不求大富大贵，只希望自己能生活富足，穿越者职业技术学校的老师都说我的梦想很简单，也很看好我……直到我穿越到了一个被恶灵害死的少年的身上……\r\n　　事情怎么会变成这样呢？\r\n　　欢迎加入群","CName":"玄幻奇幻","Score":9.4},{"Id":276624,"Name":"文豪少女的二次元时代","Author":"松子不吃糖","Img":"wenhaoshaonvdeerciyuanshidai.jpg","Desc":"士兵：“长官，如果这场仗我没能活着回来，请告诉我老婆，她的男人是个英雄。”\r\n　　长官：“……你这单身狗哪儿来的老婆？”\r\n　　士兵：“笑话！魔少难道不是我老婆吗？”\r\n　　长官：“滚！她特么是我老婆！！！”\r\n　　*********\r\n　　这是一个笔名“魔少”的少女轻小说作家用ACG文化征全世界的故事。\r\n　　*********\r\n　　轻百合。","CName":"玄幻奇幻","Score":9.4},{"Id":473639,"Name":"霍格沃茨之血脉巫师","Author":"纯洁小天使","Img":"huogewocizhixuemaiwushi.jpg","Desc":"别人穿越霍格沃茨都是魂穿婴儿，准备充分，而悲催伊凡直接穿越到了分院仪式的会场上。\r\n　　什么？我以前还学过黑魔法？家在翻倒巷的一家黑魔法商店里？母亲是邪恶的黑巫师？\r\n　　正当伊凡担心着自己日后回家身份暴露，或将被扒皮抽骨的时候，获得了融合神奇生物血脉的能力。\r\n　　邓布利多家族为何屡得凤凰相助？胖成球的小矮星彼得为何流泪半夜出逃？\r\n　　伏地魔长着蛇精脸的幕后真相到底又是什么？\r\n　　虚实转换的","CName":"玄幻奇幻","Score":9.4},{"Id":497619,"Name":"熟睡之后","Author":"吾即正道","Img":"shushuizhihou.jpg","Desc":"游魂彷徨，蠕虫四散。\r\n　　不可见之物身边环绕，耳畔窃窃私语从何而来。\r\n　　可憎之物在深渊中等待。\r\n　　死寂无风，吹不动衣角发梢。\r\n　　牧苏注视着深渊，深渊也在注视着他。\r\n　　直到开始牧苏脱下裤子——\r\n　　深渊才不得不尴尬地移开视线。","CName":"玄幻奇幻","Score":9.3},{"Id":572059,"Name":"柯学验尸官","Author":"河流之汪","Img":"kexueyanshiguan.jpg","Desc":"本书全称：《刚穿越到柯学世界就被名侦探指认为头号犯罪嫌疑人，身为验尸官的我现在一点不慌》","CName":"玄幻奇幻","Score":9.3},{"Id":107314,"Name":"寻找走丢的舰娘","Author":"海底熔岩","Img":"xunzhaozoudiudejianniang.jpg","Desc":"当你脱坑好长时间之后你可曾想过你的姑娘们会怎样？\r\n　　港区因为长官离开而分崩离析；\r\n　　胡德带着声望离开去了遥远的城市，提尔比茨为了生活在画同人本子，弗莱彻为了几个妹妹的生活同时打着几份工，无敌的苏赫巴托尔大人一手抱着黑猫奥斯卡一手抱着凶猛的大老虎有些茫然不知所措；\r\n　　儿童节的小提尔比茨，小宅也是幼宅为了寻找自己的长官走遍千山万水，当你感受到那份心情之后只想再重建那份曾经辉煌。\r\n　　欢迎","CName":"玄幻奇幻","Score":9.3},{"Id":2620,"Name":"间客","Author":"猫腻","Img":"jianke.jpg","Desc":"世界上有两件东西能够深深地震撼人们的心灵，一件是我们心中崇高的道德准则，另一件是我们头顶上灿烂的星空——康德当许乐从这行字上收回目光，第一次真正看到尘埃后方那繁若芝麻的群星时，并没有被震撼，相反他怒了：大区天空外面的星星这么刺眼，谁能受得了？天天被这些光晃着，只怕会变成矿道上那些被大灯照成痴呆的野猫！于是许乐放弃了成为一名高贵女性战舰指挥官辅官的梦想，开始在引力的作用下，堕落，","CName":"玄幻奇幻","Score":9.3},{"Id":1144,"Name":"疯巫妖的实验日志","Author":"愤怒的松鼠","Img":"1144.jpg","Desc":"关于疯巫妖的实验日志：这是个疯狂的巫妖，带着游戏系统，祸害整个世界的故事。“看下本日的日常……又是这坑爹的两选一，毁灭任意一座三万人以上的城镇，奖励10000点邪恶点数。抢三个小朋友的棒棒糖，奖励1点。若......","CName":"玄幻奇幻","Score":9.3},{"Id":124,"Name":"无尽武装","Author":"缘分0","Img":"124.jpg","Desc":"无尽武装最新章节列：小说《无尽武装》缘分0/著,无尽武装全文阅读这里是天堂，因为这里拥有地球上拥有的一切。所有你渴望的而又得不到的，在这里都可以得到；这里是地狱，因为每个人都要在这里艰苦挣扎，然后在分不清......","CName":"玄幻奇幻","Score":9.3},{"Id":2152,"Name":"猎国","Author":"跳舞","Img":"lieguo.jpg","Desc":"“不想谋朝篡位的权臣不是一个合格的权臣……总有一天，帝国的金币上会印上老子的头像！”——夏亚雷鸣【跳舞新书，欢迎新老朋友前来捧场～】","CName":"玄幻奇幻","Score":9.3},{"Id":28172,"Name":"重生之盾御苍穹","Author":"半步沧桑","Img":"zhongshengzhidunyucangqiong.jpg","Desc":"一款划时代的网游《苍穹》；一名如冬日薄冰般脆弱的天才；一段在俗世中苦苦求存、暗淡无光的岁月；一场意外，当二十年后的灵魂与今生的躯壳重叠；铸就——一个帝国壁垒的传说………………………………………………………………………………新书《网游之枭傲天下…","CName":"玄幻奇幻","Score":9.3},{"Id":570023,"Name":"诸界之深渊恶魔","Author":"路过二次元","Img":"zhujiezhishenyuanemo.jpg","Desc":"诞生于无底深渊，舍弃过往一切。\r\n　　于杀戮与毁灭之中，带着血与火登顶至高王座！\r\n　　吾是腐化世界之死疫君王，吾是焚烧万物引导终末之终焉魔神，吾是污染规则堕化众生之邪异根源，吾是杀死佛陀侵染天道之他化大自在天魔主，吾亦是一切秩序之反面，无底深渊之主！！！","CName":"玄幻奇幻","Score":9.2},{"Id":625372,"Name":"网王之从呼吸法开始","Author":"南柯ol","Img":"wangwangzhiconghuxifakaishi.jpg","Desc":"平等院凤凰，手冢国光，迹部景吾，立海大三巨头，越前龙马…\r\n　　这是一个网球的黄金时代。\r\n　　群星闪耀！\r\n　　而意外来到网王世界，获得鬼灭之刃呼吸法传承的上衫悠，\r\n　　在这个网球为王的世界究竟会掀起什么波澜……","CName":"玄幻奇幻","Score":9.2},{"Id":606781,"Name":"女尊之男神的自我修养","Author":"二次元的土豆","Img":"nvzunzhinanshendeziwoxiuyang.jpg","Desc":"弟：“姐，咱家有钱了！妈把房子卖了！”\r\n　　姐：“嗯……不过你忘了，咱家没房子……咱妈是把你卖了……”\r\n　　弟：“？？？”\r\n　　姐：“妈叫你抽时间收拾下行李……”\r\n　　沈轩默默收拾行李，他本以为穿越女尊世界的他未来将会轻松无比，没想到这就被卖到当红小鲜肉家打工……\r\n　　……\r\n　　本作品纯属虚构，作品中出现的世界、人物、事件、团体等均为剧情所需设置，请勿代入现实。\r\n　　本作品坚持正确的","CName":"玄幻奇幻","Score":9.2},{"Id":590079,"Name":"镇守府求生指北","Author":"海底熔岩","Img":"zhenshoufuqiushengzhibei.jpg","Desc":"穿越到游戏世界，装备数千、资源百万……好像已经不用再努力了。\r\n　　每天对着手机屏幕点点点。\r\n　　……好了，现在，你大难临头了。","CName":"玄幻奇幻","Score":9.2},{"Id":613599,"Name":"全球旧日","Author":"来份松果","Img":"quanqiujiuri.jpg","Desc":"更高文明的力量开始侵蚀整个世界。\r\n　　我们的世界秩序开始崩塌、瓦解、化为灰烬。\r\n　　名为旧日游戏的系统席卷全球；\r\n　　从此开始，为了活下来，我们能做的只有以下几点：\r\n　　一：努力在每场旧日游戏中存活下来。\r\n　　二：别动不该动的，别看不该看的，并完成每一场游戏的主线任务。\r\n　　三：‘保持理智！’\r\n　　并不包括：\r\n　　一：诓骗NPC并让其罚抄《食尸鬼教典》100次。\r\n　　二：面对深潜","CName":"玄幻奇幻","Score":9.2}],"Page":1,"HasNext":true}}

### 小说 分类 完结
GET https://scxs.pigqq.com/Categories/1/over/1.html HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
Content-Type: application/x-www-form-urlencoded
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Host: scxs.pigqq.com
Connection: Keep-Alive
Accept-Encoding: gzip

{"status":1,"info":"success","data":{"BookList":[{"Id":9080,"Name":"雪鹰领主","Author":"我吃西红柿","Img":"3513193.jpg","Desc":"深海魔兽的呼吸形成永不停息的风暴……\r\n　　\r\n　　    熔岩巨人的脚步毁灭一座座城池……\r\n　　\r\n　　    深渊恶魔想要侵入这座世界……\r\n　　\r\n　　    而神灵降临，行走人间传播他的光辉……\r\n　　\r\n　　    然而整个世界由夏族帝国‘龙山帝国’统治，这是人类的帝国，知识渊博的法师们埋首于法师塔中百年千年，骑士们巡守天空大地海洋……\r\n　　\r\n　　    在帝国的安阳行省，有一个很小很不起眼的贵族领地，叫——雪鹰领！","CName":"玄幻奇幻","Score":6.8},{"Id":819,"Name":"超品相师","Author":"九灯和善","Img":"819.jpg","Desc":"相师分九品，一品一重天风水有境界，明理，养气，修身，问道。二十一世纪的一位普通青年偶获诸葛亮生前的玄学传承，从此混迹都市，游走于高官权贵之间，豪门千金，世家小姐身侧，秦宇说：“我为超品相师，相人，相......","CName":"玄幻奇幻","Score":6.1},{"Id":5,"Name":"完美世界","Author":"辰东","Img":"5.jpg","Desc":"完美世界最新章节列：小说《完美世界》辰东/著,完美世界全文阅读完美世界是辰东写的东方玄幻类小说..........","CName":"玄幻奇幻","Score":9.0},{"Id":52,"Name":"儒道至圣","Author":"永恒之火","Img":"52.jpg","Desc":"关于儒道至圣：这是一个读书人掌握天地之力的世界。才气在身，诗可杀敌，词能灭军，文章安天下。秀才提笔，纸上谈兵；举人杀敌，出口成章；进士一怒，唇枪舌剑。圣人驾临，口诛笔伐，可诛人，可判天子无道，以一......","CName":"玄幻奇幻","Score":8.2},{"Id":7983,"Name":"太古神王","Author":"净无痕","Img":"taigushenwang.jpg","Desc":"九天大陆，天穹之上有九条星河，亿万星辰，皆为武命星辰，武道之人，可沟通星辰，觉醒星魂，成武命修士。传说，九天大陆最为厉害的武修，每突破一个境界，便能开辟一扇星门，从而沟通一颗星辰，直至，让九重天上，都有自己的武命星辰，化身通天彻地的太古神王。亿万生灵、诸天万界，秦问天笑看苍天，他要做天空，最亮的那颗星辰。","CName":"玄幻奇幻","Score":7.1},{"Id":8975,"Name":"全职法师","Author":"乱","Img":"quanzhifashi.jpg","Desc":"一觉醒来，世界大变。\r\n　　\r\n　　    熟悉的高中传授的是魔法，告诉大家要成为一名出色的魔法师。\r\n　　\r\n　　    居住的都市之外游荡着袭击人类的魔物妖兽，虎视眈眈。\r\n　　\r\n　　    崇尚科学的世界变成了崇尚魔法，偏偏有着一样以学渣看待自己的老师，一样目光异样的同学，一样社会底层挣扎的爸爸，一样纯美却不能走路的非血缘妹妹……\r\n　　\r\n　　    不过，莫凡发现绝大多数人都只能够主修一系魔法，自己却","CName":"玄幻奇幻","Score":8.6},{"Id":7423,"Name":"天域苍穹","Author":"风凌天下","Img":"cb_55f918fb5a617.jpg","Desc":"笑尽天下英雄，宇内我为君主！万水千山，以我为尊；八荒六合，唯我称雄！我欲舞风云，凌天下，踏天域，登苍穹！谁可争锋？！诸君可愿陪我，并肩凌天下，琼霄风云舞，征战这天域苍穹？！","CName":"玄幻奇幻","Score":6.8},{"Id":3258,"Name":"武神天下","Author":"禹枫","Img":"wushentianxia.jpg","Desc":"天生废武脉，十年傻子名，古老石碑，祖祠石棺。一个从边陲小城走出的少年，从修炼古老石碑内的神秘一式开始，一路高歌狂飙，打造一片属于自己的天下，挺身问剑，这一生，不弯腰！【激情，热血，红颜，腹黑，扮猪吃老虎，一个都不会少，禹枫出品，速度保证。】","CName":"玄幻奇幻","Score":6.8},{"Id":810,"Name":"极品狂少","Author":"我本疯狂","Img":"810.jpg","Desc":"身世如迷的少年，来到繁华都市，本想偷得浮生半日闲，却发现各方势力像飞蛾扑火一般涌现在他的身边……家事国事天下事，入世出世到救世，他像一头进山的猛虎，一路所向披靡！“想杀我的人很多，有人在地狱里忏悔，有人在前往地狱的路上！”——叶帆。已完本五本都市作品，皆进入起点精品频道。时隔四月，再度出击，新的征程，让我们携手再次征战——激情不灭，热血永恒！！","CName":"玄幻奇幻","Score":5.3},{"Id":9972,"Name":"无敌剑域","Author":"青鸾峰上","Img":"wudijianyu.jpg","Desc":"在这强者为尊的年代，只有不断努力，不断变强，才能够掌握自己与亲人的命运。律.法规则？那是为弱者制定的一一杨叶","CName":"玄幻奇幻","Score":6.4},{"Id":14,"Name":"灵域","Author":"逆苍天","Img":"14.jpg","Desc":"三万年前，自称为“神”的搏天族入侵灵域，百族奋起反抗，最终惨败，人族率先投诚，百族随后相继臣服。之后万年，所有种族皆被搏天族奴役，被严酷对待，生活在恐怖阴影中。搏天族征伐脚步，并未就此停止，以灵域为起始冲入各大秘境空间，四处树敌开战，战力消耗巨大，终被百族觅到机会一举击溃，不得不远遁域外星空。三万年后，在搏天族已成为古老传说的时代，一个怀有搏天族血脉的失忆少年，被寄养在一个小小家族，苟延残喘着，静候血脉觉醒的那一天到来。","CName":"东方玄幻","Score":7.8},{"Id":10,"Name":"武神空间","Author":"傅啸尘","Img":"10.jpg","Desc":"武神空间最新章节列：小说《武神空间》傅啸尘/著,武神空间全文阅读叶希文本只是地球上一个普通的大学生，却意外穿越到了一个名为真武界的世界！在这个世界中，强大的武者能翻山倒海，毁天灭地！本是资质平凡的他，......","CName":"玄幻奇幻","Score":6.8},{"Id":58140,"Name":"玄界之门","Author":"忘语","Img":"xuanjiezhimen.jpg","Desc":"天降神物！异血附体！群仙惊惧！万魔退避！一名从东洲大陆走出的少年。一具生死相依的红粉骷髅。一个立志成为至强者的故事。一个叱咤星河，大闹三界的传说。","CName":"玄幻奇幻","Score":6.2},{"Id":8168,"Name":"重生之最强剑神","Author":"天运老猫","Img":"zhongshengzhizuiqiangjianshen.jpg","Desc":"虚拟游戏纵横的时代。石峰带着重生十年的游戏记忆，一切重头再来。打造自己的游戏工作室，走出不一样的人生。游戏赚钱技巧！游戏副本攻略！游戏传奇任务！游戏装备出处！玩家所不知的战斗技巧！就连封测者都不知道秘密，统统都知道。PS：如果喜欢，请点击收藏一下。","CName":"玄幻奇幻","Score":9.0},{"Id":5330,"Name":"无上神王","Author":"草根","Img":"wushangshenwang.jpg","Desc":"为给母亲治病，孟凡违反族规私自金山采药，机缘巧合下获得一颗黑色珠子，传承不世奇功，自此逆转人生，痛打小人，越级挑战，收服灵兽，夺取神物，在强者如云的大陆，一步步踩着对手的鲜血逆天成神！作者QQ2889268620有对本书有什么好的建议的给我加我告诉我，鞠躬拜谢","CName":"玄幻奇幻","Score":6.6},{"Id":5316,"Name":"超级黄金指","Author":"道门弟子","Img":"chaojihuangjinzhi.jpg","Desc":"家里工厂突然倒闭，原本衣食无忧，每天开着宝马奔驰逗小妞的唐大少突然变成落魄少爷，原本订好的娃娃亲被悔婚。唐大少突获神奇金手指，帮助父亲重振家业。从此美丽大方瓷器，陶器；古朴厚重的青铜器；包浆的古玉，高调奢华钻石翡翠；惊心动魄的赌石，赌博；美丽警花，高门小姐，校园校花，美女护士等等接踵而至。落魄少爷不再落魄，生活发生了翻天覆地的变化。我要吃最好的，喝最好的，玩最好的。在获得异能之后，落魄大少发下狠誓","CName":"玄幻奇幻","Score":5.4},{"Id":1123,"Name":"佣兵的战争","Author":"如水意","Img":"1123.jpg","Desc":"高扬是一个军迷，一个很普通的军迷，爱刀，爱枪，爱冒险。只是为了能玩到真枪而已，高扬跑去了非洲，结果遇到了空难，从此就只能在枪口下混饭吃了，因为他成了一个雇佣兵。一个军迷，能在国际佣兵界达到什么样的高......","CName":"玄幻奇幻","Score":9.0},{"Id":4092,"Name":"武灵天下","Author":"颓废的烟121","Img":"wulingtianxia.jpg","Desc":"带着异世界的吞天武灵，废物少爷绝地逆袭，一跃成为震惊大6的武学天才！强大的武技信手拈来，强横的敌人踩在脚下。神秘的家族，未知的领域，一切的精彩，尽在武灵天下！","CName":"玄幻奇幻","Score":7.5},{"Id":5757,"Name":"仙武同修","Author":"月如火","Img":"xianwutongxiu.jpg","Desc":"吞食仙丹后，穿越天武大陆大秦国，成为墨河城萧家无法凝聚武魂的废柴少爷，绝境之时，意外发现前世网购的《修真大全》竟暗合这世界无上奥秘，命运从此疯狂逆袭！","CName":"玄幻奇幻","Score":5.9},{"Id":1280,"Name":"造化之王","Author":"猪三不","Img":"1280.jpg","Desc":"一夜之间，少年叶真突然发现自己拥有了一项奇异的能力！山间虫兽那无意义的叫声，传入他耳中，就变得不太一样。老鼠兄弟吱吱的叫着：兄弟，后山里能让我们体型增长数十倍的宝贝快滴落了，快走！一群蚊子在叽叽喳喳......","CName":"玄幻奇幻","Score":6.8},{"Id":43679,"Name":"真武世界","Author":"蚕茧里的牛","Img":"zhenwushijie.jpg","Desc":"卷入了三十三天所有巅峰强者的一场浩劫，人皇与他的对手最终一战，打碎了深渊世界，曾经封镇深渊魔王的神器，一张神秘的紫色卡片，却消失在时空漩涡中，横穿无尽的时空。\r\n　　\r\n　　    辽阔的蛮荒，武道文明还处于初始阶段，正在缓慢发展，很多蛮荒的绝世雄主，依旧在艰难的摸索着武道之路。\r\n　　\r\n　　    一个名叫易云的少年，拿着这张不知哪里来的紫色卡片，踏上征程。\r\n　　\r\n　　    这是一个瑰丽而又充满未知的真武世界，","CName":"玄幻奇幻","Score":7.6}],"Page":1,"HasNext":true}}

### 小说 书单 最新
GET https://scxs.pigqq.com/shudan/man/all/new/1.html HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
Content-Type: application/x-www-form-urlencoded
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Host: scxs.pigqq.com
Connection: Keep-Alive
Accept-Encoding: gzip

{"status":1,"info":"success","data":[{"ListId":91553,"UserName":"15350821211","ForMan":true,"Cover":"jipinjiading.jpg","Title":"精品一绝，不同凡响。看了不后悔，不看悔断肠…","Description":"自己的书单，经典书品","BookCount":13,"CollectionCount":57,"CommendCount":17,"IsCheck":true,"AddTime":"2021/09/14 15:07:23","UpdateTime":"2021/09/14 15:07:23"},{"ListId":91547,"UserName":"17670452486","ForMan":true,"Cover":"https://imgapixs.pysmei.com/bookfiles/bookimages/chongzushizenyanglianchengde.jpg","Title":"虫族，科幻，宇宙中的孤独","Description":"个人收藏的科幻宇宙文","BookCount":8,"CollectionCount":91,"CommendCount":19,"IsCheck":true,"AddTime":"2021/09/14 10:02:50","UpdateTime":"2021/09/14 10:02:50"},{"ListId":91497,"UserName":"18148174593","ForMan":true,"Cover":"daqin_buzhuangle_nidiewoshiqinshihuang.jpg","Title":"高智商一直在线，书籍专单","Description":"一些高智商看的书，，老铁没毛病","BookCount":42,"CollectionCount":80,"CommendCount":17,"IsCheck":true,"AddTime":"2021/09/12 22:26:25","UpdateTime":"2021/09/12 22:26:25"},{"ListId":91482,"UserName":"15779002339","ForMan":true,"Cover":"wanjiaqingshangche.jpg","Title":"拒绝书荒，每本书都是精品。","Description":"这是从我书架里精心挑选的，绝对很好看。","BookCount":50,"CollectionCount":86,"CommendCount":20,"IsCheck":true,"AddTime":"2021/09/12 16:33:01","UpdateTime":"2021/09/12 16:33:01"},{"ListId":91443,"UserName":"18867584512","ForMan":true,"Cover":"guizuwenzhang.jpg","Title":"在看的书，自己存一份，就这样，可以看看","Description":"在看的书，自己存一份，就这样，可以看看1","BookCount":99,"CollectionCount":95,"CommendCount":22,"IsCheck":true,"AddTime":"2021/09/11 23:53:15","UpdateTime":"2021/09/11 23:53:15"},{"ListId":91431,"UserName":"19932245545","ForMan":true,"Cover":"tianqiyubao.jpg","Title":"书荒的可以看一下，各个类型。。都有吧","Description":"十二年老书虫近期看的小说，不小白，看书喜欢投入进去的绝对会感到惊喜","BookCount":32,"CollectionCount":37,"CommendCount":14,"IsCheck":true,"AddTime":"2021/09/11 20:36:56","UpdateTime":"2021/09/11 20:36:56"},{"ListId":91379,"UserName":"13767995520","ForMan":true,"Cover":"shenhaocongxitongdangjikaishi.jpg","Title":"渣男后宫～重生之我真没想当男神","Description":"最好看的男频文，，，","BookCount":26,"CollectionCount":87,"CommendCount":4,"IsCheck":true,"AddTime":"2021/09/10 19:37:50","UpdateTime":"2021/09/10 19:37:50"},{"ListId":91365,"UserName":"18306410271","ForMan":true,"Cover":"wozaifanrenkexuexiuxian.jpg","Title":"真心推荐，读起来上瘾","Description":"看书7七年来的真心推荐","BookCount":8,"CollectionCount":8,"CommendCount":5,"IsCheck":true,"AddTime":"2021/09/10 12:08:04","UpdateTime":"2021/09/10 12:08:04"},{"ListId":91153,"UserName":"17503082254","ForMan":true,"Cover":"wozaijuedoudoushiwankapai.jpg","Title":"好看的，后宫，历史，创意，诸天，搞笑","Description":"我认为都很好看，由其是万界圆梦师","BookCount":55,"CollectionCount":435,"CommendCount":237,"IsCheck":true,"AddTime":"2021/09/05 20:27:21","UpdateTime":"2021/09/05 20:27:21"},{"ListId":91150,"UserName":"19176917809","ForMan":true,"Cover":"zhenlidadi.jpg","Title":"杀伐果断主角不圣母，升级流","Description":"杀伐果断，不圣母，狠辣果决","BookCount":16,"CollectionCount":288,"CommendCount":301,"IsCheck":true,"AddTime":"2021/09/05 19:16:10","UpdateTime":"2021/09/05 19:16:10"},{"ListId":91125,"UserName":"15074596402","ForMan":true,"Cover":"hanshixianlu.jpg","Title":"种田流，发展，修仙家族类小说","Description":"喜欢看种田流的不要错过了，这些小说攒了很久才有的","BookCount":19,"CollectionCount":297,"CommendCount":224,"IsCheck":true,"AddTime":"2021/09/05 14:01:53","UpdateTime":"2021/09/05 14:01:53"},{"ListId":91045,"UserName":"C60920018","ForMan":true,"Cover":"zhangshengzhiyi_kaijucaishikoubeizhanshou.jpg","Title":"精品推荐，拒绝无脑小白","Description":"万界，仙侠，无限，同人","BookCount":40,"CollectionCount":286,"CommendCount":153,"IsCheck":true,"AddTime":"2021/09/04 00:17:59","UpdateTime":"2021/09/04 00:17:59"},{"ListId":90981,"UserName":"18583666853","ForMan":true,"Cover":"kuaichuan：nvpei，lengjingdian.jpg","Title":"快穿女强虐渣 拒绝攻略","Description":"都是非常经典的快穿文搞笑的也有虐渣为主女强","BookCount":33,"CollectionCount":71,"CommendCount":13,"IsCheck":true,"AddTime":"2021/09/03 08:19:12","UpdateTime":"2021/09/03 08:19:12"},{"ListId":90931,"UserName":"jsnlovedie","ForMan":true,"Cover":"weimianchengshenzhixukongjie.jpg","Title":"万界，诸天，系统，穿越，同人，二次元，后宫等等","Description":"都看过了，求同类型。。。。。。。。。。。。。。","BookCount":79,"CollectionCount":294,"CommendCount":147,"IsCheck":true,"AddTime":"2021/09/02 10:26:38","UpdateTime":"2021/09/02 10:26:38"},{"ListId":90915,"UserName":"13755614860","ForMan":true,"Cover":"xianyuguaishouhennuli.jpg","Title":"食之无味，弃之可惜。","Description":"都是前面还可以，后面有点水","BookCount":80,"CollectionCount":182,"CommendCount":25,"IsCheck":true,"AddTime":"2021/09/01 22:55:04","UpdateTime":"2021/09/01 22:55:04"},{"ListId":90888,"UserName":"13124392063","ForMan":true,"Cover":"wodezhiyuxiyouxi.jpg","Title":"书虫推荐，精品，绝对精品","Description":"十年书虫，什么都有一些，但都是精品，二次元，后宫，克苏鲁……总之不会让人失望","BookCount":57,"CollectionCount":312,"CommendCount":63,"IsCheck":true,"AddTime":"2021/09/01 11:45:26","UpdateTime":"2021/09/01 11:45:26"},{"ListId":90867,"UserName":"18256037760","ForMan":true,"Cover":"shenjijidi.jpg","Title":"20年老书虫，让你告别书荒","Description":"穿越，系统，修仙，恐怖，都市，全部都是经典，不看是你的损失。","BookCount":100,"CollectionCount":150,"CommendCount":26,"IsCheck":true,"AddTime":"2021/09/01 00:50:35","UpdateTime":"2021/09/01 00:50:35"},{"ListId":90848,"UserName":"13250842827","ForMan":true,"Cover":"rangangzhihun.jpg","Title":"黑暗  灵异恐怖 武侠 无限","Description":"看过的小说，各种都有","BookCount":51,"CollectionCount":104,"CommendCount":33,"IsCheck":true,"AddTime":"2021/08/31 19:36:20","UpdateTime":"2021/08/31 19:36:20"},{"ListId":90847,"UserName":"18850628812","ForMan":true,"Cover":"zhutianciyuanzhangkongzhe.jpg","Title":"无限、修真、卡牌","Description":"都是很不错且值得一看的书","BookCount":14,"CollectionCount":56,"CommendCount":30,"IsCheck":true,"AddTime":"2021/08/31 19:29:28","UpdateTime":"2021/08/31 19:29:28"},{"ListId":90720,"UserName":"15919790246","ForMan":true,"Cover":"bukexueyushou.jpg","Title":"种田文，系统文，历史，同人，游戏","Description":"内容不错的小说。。。。。","BookCount":21,"CollectionCount":61,"CommendCount":28,"IsCheck":true,"AddTime":"2021/08/29 23:31:57","UpdateTime":"2021/08/29 23:31:57"},{"ListId":90713,"UserName":"16638685984","ForMan":true,"Cover":"moriyuanhuan.jpg","Title":"让你看到不想睡觉，熬夜吧，兄弟","Description":"巨好看后宫文男主智商爆表，剧情巨流畅","BookCount":22,"CollectionCount":160,"CommendCount":52,"IsCheck":true,"AddTime":"2021/08/29 22:25:43","UpdateTime":"2021/08/29 22:25:43"}]}

### 小说 书单 本周最热
GET https://scxs.pigqq.com/shudan/man/all/hot/1.html HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
Content-Type: application/x-www-form-urlencoded
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Host: scxs.pigqq.com
Connection: Keep-Alive
Accept-Encoding: gzip

{"status":1,"info":"success","data":[{"ListId":32982,"UserName":"shudan666","ForMan":true,"Cover":"https://imgapi.jiaston.com/BookFiles/BookImages/zhutianjutouqun.jpg","Title":"制霸诸天万界","Description":"穿越到异界，成为诸天聊天群的群主。","BookCount":8,"CommendImage":"https://imgapi.xllxdg.com/shudan/images/32982.jpg","CollectionCount":44489,"CommendCount":18055,"IsCheck":true,"AddTime":"2019/09/05 01:24:38","UpdateTime":"2019/09/05 18:28:09"},{"ListId":892,"UserName":"13655825179","ForMan":true,"Cover":"mofamiandianshi.jpg","Title":"二次元类的同人以及宅系精品","Description":"精品同人，第一次推书，不过都是我认为很好看的书，不看后悔","BookCount":123,"CollectionCount":23924,"CommendCount":2294,"IsCheck":true,"AddTime":"2018/01/19 20:40:55","UpdateTime":"2020/01/15 18:12:12"},{"ListId":2529,"UserName":"93219686","ForMan":true,"Cover":"shouxuefeiteng.jpg","Title":"种马后宫！一男多女主的小说","Description":"各类都有个人比较喜欢动漫的","BookCount":13,"CollectionCount":23629,"CommendCount":2595,"IsCheck":true,"AddTime":"2018/03/06 00:44:55","UpdateTime":"2018/03/11 18:08:24"},{"ListId":6212,"UserName":"18756802952","ForMan":true,"Cover":"zuiqiangshenhuadihuang.jpg","Title":"爽文，系统流","Description":"书荒看看，爽文不虐。。。。","BookCount":52,"CollectionCount":18334,"CommendCount":1786,"IsCheck":true,"AddTime":"2018/06/04 08:45:47","UpdateTime":"2018/06/06 15:34:29"},{"ListId":37005,"UserName":"13315398495","ForMan":true,"Cover":"sinveciyuandewuxianjianzhi.jpg","Title":"同人小说，二次元等","Description":"分享，个人用，感觉挺有意思的","BookCount":252,"CollectionCount":14355,"CommendCount":1158,"IsCheck":true,"AddTime":"2019/11/19 20:48:04","UpdateTime":"2019/11/19 23:49:34"},{"ListId":344,"UserName":"18585892214","ForMan":true,"Cover":"bianshenhuajiluoli.jpg","Title":"二次元，变身流，非极品不要","Description":"各种变身小说，基本好看的都在这里了还有里面有个9.8分的书是系统强行放进来的，我删不掉勿喷","BookCount":19,"CollectionCount":13509,"CommendCount":1586,"IsCheck":true,"AddTime":"2017/12/31 01:48:36","UpdateTime":"2019/04/25 00:15:16"},{"ListId":36052,"UserName":"shudan666","ForMan":true,"Cover":"https://imgapi.jiaston.com/BookFiles/BookImages/wosidangchuanyuele.jpg","Title":"我能无限穿越","Description":"当流浪地球穿越到无限世界，会发生什么事呢？","BookCount":8,"CommendImage":"https://imgapi.jiaston.com/shudan/images/36052.jpg","CollectionCount":12565,"CommendCount":4646,"IsCheck":true,"AddTime":"2019/11/03 16:15:56","UpdateTime":"2019/11/03 17:46:36"},{"ListId":6,"UserName":"风一样的男人","ForMan":true,"Cover":"buxiufanren.jpg","Title":"热血澎湃，装逼打脸！","Description":"不拜神佛仙灵，不惧妖魔鬼魅！","BookCount":19,"CommendImage":"https://image.zsdfm.com/shudan/images/6.jpg","CollectionCount":10656,"CommendCount":4236,"IsCheck":true,"AddTime":"2017/11/22 23:08:16","UpdateTime":"2017/12/01 01:20:25"},{"ListId":7051,"UserName":"fxz199484","ForMan":true,"Cover":"wanjielvxingzhe.jpg","Title":"各种爽文，主穿越，面位，同人，各种经典。","Description":"爽文，同人，面位，穿越，宠物。","BookCount":100,"CollectionCount":10360,"CommendCount":705,"IsCheck":true,"AddTime":"2018/06/21 06:59:54","UpdateTime":"2018/06/22 18:58:18"},{"ListId":20,"UserName":"风一样的男人","ForMan":true,"Cover":"1279.jpg","Title":"书友公认大神100部最经典网络小说","Description":"真正的神作，真正的精品，真正的经典一百本神作！","BookCount":100,"CommendImage":"","CollectionCount":9942,"CommendCount":764,"IsCheck":true,"AddTime":"2017/11/25 05:21:37","UpdateTime":"2017/11/30 23:04:17"},{"ListId":23266,"UserName":"13059413837","ForMan":true,"Cover":"guanyuwozhuanshengbianchenghulizheidangshi.jpg","Title":"变身文，重生文，穿越文，轻松娱乐文。","Description":"自己找的书，书架已满，","BookCount":96,"CollectionCount":9321,"CommendCount":656,"IsCheck":true,"AddTime":"2019/05/03 03:24:45","UpdateTime":"2019/05/03 15:12:05"},{"ListId":36050,"UserName":"shudan666","ForMan":true,"Cover":"https://imgapi.jiaston.com/BookFiles/BookImages/cangyuantu.jpg","Title":"开局就无敌了","Description":"叮，掉落至高天赋，时空天赋。叮，掉落无上级武技，混沌青莲……","BookCount":8,"CommendImage":"https://imgapi.jiaston.com/shudan/images/36050.jpg","CollectionCount":9109,"CommendCount":1809,"IsCheck":true,"AddTime":"2019/11/03 16:06:05","UpdateTime":"2019/11/03 17:46:50"},{"ListId":515,"UserName":"风一样的男人","ForMan":true,"Cover":"http://statics.zhuishushenqi.com/agent/http%3A%2F%2Fimg.1391.com%2Fapi%2Fv1%2Fbookcenter%2Fcover%2F1%2F30170%2F_30170_873129.jpg%2F","Title":"网络文学中哪些小说能称为神作？告诉你这些就是神作","Description":"总结一下一些神作，相信大家也都知道，有遗漏的，希望大家来补充一下。","BookCount":40,"CommendImage":"https://image.zsdfm.com/shudan/images/515.jpg","CollectionCount":9009,"CommendCount":1264,"IsCheck":true,"AddTime":"2018/01/06 15:40:09","UpdateTime":"2018/03/21 11:25:21"},{"ListId":497,"UserName":"风一样的男人","ForMan":true,"Cover":"http://www.apporapp.cc/BookFiles/BookImages/bahuangjianshen.jpg","Title":"网络文学玄幻神作书单，不得不看的口碑经典，完本1000章以上！","Description":"整理一些玄幻精品书单，其实很多经典作品都集中在200万到三百万之间，感觉书单不错的话，别忘了加“收藏”。","BookCount":20,"CommendImage":"https://image.zsdfm.com/shudan/images/497.jpg","CollectionCount":8807,"CommendCount":1952,"IsCheck":true,"AddTime":"2018/01/06 01:51:29","UpdateTime":"2018/03/21 11:24:22"},{"ListId":25850,"UserName":"kenneth9999","ForMan":true,"Cover":"hunzaihaizeishijiederizi.jpg","Title":"动漫类～爽文～一级棒哟，不看看就可惜了嘿","Description":"好看到爆炸阿，伙计们不来看看可惜咯！必定遗憾终身地，还有一点嘿，你们这群凡人，系统一定会降临我身的，我才是这方世界的主角阿","BookCount":54,"CollectionCount":7241,"CommendCount":456,"IsCheck":true,"AddTime":"2019/06/16 15:00:24","UpdateTime":"2019/06/17 00:34:35"},{"ListId":5299,"UserName":"风一样的男人","ForMan":true,"Cover":"http://www.apporapp.cc/BookFiles/BookImages/quanqiujinhua.jpg","Title":"经典末世小说，都已完本，精品不容错过。","Description":"关于末世流的书单。都是精品。","BookCount":8,"CollectionCount":7085,"CommendCount":1052,"IsCheck":true,"AddTime":"2018/05/13 01:03:09","UpdateTime":"2018/05/13 14:48:12"},{"ListId":8388,"UserName":"风一样的男人","ForMan":true,"Cover":"http://www.apporapp.cc/BookFiles/BookImages/doupocangqiong.jpg","Title":"点击量破亿的十大网文小说，你看过哪些","Description":"好书推荐一下给大家，好的话记得收藏哦。","BookCount":10,"CollectionCount":6767,"CommendCount":2819,"IsCheck":true,"AddTime":"2018/07/15 18:33:25","UpdateTime":"2018/07/15 22:57:13"},{"ListId":36049,"UserName":"shudan666","ForMan":true,"Cover":"https://imgapi.jiaston.com/BookFiles/BookImages/zhutianjianglindataosha.jpg","Title":"我的末世狂想曲","Description":"生存即艺术，看到丧尸难道不该跑吗？","BookCount":8,"CommendImage":"https://imgapi.jiaston.com/shudan/images/36049.jpg","CollectionCount":6474,"CommendCount":1627,"IsCheck":true,"AddTime":"2019/11/03 16:00:59","UpdateTime":"2019/11/03 17:47:04"},{"ListId":14887,"UserName":"风一样的男人","ForMan":true,"Cover":"http://www.apporapp.cc/BookFiles/BookImages/zuiqiangfantaoluxitong.jpg","Title":"除了《大王饶命》，还有这些好看的小说，笑到让你停不下来。","Description":"推荐一些好看又搞笑的小说给大家乐一乐。","BookCount":8,"CommendImage":"https://image.zsdfm.com/shudan/images/14887.png","CollectionCount":6331,"CommendCount":1004,"IsCheck":true,"AddTime":"2018/11/14 20:09:42","UpdateTime":"2018/11/29 23:25:42"},{"ListId":7208,"UserName":"14719933678","ForMan":true,"Cover":"jianlai.jpg","Title":"各种风格，各种类型，杜绝无脑","Description":"大部分没更完，适合养着","BookCount":89,"CollectionCount":5775,"CommendCount":643,"IsCheck":true,"AddTime":"2018/06/23 23:10:29","UpdateTime":"2018/06/24 15:49:34"},{"ListId":22108,"UserName":"shudan666","ForMan":true,"Cover":"https://imgapi.jiaston.com/BookFiles/BookImages/shenzang.jpg","Title":"风水秘术局，古董宝中宝","Description":"修仙千年后，重回都市.都市修仙，鉴宝求真之路。","BookCount":9,"CommendImage":"https://image.zsdfm.com/shudan/images/22108.jpg","CollectionCount":5487,"CommendCount":2248,"IsCheck":true,"AddTime":"2019/04/08 00:12:26","UpdateTime":"2019/04/08 17:12:03"}]}

### 小说 书单 最多收藏
GET https://scxs.pigqq.com/shudan/man/all/collect/1.html HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
Content-Type: application/x-www-form-urlencoded
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Host: scxs.pigqq.com
Connection: Keep-Alive
Accept-Encoding: gzip

{"status":1,"info":"success","data":[{"ListId":32982,"UserName":"shudan666","ForMan":true,"Cover":"https://imgapi.jiaston.com/BookFiles/BookImages/zhutianjutouqun.jpg","Title":"制霸诸天万界","Description":"穿越到异界，成为诸天聊天群的群主。","BookCount":8,"CommendImage":"https://imgapi.xllxdg.com/shudan/images/32982.jpg","CollectionCount":44489,"CommendCount":18055,"IsCheck":true,"AddTime":"2019/09/05 01:24:38","UpdateTime":"2019/09/05 18:28:09"},{"ListId":36052,"UserName":"shudan666","ForMan":true,"Cover":"https://imgapi.jiaston.com/BookFiles/BookImages/wosidangchuanyuele.jpg","Title":"我能无限穿越","Description":"当流浪地球穿越到无限世界，会发生什么事呢？","BookCount":8,"CommendImage":"https://imgapi.jiaston.com/shudan/images/36052.jpg","CollectionCount":12565,"CommendCount":4646,"IsCheck":true,"AddTime":"2019/11/03 16:15:56","UpdateTime":"2019/11/03 17:46:36"},{"ListId":6,"UserName":"风一样的男人","ForMan":true,"Cover":"buxiufanren.jpg","Title":"热血澎湃，装逼打脸！","Description":"不拜神佛仙灵，不惧妖魔鬼魅！","BookCount":19,"CommendImage":"https://image.zsdfm.com/shudan/images/6.jpg","CollectionCount":10656,"CommendCount":4236,"IsCheck":true,"AddTime":"2017/11/22 23:08:16","UpdateTime":"2017/12/01 01:20:25"},{"ListId":8388,"UserName":"风一样的男人","ForMan":true,"Cover":"http://www.apporapp.cc/BookFiles/BookImages/doupocangqiong.jpg","Title":"点击量破亿的十大网文小说，你看过哪些","Description":"好书推荐一下给大家，好的话记得收藏哦。","BookCount":10,"CollectionCount":6767,"CommendCount":2819,"IsCheck":true,"AddTime":"2018/07/15 18:33:25","UpdateTime":"2018/07/15 22:57:13"},{"ListId":2529,"UserName":"93219686","ForMan":true,"Cover":"shouxuefeiteng.jpg","Title":"种马后宫！一男多女主的小说","Description":"各类都有个人比较喜欢动漫的","BookCount":13,"CollectionCount":23629,"CommendCount":2595,"IsCheck":true,"AddTime":"2018/03/06 00:44:55","UpdateTime":"2018/03/11 18:08:24"},{"ListId":892,"UserName":"13655825179","ForMan":true,"Cover":"mofamiandianshi.jpg","Title":"二次元类的同人以及宅系精品","Description":"精品同人，第一次推书，不过都是我认为很好看的书，不看后悔","BookCount":123,"CollectionCount":23924,"CommendCount":2294,"IsCheck":true,"AddTime":"2018/01/19 20:40:55","UpdateTime":"2020/01/15 18:12:12"},{"ListId":22108,"UserName":"shudan666","ForMan":true,"Cover":"https://imgapi.jiaston.com/BookFiles/BookImages/shenzang.jpg","Title":"风水秘术局，古董宝中宝","Description":"修仙千年后，重回都市.都市修仙，鉴宝求真之路。","BookCount":9,"CommendImage":"https://image.zsdfm.com/shudan/images/22108.jpg","CollectionCount":5487,"CommendCount":2248,"IsCheck":true,"AddTime":"2019/04/08 00:12:26","UpdateTime":"2019/04/08 17:12:03"},{"ListId":497,"UserName":"风一样的男人","ForMan":true,"Cover":"http://www.apporapp.cc/BookFiles/BookImages/bahuangjianshen.jpg","Title":"网络文学玄幻神作书单，不得不看的口碑经典，完本1000章以上！","Description":"整理一些玄幻精品书单，其实很多经典作品都集中在200万到三百万之间，感觉书单不错的话，别忘了加“收藏”。","BookCount":20,"CommendImage":"https://image.zsdfm.com/shudan/images/497.jpg","CollectionCount":8807,"CommendCount":1952,"IsCheck":true,"AddTime":"2018/01/06 01:51:29","UpdateTime":"2018/03/21 11:24:22"},{"ListId":36050,"UserName":"shudan666","ForMan":true,"Cover":"https://imgapi.jiaston.com/BookFiles/BookImages/cangyuantu.jpg","Title":"开局就无敌了","Description":"叮，掉落至高天赋，时空天赋。叮，掉落无上级武技，混沌青莲……","BookCount":8,"CommendImage":"https://imgapi.jiaston.com/shudan/images/36050.jpg","CollectionCount":9109,"CommendCount":1809,"IsCheck":true,"AddTime":"2019/11/03 16:06:05","UpdateTime":"2019/11/03 17:46:50"},{"ListId":6212,"UserName":"18756802952","ForMan":true,"Cover":"zuiqiangshenhuadihuang.jpg","Title":"爽文，系统流","Description":"书荒看看，爽文不虐。。。。","BookCount":52,"CollectionCount":18334,"CommendCount":1786,"IsCheck":true,"AddTime":"2018/06/04 08:45:47","UpdateTime":"2018/06/06 15:34:29"},{"ListId":36049,"UserName":"shudan666","ForMan":true,"Cover":"https://imgapi.jiaston.com/BookFiles/BookImages/zhutianjianglindataosha.jpg","Title":"我的末世狂想曲","Description":"生存即艺术，看到丧尸难道不该跑吗？","BookCount":8,"CommendImage":"https://imgapi.jiaston.com/shudan/images/36049.jpg","CollectionCount":6474,"CommendCount":1627,"IsCheck":true,"AddTime":"2019/11/03 16:00:59","UpdateTime":"2019/11/03 17:47:04"},{"ListId":344,"UserName":"18585892214","ForMan":true,"Cover":"bianshenhuajiluoli.jpg","Title":"二次元，变身流，非极品不要","Description":"各种变身小说，基本好看的都在这里了还有里面有个9.8分的书是系统强行放进来的，我删不掉勿喷","BookCount":19,"CollectionCount":13509,"CommendCount":1586,"IsCheck":true,"AddTime":"2017/12/31 01:48:36","UpdateTime":"2019/04/25 00:15:16"},{"ListId":82019,"UserName":"18007298595","ForMan":true,"Cover":"wunianbenghuaisannianmoni.jpg","Title":"同人，系统，爽文诶嘿嘿(o﹃o?)","Description":"诶嘿嘿还好还好哈-_-||","BookCount":29,"CollectionCount":1549,"CommendCount":1383,"IsCheck":true,"AddTime":"2021/05/20 10:24:39","UpdateTime":"2021/05/20 10:24:39"},{"ListId":515,"UserName":"风一样的男人","ForMan":true,"Cover":"http://statics.zhuishushenqi.com/agent/http%3A%2F%2Fimg.1391.com%2Fapi%2Fv1%2Fbookcenter%2Fcover%2F1%2F30170%2F_30170_873129.jpg%2F","Title":"网络文学中哪些小说能称为神作？告诉你这些就是神作","Description":"总结一下一些神作，相信大家也都知道，有遗漏的，希望大家来补充一下。","BookCount":40,"CommendImage":"https://image.zsdfm.com/shudan/images/515.jpg","CollectionCount":9009,"CommendCount":1264,"IsCheck":true,"AddTime":"2018/01/06 15:40:09","UpdateTime":"2018/03/21 11:25:21"},{"ListId":36048,"UserName":"shudan666","ForMan":true,"Cover":"https://imgapi.jiaston.com/BookFiles/BookImages/wuxianlingyaopu.jpg","Title":"炼药才是王道","Description":"炼最毒的药，升最快的级，吃药就能升级，谁还辛苦去pk","BookCount":8,"CommendImage":"https://imgapi.jiaston.com/shudan/images/36048.jpg","CollectionCount":3370,"CommendCount":1179,"IsCheck":true,"AddTime":"2019/11/03 15:55:47","UpdateTime":"2019/11/03 17:47:17"},{"ListId":16901,"UserName":"zero1997","ForMan":true,"Cover":"http://www.apporapp.cc/BookFiles/BookImages/sanjiehongbaoqun.jpg","Title":"各路神仙的红包都能抢？那给我来个大的","Description":"加入了一个神秘的红包群，各路神仙的红包都能抢？","BookCount":8,"CommendImage":"https://image.zsdfm.com/shudan/images/16901.jpg","CollectionCount":3456,"CommendCount":1171,"IsCheck":true,"AddTime":"2018/12/29 14:28:08","UpdateTime":"2018/12/31 19:34:11"},{"ListId":37005,"UserName":"13315398495","ForMan":true,"Cover":"sinveciyuandewuxianjianzhi.jpg","Title":"同人小说，二次元等","Description":"分享，个人用，感觉挺有意思的","BookCount":252,"CollectionCount":14355,"CommendCount":1158,"IsCheck":true,"AddTime":"2019/11/19 20:48:04","UpdateTime":"2019/11/19 23:49:34"},{"ListId":82057,"UserName":"18669612331","ForMan":true,"Cover":"guiyishijieshengcunshouce.jpg","Title":"书荒    喜欢玄幻类  求推荐","Description":"书荒喜欢玄幻类求推荐","BookCount":23,"CollectionCount":508,"CommendCount":1087,"IsCheck":true,"AddTime":"2021/05/20 22:34:44","UpdateTime":"2021/05/20 22:34:44"},{"ListId":6359,"UserName":"风一样的男人","ForMan":true,"Cover":"womenshiguanjun.jpg","Title":"足球类的十部精品小说，每一本都是不容错过的好书。","Description":"整理一下好看的足球类小说，希望大家喜欢。","BookCount":10,"CollectionCount":3516,"CommendCount":1070,"IsCheck":true,"AddTime":"2018/06/07 16:06:09","UpdateTime":"2018/06/07 16:08:28"},{"ListId":27150,"UserName":"15055885588","ForMan":true,"Cover":"https://imgapi.jiaston.com/BookFiles/BookImages/futianshi.jpg","Title":"蛰伏数年，一朝崛起雷惊天下","Description":"神雷降，天下惊。万古雷帝就此觉醒","BookCount":8,"CommendImage":"https://imgapi.jiaston.com/shudan/images/27150.jpg","CollectionCount":2479,"CommendCount":1061,"IsCheck":true,"AddTime":"2019/07/02 16:35:09","UpdateTime":"2019/07/02 19:09:58"},{"ListId":5299,"UserName":"风一样的男人","ForMan":true,"Cover":"http://www.apporapp.cc/BookFiles/BookImages/quanqiujinhua.jpg","Title":"经典末世小说，都已完本，精品不容错过。","Description":"关于末世流的书单。都是精品。","BookCount":8,"CollectionCount":7085,"CommendCount":1052,"IsCheck":true,"AddTime":"2018/05/13 01:03:09","UpdateTime":"2018/05/13 14:48:12"}]}

### 小说 书单 小编推荐
GET https://scxs.pigqq.com/shudan/man/all/commend/1.html HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
Content-Type: application/x-www-form-urlencoded
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Host: scxs.pigqq.com
Connection: Keep-Alive
Accept-Encoding: gzip

{"status":1,"info":"success","data":[{"ListId":32982,"UserName":"shudan666","ForMan":true,"Cover":"https://imgapi.jiaston.com/BookFiles/BookImages/zhutianjutouqun.jpg","Title":"制霸诸天万界","Description":"穿越到异界，成为诸天聊天群的群主。","BookCount":8,"CommendImage":"https://imgapi.xllxdg.com/shudan/images/32982.jpg","CollectionCount":44489,"CommendCount":18055,"IsCheck":true,"AddTime":"2019/09/05 01:24:38","UpdateTime":"2019/09/05 18:28:09"},{"ListId":36052,"UserName":"shudan666","ForMan":true,"Cover":"https://imgapi.jiaston.com/BookFiles/BookImages/wosidangchuanyuele.jpg","Title":"我能无限穿越","Description":"当流浪地球穿越到无限世界，会发生什么事呢？","BookCount":8,"CommendImage":"https://imgapi.jiaston.com/shudan/images/36052.jpg","CollectionCount":12565,"CommendCount":4646,"IsCheck":true,"AddTime":"2019/11/03 16:15:56","UpdateTime":"2019/11/03 17:46:36"},{"ListId":22108,"UserName":"shudan666","ForMan":true,"Cover":"https://imgapi.jiaston.com/BookFiles/BookImages/shenzang.jpg","Title":"风水秘术局，古董宝中宝","Description":"修仙千年后，重回都市.都市修仙，鉴宝求真之路。","BookCount":9,"CommendImage":"https://image.zsdfm.com/shudan/images/22108.jpg","CollectionCount":5487,"CommendCount":2248,"IsCheck":true,"AddTime":"2019/04/08 00:12:26","UpdateTime":"2019/04/08 17:12:03"},{"ListId":497,"UserName":"风一样的男人","ForMan":true,"Cover":"http://www.apporapp.cc/BookFiles/BookImages/bahuangjianshen.jpg","Title":"网络文学玄幻神作书单，不得不看的口碑经典，完本1000章以上！","Description":"整理一些玄幻精品书单，其实很多经典作品都集中在200万到三百万之间，感觉书单不错的话，别忘了加“收藏”。","BookCount":20,"CommendImage":"https://image.zsdfm.com/shudan/images/497.jpg","CollectionCount":8807,"CommendCount":1952,"IsCheck":true,"AddTime":"2018/01/06 01:51:29","UpdateTime":"2018/03/21 11:24:22"},{"ListId":36050,"UserName":"shudan666","ForMan":true,"Cover":"https://imgapi.jiaston.com/BookFiles/BookImages/cangyuantu.jpg","Title":"开局就无敌了","Description":"叮，掉落至高天赋，时空天赋。叮，掉落无上级武技，混沌青莲……","BookCount":8,"CommendImage":"https://imgapi.jiaston.com/shudan/images/36050.jpg","CollectionCount":9109,"CommendCount":1809,"IsCheck":true,"AddTime":"2019/11/03 16:06:05","UpdateTime":"2019/11/03 17:46:50"},{"ListId":36049,"UserName":"shudan666","ForMan":true,"Cover":"https://imgapi.jiaston.com/BookFiles/BookImages/zhutianjianglindataosha.jpg","Title":"我的末世狂想曲","Description":"生存即艺术，看到丧尸难道不该跑吗？","BookCount":8,"CommendImage":"https://imgapi.jiaston.com/shudan/images/36049.jpg","CollectionCount":6474,"CommendCount":1627,"IsCheck":true,"AddTime":"2019/11/03 16:00:59","UpdateTime":"2019/11/03 17:47:04"},{"ListId":515,"UserName":"风一样的男人","ForMan":true,"Cover":"http://statics.zhuishushenqi.com/agent/http%3A%2F%2Fimg.1391.com%2Fapi%2Fv1%2Fbookcenter%2Fcover%2F1%2F30170%2F_30170_873129.jpg%2F","Title":"网络文学中哪些小说能称为神作？告诉你这些就是神作","Description":"总结一下一些神作，相信大家也都知道，有遗漏的，希望大家来补充一下。","BookCount":40,"CommendImage":"https://image.zsdfm.com/shudan/images/515.jpg","CollectionCount":9009,"CommendCount":1264,"IsCheck":true,"AddTime":"2018/01/06 15:40:09","UpdateTime":"2018/03/21 11:25:21"},{"ListId":36048,"UserName":"shudan666","ForMan":true,"Cover":"https://imgapi.jiaston.com/BookFiles/BookImages/wuxianlingyaopu.jpg","Title":"炼药才是王道","Description":"炼最毒的药，升最快的级，吃药就能升级，谁还辛苦去pk","BookCount":8,"CommendImage":"https://imgapi.jiaston.com/shudan/images/36048.jpg","CollectionCount":3370,"CommendCount":1179,"IsCheck":true,"AddTime":"2019/11/03 15:55:47","UpdateTime":"2019/11/03 17:47:17"},{"ListId":16901,"UserName":"zero1997","ForMan":true,"Cover":"http://www.apporapp.cc/BookFiles/BookImages/sanjiehongbaoqun.jpg","Title":"各路神仙的红包都能抢？那给我来个大的","Description":"加入了一个神秘的红包群，各路神仙的红包都能抢？","BookCount":8,"CommendImage":"https://image.zsdfm.com/shudan/images/16901.jpg","CollectionCount":3456,"CommendCount":1171,"IsCheck":true,"AddTime":"2018/12/29 14:28:08","UpdateTime":"2018/12/31 19:34:11"},{"ListId":27150,"UserName":"15055885588","ForMan":true,"Cover":"https://imgapi.jiaston.com/BookFiles/BookImages/futianshi.jpg","Title":"蛰伏数年，一朝崛起雷惊天下","Description":"神雷降，天下惊。万古雷帝就此觉醒","BookCount":8,"CommendImage":"https://imgapi.jiaston.com/shudan/images/27150.jpg","CollectionCount":2479,"CommendCount":1061,"IsCheck":true,"AddTime":"2019/07/02 16:35:09","UpdateTime":"2019/07/02 19:09:58"},{"ListId":14887,"UserName":"风一样的男人","ForMan":true,"Cover":"http://www.apporapp.cc/BookFiles/BookImages/zuiqiangfantaoluxitong.jpg","Title":"除了《大王饶命》，还有这些好看的小说，笑到让你停不下来。","Description":"推荐一些好看又搞笑的小说给大家乐一乐。","BookCount":8,"CommendImage":"https://image.zsdfm.com/shudan/images/14887.png","CollectionCount":6331,"CommendCount":1004,"IsCheck":true,"AddTime":"2018/11/14 20:09:42","UpdateTime":"2018/11/29 23:25:42"},{"ListId":54827,"UserName":"shudan666","ForMan":true,"Cover":"https://imgapi.jiaston.com/BookFiles/BookImages/shenghuoxinanshen.jpg","Title":"职场大佬是宅男","Description":"有的人开会时是霸道总裁，冰箱厨房里却只有肥宅快乐水。","BookCount":8,"CommendImage":"https://imgapi.jiaston.com/shudan/images/54827.jpg","CollectionCount":1713,"CommendCount":925,"IsCheck":true,"AddTime":"2020/05/15 00:32:01","UpdateTime":"2020/05/15 15:21:44"},{"ListId":43105,"UserName":"shudan666","ForMan":true,"Cover":"https://imgapi.jiaston.com/BookFiles/BookImages/xiangong.jpg","Title":"少年仗剑走天下","Description":"少年意气，一刀一剑走江湖。","BookCount":8,"CommendImage":"https://imgapi.jiaston.com/shudan/images/43105.jpg","CollectionCount":2070,"CommendCount":923,"IsCheck":true,"AddTime":"2020/02/13 17:22:05","UpdateTime":"2020/02/13 22:26:00"},{"ListId":17939,"UserName":"zero1997","ForMan":true,"Cover":"https://imgapi.jiaston.com/BookFiles/BookImages/meishigongyingshang.jpg","Title":"美食旅行家，仙界开餐厅","Description":"欢迎光临深夜食堂，客官，里面请……美食大陆，灵厨为尊！","BookCount":13,"CommendImage":"https://image.zsdfm.com/shudan/images/17939.jpg","CollectionCount":4588,"CommendCount":820,"IsCheck":true,"AddTime":"2019/01/15 18:53:08","UpdateTime":"2019/02/18 15:54:20"},{"ListId":30445,"UserName":"shudan666","ForMan":true,"Cover":"https://imgapi.jiaston.com/BookFiles/BookImages/yinyangdailiren.jpg","Title":"游走阴阳两界，今日，地狱归来","Description":"今日，他从地狱中归来，掀起一个灵异的传奇","BookCount":8,"CommendImage":"https://imgapi.xllxdg.com/shudan/images/30445.jpg","CollectionCount":2660,"CommendCount":815,"IsCheck":true,"AddTime":"2019/08/07 15:07:04","UpdateTime":"2019/08/09 19:25:04"},{"ListId":36047,"UserName":"shudan666","ForMan":true,"Cover":"https://imgapi.jiaston.com/BookFiles/BookImages/damingwenkui.jpg","Title":"奇葩主角的上下五千年","Description":"唐尧虞舜夏商周，春秋战国…今天穿越哪个朝代呢？好难选啊！","BookCount":8,"CommendImage":"https://imgapi.jiaston.com/shudan/images/36047.jpg","CollectionCount":2126,"CommendCount":664,"IsCheck":true,"AddTime":"2019/11/03 15:50:17","UpdateTime":"2019/11/03 17:47:28"},{"ListId":24944,"UserName":"shudan666","ForMan":true,"Cover":"xitongdeheikejiwangba.jpg","Title":"带着一扇穿梭门，开启黑科技时代","Description":"这个穿越画风有些不对？","BookCount":9,"CommendImage":"https://imgapi.jiaston.com/shudan/images/24944.jpg","CollectionCount":3142,"CommendCount":663,"IsCheck":true,"AddTime":"2019/06/03 18:52:08","UpdateTime":"2019/06/03 23:34:54"},{"ListId":20904,"UserName":"shudan666","ForMan":true,"Cover":"https://imgapi.jiaston.com/BookFiles/BookImages/fanrenxiuxianzhixianjiepian.jpg","Title":"携金榜穿越，做异界神灵。","Description":"带着一身通天本领强势回归，会治病，会算命，会炼药…","BookCount":12,"CommendImage":"https://image.zsdfm.com/shudan/images/20904.jpg","CollectionCount":2011,"CommendCount":650,"IsCheck":true,"AddTime":"2019/03/13 16:42:29","UpdateTime":"2019/03/14 23:58:28"},{"ListId":27146,"UserName":"15055885588","ForMan":true,"Cover":"https://imgapi.jiaston.com/BookFiles/BookImages/dushuchengsheng.jpg","Title":"疯狂任务系统，喂喂喂，你不要搞事情","Description":"已成功绑定大魔王系统，存活时间还剩三分钟，请尽快补充时间！","BookCount":8,"CommendImage":"https://imgapi.jiaston.com/shudan/images/27146.jpg","CollectionCount":2343,"CommendCount":646,"IsCheck":true,"AddTime":"2019/07/02 16:23:37","UpdateTime":"2019/07/02 19:10:41"},{"ListId":3333,"UserName":"风一样的男人","ForMan":true,"Cover":"http://www.apporapp.cc/BookFiles/BookImages/daomubiji.jpg","Title":"精选最具人气及影响力的悬疑小说","Description":"整理《盗墓笔记》《鬼出灯》《苗疆蛊事》等网络作品，堪称近年来的经典之作，获得百万读者狂热追捧。","BookCount":6,"CommendImage":"https://image.zsdfm.com/shudan/images/3333.jpg","CollectionCount":4241,"CommendCount":637,"IsCheck":true,"AddTime":"2018/03/26 22:43:21","UpdateTime":"2018/06/03 00:44:05"},{"ListId":16900,"UserName":"zero1997","ForMan":true,"Cover":"http://www.apporapp.cc/BookFiles/BookImages/shangmennvxudeyouxianshenghuo.jpg","Title":"我的二次元老婆，各种操作玩翻天！","Description":"老婆重生还变身，这是什么操作？","BookCount":16,"CommendImage":"https://image.zsdfm.com/shudan/images/16900.jpg","CollectionCount":4607,"CommendCount":600,"IsCheck":true,"AddTime":"2018/12/29 14:24:14","UpdateTime":"2018/12/31 19:33:46"}]}

### 小说 我的书单 
GET https://userxs.pigqq.com/UserBookList.aspx?type=personallist HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
Content-Type: application/x-www-form-urlencoded
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Host: userxs.pigqq.com
Connection: Keep-Alive
Accept-Encoding: gzip

{"status":1,"info":"success","data":{"pub":null,"col":null}}

### 小说 创建书单
POST https://userxs.pigqq.com/UserListAction.aspx HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Content-Type: application/x-www-form-urlencoded
Content-Length: 194
Host: userxs.pigqq.com
Connection: Keep-Alive
Accept-Encoding: gzip

listid=&cover=conghongyuekaishi.jpg&jsondata=%5B%7B%22bookid%22%3A%22610529%22%2C%22description%22%3A%22%22%7D%5D&action=booklist&description=back123123123&title=%E7%88%B8%E7%88%B8&isforman=true

{"status":1,"info":"成功添加书单！","data":{"result": "1","listid":91936}}

### 小说 移除书架
POST https://userxs.pigqq.com/BookAction.aspx HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Content-Type: application/x-www-form-urlencoded
Content-Length: 36
Host: userxs.pigqq.com
Connection: Keep-Alive
Accept-Encoding: gzip

bookIds=626698&action=removebookcase

{"status":1,"info":"批量移除书架成功！","data":{"result": "2"}}


### 漫画书单
POST https://usermanhua.pigqq.com/Bookshelf.aspx HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Content-Type: application/x-www-form-urlencoded
Content-Length: 0
Host: usermanhua.pigqq.com
Connection: Keep-Alive
Accept-Encoding: gzip

{"status":1,"info":"success","data":null}

### 漫画banner
GET https://scmanhua.pigqq.com/prov1/base/banner_man.html HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
Content-Type: application/x-www-form-urlencoded
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Host: scmanhua.pigqq.com
Connection: Keep-Alive
Accept-Encoding: gzip

{
    "status": 1,
    "info": "",
    "data": [
        {
            "type": "booklist",
            "param": "84",
            "imgurl": "https://scmanhua.pysmei.com/pubimgs/mhsdimgs/84.jpg"
        },
        {
            "type": "booklist",
            "param": "85",
            "imgurl": "https://scmanhua.pysmei.com/pubimgs/mhsdimgs/85.jpg"
        },
        {
            "type": "booklist",
            "param": "86",
            "imgurl": "https://scmanhua.pysmei.com/pubimgs/mhsdimgs/86.jpg"
        }
    ]
}

### 漫画书城
GET https://scmanhua.pigqq.com/prov1/base/man2.html HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
Content-Type: application/x-www-form-urlencoded
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Host: scmanhua.pigqq.com
Connection: Keep-Alive
Accept-Encoding: gzip

{
  "status": 1,
  "info": "success",
  "data": [
    {
      "Category": "强力推荐",
      "ViewType": "12c",
      "NavIcon": "https://scmanhua.pysmei.com/pubimgs/recommend.png",
      "More": "https://scmanhua.pysmei.com/top/man/top/area/all/commend/total/{page}.html",
      "MoreFlag": "api",
      "ChangeFlag": "no",
      "Books": [{
			"Id": 6157,
			"Name": "我和妹子们的荒岛余生",
			"Author": "青葶动漫",
			"Img": "https://acbqimg.cdn.bcebos.com/BookFiles/BookImage/acac/wohemeizimendehuangdaoyusheng.jpg",
			"HostKey": "acac",
			"Desc": "远古巨兽，现代人类，未来科技，时空混乱的荒岛；石器时代，动力时代，电气时代，飞速发展的荒岛文明。流落无人荒岛，开局一个系统，秦天从零开始求生。校花女神，金发御姐，暴走萝莉，我统统都要；驯金雕，收狼王，退巨蟒，这座荒岛，由我做主！",
			"CName": "其它",
			"Score": "7.0"
		}, {
			"Id": 6122,
			"Name": "斗罗大陆4终极斗罗",
			"Author": "神漫",
			"Img": "https://acbqimg.cdn.bcebos.com/BookFiles/BookImage/acac/douluodalu4zhongjidouluo.jpg",
			"HostKey": "acac",
			"Desc": "【每周二、周六上午10点更新】斗罗联邦科考队在极北之地科考时，发现了一个有着金银双色花纹的蛋。他们探查后发现里面居然有生命迹象，于是赶忙将其带回研究所进行孵化。蛋孵化出来了，可孵出来的是一个婴儿，一个和人类一模一样的孩子；与此同时，联邦研究所正在解冻一名银色长发女子，而一名蓝发青年则在海滨被人发现",
			"CName": "其它",
			"Score": "8.2"
		}, {
			"Id": 5861,
			"Name": "炼气练了三千年",
			"Author": "刺猬猫阅读",
			"Img": "https://kuaikanbqimg.cdn.bcebos.com/BookFiles/BookImage/kan/lianqilianlesanqiannian.jpg",
			"HostKey": "kan",
			"Desc": "《炼气练了三千年》小说改编作品。三千年前，天资绝顶的白秋然被青冥剑宗创始人青冥道人收为门徒，开始修仙之路。三千年后，青冥道人飞升成仙，大师兄渡劫失败身死道消，就连最小的小师妹的六世孙都筑基成功，学会了御剑乘风而行。而经历三千年的苦修，白秋然他，终于达到了炼气期第六万六千六百六十四层",
			"CName": "魔幻",
			"Score": "8.5"
		}, {
			"Id": 4354,
			"Name": "本婿修的是贱道",
			"Author": "博易动漫",
			"Img": "https://acbqimg.cdn.bcebos.com/BookFiles/BookImage/acac/benxuxiudeshijiandao.jpg",
			"HostKey": "acac",
			"Desc": "前世遭受冷艳女帝“强迫双修”百年，切掉一魄只为逃离虎穴！！今涅槃重生成赘婿，这一世我武学魂法齐全，看我在这满是鄙夷的大陆上，一柱擎天定乾坤！每周一，四更新！",
			"CName": "玄幻",
			"Score": "6.0"
		}, {
			"Id": 4013,
			"Name": "大王饶命",
			"Author": "阅动文化",
			"Img": "https://acbqimg.cdn.bcebos.com/BookFiles/BookImage/acac/dawangraoming.jpg",
			"HostKey": "acac",
			"Desc": "《大王饶命》漫画版由漫画团队阅动文化绘制，根据阅文集团旗下起点中文网同名小说改编，原作者：会说话的肘子。灵气复苏，全民抓紧每丝灵气修行。只有吕树背靠负面情绪值系统，怼人就变强！他只想保护妹妹，但时代洪流无可避，那只好……顺便怼怼人，成为最强！准备好了吗，吕树“大魔王”来喽~",
			"CName": "爆笑",
			"Score": "9.0"
		}, {
			"Id": 1561,
			"Name": "元尊",
			"Author": "天蚕土豆",
			"Img": "https://acbqimg.cdn.bcebos.com/BookFiles/BookImage/acac/yuanzun.jpg",
			"HostKey": "acac",
			"Desc": "2017年12月5日上线，每周二、四、六、日更新。此漫画由天蚕土豆热门小说《元尊》改编。少年执笔，龙蛇舞动；劈开乱世，点亮苍穹。气掌乾坤的世界里，究竟是蟒雀吞龙，还是圣龙崛起？！",
			"CName": "玄幻",
			"Score": "9.3"
		}, {
			"Id": 1100,
			"Name": "百炼成神",
			"Author": "燃哉工作室",
			"Img": "https://acbqimg.cdn.bcebos.com/BookFiles/BookImage/acac/bailianchengshen.jpg",
			"HostKey": "acac",
			"Desc": "【每周三、五、六更新】现在身为卑微家奴的罗征，本身家中大少爷，因家族败落，妹妹被强大势力囚禁，无奈只得听命于人。可是天无绝人之路，父亲留给他的古书中竟然暗藏炼器神法，可将人炼制成器！而隐藏在这背后的神秘力量到底是什么？这是一场与命运的较量。",
			"CName": "热血",
			"Score": "8.0"
		}, {
			"Id": 1098,
			"Name": "斗破苍穹",
			"Author": "知音漫客",
			"Img": "https://acbqimg.cdn.bcebos.com/BookFiles/BookImage/acac/doupocangqiong.jpg",
			"HostKey": "acac",
			"Desc": "【每周六周日12点更新】正所谓三十年河东三十年河西，天才少年因忽然失去了天生的灵力，被所有人嘲笑排挤，为了一雪前耻他亲手毁掉婚约，一心进修、打怪、升级！重登人生巅峰的他让人们知道莫欺少年穷真的很重要！",
			"CName": "热血",
			"Score": "9.7"
		}, {
			"Id": 1066,
			"Name": "武炼巅峰",
			"Author": "噼咔噼",
			"Img": "https://acbqimg.cdn.bcebos.com/BookFiles/BookImage/acac/wuliandianfeng.jpg",
			"HostKey": "acac",
			"Desc": "《武炼巅峰》漫画版是由深圳漫画团队噼咔噼绘制，根据阅文集团旗起点中文网的同名小说改编，作者是莫默。武之巅峰，是孤独，是寂寞，是漫漫求索，是高处不胜寒。逆境中成长，绝地里求生，才能堪破武之极道。凌霄阁试炼弟子兼扫地小厮杨开偶获一本无字黑书，从此踏上漫漫武道。",
			"CName": "玄幻",
			"Score": "8.7"
		}, {
			"Id": 1057,
			"Name": "全职法师",
			"Author": "阅文漫画",
			"Img": "https://acbqimg.cdn.bcebos.com/BookFiles/BookImage/acac/quanzhifashi.jpg",
			"HostKey": "acac",
			"Desc": "周三、周五、周六上午10点准时更新！官方1群号：598116890官方2群号：637220919官方3群号：653340196官方4群号：697672941莫凡继承了一个神奇的项链。一觉醒来世界大变。崇尚科学的世界变成了崇尚魔法。不过，莫凡发现大家都只能够主修一系魔法，自己却是全系全能法师！",
			"CName": "热血",
			"Score": "9.0"
		}, {
			"Id": 29,
			"Name": "斗罗大陆",
			"Author": "风炫动漫",
			"Img": "https://kkkbqimg.cdn.bcebos.com/BookFiles/BookImage/kkk/douluodalu.jpg",
			"HostKey": "kkk",
			"Desc": "唐三因偷学绝门派武功，被逼无奈怀揣着一身绝技和未完成的心愿跳崖明志，不料却带着前世记忆转世重生。还是小正太的他凭借天生双武魂先天满魄力的天赋走进了诺丁学院，遇到了野蛮可爱的萝莉小舞，同时也发现了自己的身世之谜。前世心愿今生能实现吗？",
			"CName": "热血",
			"Score": "6.9"
		}]
    },
    {
      "Category": "新番出炉",
      "ViewType": "3c3c",
      "NavIcon": "https://scmanhua.pysmei.com/pubimgs/recommend.png",
      "More": "https://scmanhua.pysmei.com/top/man/top/area/all/new/total/{page}.html",
      "MoreFlag": "api",
      "ChangeFlag": "no",
      "Books": [{
			"Id": 8130,
			"Name": "凡人修仙之仙界篇",
			"Author": "忘语,囧标,蛋糕月",
			"Img": "https://rmbqimg.cdn.bcebos.com/BookFiles/BookImage/rm/384.jpg",
			"HostKey": "rm",
			"Desc": "《凡人修仙传》故事开始的万年之后，在灵寰界，狐女柳乐儿的族亲被血刀会灭门，自己也被追杀。伤痕累累的柳乐儿躲到了一块大石头下，正当追杀的三位修仙者要对其下毒手之时，石头突然炸裂开来，里面出现了一个相貌平平的男子……《凡人修仙之仙界篇》是一部类型为玄幻|古风|冒险的高人气国漫漫画,凡人修仙之仙界篇漫画免费完整版由网友上传完整版免费阅读,同时还提供了凡人修仙之仙界篇漫画作者,地区,连载状态等相关信息!",
			"CName": "玄幻",
			"Score": "6.0"
		}, {
			"Id": 8116,
			"Name": "仙王的日常生活",
			"Author": "娱乐没错",
			"Img": "https://rmbqimg.cdn.bcebos.com/BookFiles/BookImage/rm/379.jpg",
			"HostKey": "rm",
			"Desc": "枯玄著同名小说改编!!这是一个全民修仙的时代！御剑飞行，修仙成圣，人人都在为之而努力！而王令却是一个反例！仙术？修炼？丹药？他毫不在意，但修为却如同外挂般飞速升级。3岁御剑，7岁化神，本想低调佛性过一生的他却栽倒在了一所普通高中！一不小心成为万众瞩目真的很让人心累……唉……无敌是多么的寂寞，且让我和我的干脆面虚度一生，强者的生活就是这么枯燥……且无聊……并且……状况百出--|||《仙王的日常生活》",
			"CName": "恶搞",
			"Score": "6.0"
		}, {
			"Id": 8050,
			"Name": "我独自满级重生",
			"Author": "Honey,VERTWO,Anaziro,graycompany",
			"Img": "https://rmbqimg.cdn.bcebos.com/BookFiles/BookImage/rm/283.jpg",
			"HostKey": "rm",
			"Desc": "全世界超过一亿的人消失了！而现实世界中却出现了无数“奇怪生命体”在摧毁地球，人类危在旦夕。此时，一群能够制服怪兽的人挺身而出，他们正是当时消失在网络游戏“永恒世界”中的玩家。而作为22年来首次通关完成最难生存游戏的最强者，陈瑞也终于带着谁都无法成功获得的奖赏回归了…他会在这个游戏般的现实世界中遇到什么呢？《我独自满级重生》是一部类型为热血|冒险|奇幻的高人气国漫漫画,我独自满级重生漫画免费完整版由",
			"CName": "热血",
			"Score": "6.0"
		}, {
			"Id": 6628,
			"Name": "仙尊洛无极",
			"Author": "大魔王漫画",
			"Img": "https://acbqimg.cdn.bcebos.com/BookFiles/BookImage/acac/2855.jpg",
			"HostKey": "acac",
			"Desc": "弟子、兄弟接连背叛，一代仙尊就此陨落。虽肉身已死，然精魂不灭！且凭至宝“太皇经”扭转因果，重回地球，破除业障，再铸神格！此生必使“无极”之名，凌驾天地日月之上！",
			"CName": "其它",
			"Score": "6.0"
		}, {
			"Id": 5625,
			"Name": "魔道祖师",
			"Author": "墨香铜臭",
			"Img": "https://kuaikanbqimg.cdn.bcebos.com/BookFiles/BookImage/kan/modaozushi.jpg",
			"HostKey": "kan",
			"Desc": "改编自墨香铜臭原创同名小说，前世掀起腥风血雨的一代魔道祖师，竟重生成一个脑残！此生的魏无羡与故人一同祛除邪魔匡扶正义，不知这一次是否能迎来圆满结局？【独家/每周一更新责编：林早上】",
			"CName": "魔幻",
			"Score": "9.2"
		}, {
			"Id": 4538,
			"Name": "修仙者大战超能力",
			"Author": "一号奶粉",
			"Img": "https://kkkbqimg.cdn.bcebos.com/BookFiles/BookImage/kkk/xiuxianzhedazhanchaonengli.jpg",
			"HostKey": "kkk",
			"Desc": "修仙大陆有一位大能者，意外穿越到了现代英雄社会，在这渺小的地球中仙法和超能力了激烈的对抗……",
			"CName": "热血",
			"Score": "9.2"
		}]
    },
    {
      "Category": "精彩连载",
      "ViewType": "1r3c3c",
      "NavIcon": "https://scmanhua.pysmei.com/pubimgs/recommend.png",
      "More": "https://scmanhua.pysmei.com/top/man/top/area/all/hot/total/{page}.html",
      "MoreFlag": "api",
      "ChangeFlag": "no",
      "Books": [{
			"Id": 7718,
			"Name": "开局就有王者账号",
			"Author": "仁山动漫",
			"Img": "https://acbqimg.cdn.bcebos.com/BookFiles/BookImage/acac/2872.jpg",
			"HostKey": "acac",
			"Desc": "突如其来的危机让地球直接进入OL时代，全人类沦为未知势力的掌中之物，所有人都变成了一级的小号，在弱肉强食的残酷时代，高中生叶昊却始终只能升到三级，濒死之际，意外开启王者账号升级系统，叶昊能成为那个最强王者吗？",
			"CName": "其它",
			"Score": "6.0"
		}, {
			"Id": 6534,
			"Name": "我的弟子都超神",
			"Author": "口袋宇宙 x 时光鱼文化",
			"Img": "https://acbqimg.cdn.bcebos.com/BookFiles/BookImage/acac/2796.jpg",
			"HostKey": "acac",
			"Desc": "游戏公司的加班狗叶阳，带着‘全职业满技能’的帐号穿越了！满级剑圣+修仙者+魔法师的咸鱼宗主生活开启，头痛的是有一群美女弟子天天劝他上进…",
			"CName": "其它",
			"Score": "8.8"
		}, {
			"Id": 5670,
			"Name": "魔皇大管家",
			"Author": "夜枭",
			"Img": "https://kuaikanbqimg.cdn.bcebos.com/BookFiles/BookImage/kan/mohuangdaguanjia.jpg",
			"HostKey": "kan",
			"Desc": "魔皇卓一凡因得到上古魔帝传承，遭亲信背叛并引来杀身之祸。重生后修为归零的他又被心魔所困，不得不成为一个落寞家族大小姐的专属管家。从魔皇到小小管家，他究竟要怎样和自己的“心魔大小姐”相处，又如何才能带领这个没落家族和自己一起重回这片大陆的巅峰呢！【每周二/周六更新责编：金小明】",
			"CName": "魔幻",
			"Score": "9.6"
		}, {
			"Id": 4356,
			"Name": "我有九个女徒弟",
			"Author": "博易动漫",
			"Img": "https://acbqimg.cdn.bcebos.com/BookFiles/BookImage/acac/woyoujiugenvtudi.jpg",
			"HostKey": "acac",
			"Desc": "敢在老祖头上动土？打脸打不死你！女人？我有九个！！上天入地，岂有对手？就是这么狂！每周三，六更新！",
			"CName": "玄幻",
			"Score": "8.0"
		}, {
			"Id": 4212,
			"Name": "龙王殿",
			"Author": "本命漫画",
			"Img": "https://acbqimg.cdn.bcebos.com/BookFiles/BookImage/acac/longwangdian.jpg",
			"HostKey": "acac",
			"Desc": "作品名称《龙王殿》，改编自逐浪网小说。林清涵爷爷危在旦夕，一干亲戚却为了争夺家产，不顾林氏集团的安稳，用尽各种卑劣的手段，却陷害女总裁林清涵，然而，却被有“撒旦”之称的龙王殿之主，女婿张玄，给一一化解。",
			"CName": "热血",
			"Score": "4.8"
		}, {
			"Id": 3540,
			"Name": "英雄再临（英雄？我早就不当了）",
			"Author": "SF轻小说",
			"Img": "https://acbqimg.cdn.bcebos.com/BookFiles/BookImage/acac/yingxiongzailin（yingxiong？wozaojiubudangle）.jpg",
			"HostKey": "acac",
			"Desc": "“零”是人类第一个真正意义上的超级英雄。在他的带动下，不断涌现出了大量的超级英雄。但是他在持续战斗了五年之后，却消失在了人们的视线之中。【授权/每周二更新】",
			"CName": "爆笑",
			"Score": "8.8"
		}, {
			"Id": 153,
			"Name": "从今天开始当城主",
			"Author": "青葶动漫",
			"Img": "https://kkkbqimg.cdn.bcebos.com/BookFiles/BookImage/kkk/congjintiankaishidangchengzhu.jpg",
			"HostKey": "kkk",
			"Desc": "当游戏宅男启穿越Buff，当然是选择搞事！搞事！搞事！御姐猫耳娘，萝莉狐耳娘，软妹兔耳娘……这不是动物园！这是一个弱肉强食却又奇妙的异世界！一场真实的策略性游戏，一个巨大的阴谋危机，异界霸主正在加载，尔等都是渣渣……",
			"CName": "热血",
			"Score": "9.2"
		}]
    },
    {
      "Category": "完结畅读",
      "ViewType": "3c3c",
      "NavIcon": "https://scmanhua.pysmei.com/pubimgs/recommend.png",
      "More": "https://scmanhua.pysmei.com/top/man/top/area/all/over/total/{page}.html",
      "MoreFlag": "api",
      "ChangeFlag": "no",
      "Books": [{
			"Id": 6498,
			"Name": "尸兄（我叫白小飞）",
			"Author": "七度魚",
			"Img": "https://acbqimg.cdn.bcebos.com/BookFiles/BookImage/acac/shixiong（wojiaobaixiaofei）.jpg",
			"HostKey": "acac",
			"Desc": "即将毁灭的世界......每周更新...",
			"CName": "恐怖",
			"Score": "8.7"
		}, {
			"Id": 4300,
			"Name": "死神/境·界",
			"Author": "久保带人",
			"Img": "https://acbqimg.cdn.bcebos.com/BookFiles/BookImage/acac/sishen/jing·jie.jpg",
			"HostKey": "acac",
			"Desc": "作品连载于周刊杂志《周刊少年JUMP》，与日本同步更新，每周周一更新。有特殊能力的日本某高中生黑崎一护，在街头邂逅了一个奉命来执行任务的神界少女，任务是处理某种邪恶怪物“虚”！为了维护人类和神界的和平，一护、露琪亚和伙伴们开始了漫漫征程。",
			"CName": "动作",
			"Score": "9.0"
		}, {
			"Id": 2804,
			"Name": "火影忍者",
			"Author": "岸本齐史",
			"Img": "https://kkkbqimg.cdn.bcebos.com/BookFiles/BookImage/kkk/huoyingrenzhe.jpg",
			"HostKey": "kkk",
			"Desc": "从小身上封印着邪恶的九尾妖狐，无父无母的鸣人受尽了村人的冷落，但是他却不知道原因，只是拼命用各种恶作剧试图吸引大家的注意力，人们却反而更远离他。好在还是有依卡鲁老师关心他，鸣人的性格才没有变得扭曲，他总是干劲十足，嘻嘻哈哈，超级乐观。为了让更多的人认可自己，鸣人的目标是——成为第五代火影！这可是很高[]高的目标哦，火影是世上最强的五位忍者之一的封号，也是木叶忍者村的首领。鸣人可不管，对于自己终有一",
			"CName": "热血",
			"Score": "7.4"
		}, {
			"Id": 2707,
			"Name": "鬼灭之刃",
			"Author": "吾峠呼世晴",
			"Img": "https://rmbqimg.cdn.bcebos.com/BookFiles/BookImage/rm/guimiezhiren.jpg",
			"HostKey": "rm",
			"Desc": "鬼灭之刃漫画简介：鬼灭之刃漫画，时值日本大正时期。传说太阳下山后，恶鬼出没吃人。亦有猎鬼人斩杀恶鬼、保护人们。卖炭少年·炭治郎，他那平凡而幸福的日常生活，在家人遭到恶鬼袭击的那一天发生剧变。母亲与四个弟妹惨遭杀害，而与他一起生还的妹妹：祢豆子亦异变成凶暴的鬼。在猎鬼人的指引下，立志成为猎鬼人的炭治郎与变成鬼却尚存理智的祢豆子二人踏上了旅程。通过艰苦的剑术修行与赌命试炼，炭治郎成为了鬼猎人组织“鬼杀",
			"CName": "冒险",
			"Score": "9.7"
		}, {
			"Id": 1583,
			"Name": "偷星九月天",
			"Author": "周洪滨 小松",
			"Img": "https://acbqimg.cdn.bcebos.com/BookFiles/BookImage/acac/touxingjiuyuetian.jpg",
			"HostKey": "acac",
			"Desc": "一场爱与梦冒险，是男仆还是热血侦探？是江洋大盗还是美女“主人”？从琉星的VV学院的奇特异能，到九月的黑月铁骑们魅影闪现，迷雾一层层的被解开……【授权/已完结】",
			"CName": "热血",
			"Score": "9.8"
		}, {
			"Id": 1056,
			"Name": "重生大玩家",
			"Author": "知音漫客",
			"Img": "https://acbqimg.cdn.bcebos.com/BookFiles/BookImage/acac/zhongshengdawanjia.jpg",
			"HostKey": "acac",
			"Desc": "游戏重生竟成最强外挂！男主万葭在“大玩家”游戏中惨遭队友暗算，失去比赛资格，却在退出游戏的一瞬间，穿越回了一年前，“大玩家”比赛刚刚开始的那一天。为了惩戒背后阴自己的小人，更为了获胜！已经对马上来临的比赛内容了如指掌的万葭，即将开启这一场王者归来的表演。",
			"CName": "冒险",
			"Score": "9.4"
		}]
    },
    {
      "Category": "万人追更",
      "ViewType": "3c3c",
      "NavIcon": "https://scmanhua.pysmei.com/pubimgs/recommend.png",
      "More": "https://scmanhua.pysmei.com/top/man/top/area/all/hot/month/{page}.html",
      "MoreFlag": "api",
      "ChangeFlag": "no",
      "Books":  [{
			"Id": 8286,
			"Name": "我有一座冒险屋",
			"Author": "极漫文化",
			"Img": "https://rmbqimg.cdn.bcebos.com/BookFiles/BookImage/rm/612.jpg",
			"HostKey": "rm",
			"Desc": "陈歌继承了失踪父母留下的鬼屋，无奈生意萧条，直到整理鬼屋时意外发现的手机改变了这一切。只要完成手机每日布置的不同难度的任务，鬼屋就能得到修缮甚至扩建。于是陈歌开始在各大禁地里探险取材，将其中场景元素纳入到自己的鬼屋中。随着前来参观的游客们各种惊声尖叫，鬼屋一举成名！然而虽然任务带来的好处越来越多，但其中隐患也慢慢显现，甚至父母失踪的线索似乎也藏其中……展开",
			"CName": "冒险",
			"Score": "6.0"
		}, {
			"Id": 8233,
			"Name": "神印王座",
			"Author": "快乐工场",
			"Img": "https://rmbqimg.cdn.bcebos.com/BookFiles/BookImage/rm/517.jpg",
			"HostKey": "rm",
			"Desc": "魔族强势，在人类即将被灭绝之时，六大圣殿崛起，带领着人类守住最后的领土。一名少年，为救母加入骑士圣殿，奇迹、诡计，不断在他身上上演。在这人类6大圣殿与魔族72柱魔神相互倾轧的世界，他能否登上象征着骑士最高荣耀的神印王座？《神印王座》是一部类型为热血|玄幻|动作的高人气国漫漫画,神印王座漫画免费完整版由网友上传完整版免费阅读,同时还提供了神印王座漫画作者,地区,连载状态等相关信息!",
			"CName": "热血",
			"Score": "6.0"
		}, {
			"Id": 8131,
			"Name": "凡人修仙传",
			"Author": "HeHeX蛋糕月",
			"Img": "https://rmbqimg.cdn.bcebos.com/BookFiles/BookImage/rm/383.jpg",
			"HostKey": "rm",
			"Desc": "山村少年韩立出生贫苦。为了补贴家用，加入江湖门派七玄门。因身具灵根，被门派内神秘的墨大夫收为弟子，修炼《长春功》。虽然资质平庸，但韩立凭着不屈的意志，和一个偶然捡到的神秘小瓶，踏上了凶险的修仙之路……《凡人修仙传》是一部类型为热血|玄幻|古风|冒险的高人气国漫漫画,凡人修仙传漫画免费完整版由网友上传完整版免费阅读,同时还提供了凡人修仙传漫画作者,地区,连载状态等相关信息!",
			"CName": "热血",
			"Score": "6.0"
		}, {
			"Id": 6325,
			"Name": "九星霸体诀",
			"Author": "遁入空门",
			"Img": "https://acbqimg.cdn.bcebos.com/BookFiles/BookImage/acac/2659.jpg",
			"HostKey": "acac",
			"Desc": "是丹帝重生？是融合灵魂？被盗走灵根、灵血、灵骨的三无少年——龙尘，凭借着记忆中的炼丹神术，修行神秘功法九星霸体诀，拨开重重迷雾，解开惊天之局。手掌天地乾坤，脚踏日月星辰，勾搭各色美女，镇压恶鬼邪神。",
			"CName": "其它",
			"Score": "8.0"
		}, {
			"Id": 1096,
			"Name": "传武",
			"Author": "GK工坊",
			"Img": "https://acbqimg.cdn.bcebos.com/BookFiles/BookImage/acac/chuanwu.jpg",
			"HostKey": "acac",
			"Desc": "他说：“这世上本不该有鬼”。然后，这世间为之一清。",
			"CName": "古风",
			"Score": "9.7"
		}, {
			"Id": 1038,
			"Name": "放开那个女巫",
			"Author": "阅文漫画",
			"Img": "https://acbqimg.cdn.bcebos.com/BookFiles/BookImage/acac/fangkaineigenvwu.jpg",
			"HostKey": "acac",
			"Desc": "工科男穿越异世界，成为一位王子。这里酷似欧洲中世纪，但又似乎不太一样？女巫真实存在，而且还真有魔力！魔力就是生产力！拯救女巫，解放生产力！开地图，斗邪魔，破阴谋，爬升科技树，开启硬核“种田”之路！",
			"CName": "热血",
			"Score": "9.0"
		}]
    },
    {
      "Category": "最多收藏",
      "ViewType": "3c3c",
      "NavIcon": "https://scmanhua.pysmei.com/pubimgs/recommend.png",
      "More": "https://scmanhua.pysmei.com/top/man/top/area/all/collect/total/{page}.html",
      "MoreFlag": "api",
      "ChangeFlag": "no",
      "Books": [{
			"Id": 8035,
			"Name": "元龙",
			"Author": "任怨,闻源文化",
			"Img": "https://rmbqimg.cdn.bcebos.com/BookFiles/BookImage/rm/274.jpg",
			"HostKey": "rm",
			"Desc": "特种兵王胜穿越到了元魂世界，被废物鲤鱼元魂附身，成为了元魂世界名副其实的废人。王胜在高手如云的元魂世界里用学来的知识过关斩将，甚至找到了废物鲤鱼元魂进化的方法！麻雀变凤凰，鲤鱼跃龙门。王胜从险恶的元魂纷争中走出了一条成龙之路！《元龙》是一部类型为热血|玄幻|冒险的高人气国漫漫画,元龙漫画免费完整版由网友上传完整版免费阅读,同时还提供了元龙漫画作者,地区,连载状态等相关信息!",
			"CName": "热血",
			"Score": "6.0"
		}, {
			"Id": 4353,
			"Name": "回到地球当神棍",
			"Author": "本命漫画",
			"Img": "https://acbqimg.cdn.bcebos.com/BookFiles/BookImage/acac/huidaodiqiudangshengun.jpg",
			"HostKey": "acac",
			"Desc": "他，曾经失踪八年。可没有人想到，他是穿越到了异界，并且修炼了八千年！回到地球后，他寻找妹妹，可没有人想到，他在找妹妹的过程中，同时干翻了地球上的所有大势力！他拐跑豪门千金。可没有人想到，他在拐跑千金的同时，顺便灭了人家的未婚夫。他能炼丹，会打架，若是有人惹了他……将会万劫不复！",
			"CName": "玄幻",
			"Score": "6.0"
		}, {
			"Id": 4036,
			"Name": "我捡起了一地属性",
			"Author": "刺猬猫阅读",
			"Img": "https://acbqimg.cdn.bcebos.com/BookFiles/BookImage/acac/wojianqileyidishuxing.jpg",
			"HostKey": "acac",
			"Desc": "游戏肝帝风夏穿越到末法时代的修真世界，凭借属性异能和在游戏中培养出来的战略手段一路打爆敌人，获得敌人的属性及技能，扭转乾坤！还有各路兽娘美少女……通通要往碗里来！敌人得意：“我的盖世神功天下无敌！”风夏一拳将其打爆！在敌人面前捏碎属性光团：“多谢，现在它是我的盖世神功了！”",
			"CName": "玄幻",
			"Score": "6.8"
		}, {
			"Id": 1257,
			"Name": "我身上有条龙",
			"Author": "岛上Project",
			"Img": "https://acbqimg.cdn.bcebos.com/BookFiles/BookImage/acac/woshenshangyoutiaolong.jpg",
			"HostKey": "acac",
			"Desc": "一代天界帝师，重回高中时代，他却惊讶地发现他身上多了一条龙……当你还很弱小时，面对欺压，你是会拼命反抗还是顺从？上一世，他顺从了，但这一世……风流帝师纵横都市，覆手翻云，心中执念只有一个：我为王者，何居人下？！周二、周四、周六更新",
			"CName": "热血",
			"Score": "6.9"
		}, {
			"Id": 536,
			"Name": "失业魔王",
			"Author": "SF轻小说/汤力水",
			"Img": "https://kkkbqimg.cdn.bcebos.com/BookFiles/BookImage/kkk/shiyemowang.jpg",
			"HostKey": "kkk",
			"Desc": "他是因为被弹劾而失业的魔界之王，她是因为征伐失败下岗的人界勇者，命运的纽带将二人绑定在一起，始一起踏上充满未知的冒险&还债之旅。",
			"CName": "恋爱",
			"Score": "8.0"
		}, {
			"Id": 69,
			"Name": "驭灵师",
			"Author": "时代漫王",
			"Img": "https://kkkbqimg.cdn.bcebos.com/BookFiles/BookImage/kkk/yulingshi.jpg",
			"HostKey": "kkk",
			"Desc": "“我被丢到自己的漫画里啦！”“我变强了，但也秃了。”“那个把我扔进这个世界的SB，你对力量一无所知！”“等等！光头太丑了！我才不要做埼玉老师！”“不过我怎么就成了配角呢？旁边那个家伙的主角光环真是耀眼啊！”“果然还是要一头帅气的长发才符合我大BOSS的身份！”这是一个漫画家降临自己笔下世界的冒险故事",
			"CName": "热血",
			"Score": "8.4"
		}]
    },
    {
      "Category": "高分日漫",
      "ViewType": "3c3c",
      "NavIcon": "https://scmanhua.pysmei.com/pubimgs/recommend.png",
      "More": "https://scmanhua.pysmei.com/top/man/top/area/all/vote/total/{page}.html",
      "MoreFlag": "api",
      "ChangeFlag": "no",
      "Books": [{
			"Id": 7733,
			"Name": "咒术回战",
			"Author": "芥见下々",
			"Img": "https://kkkbqimg.cdn.bcebos.com/BookFiles/BookImage/kkk/2937.jpg",
			"HostKey": "kkk",
			"Desc": "漫画《咒术回战》是由新锐漫画家芥见下下所作的少年漫画作品，讲述的是拥有超人般身体能力的男子高中生虎杖悠仁的黑暗幻想故事。因为某种理由，想要每天17点之前回家的虎杖悠仁来到了不强制出席的灵异现象研究会，享受着悠闲的活动。这样的某一天，来学校寻找被封印的诅咒之物的青年伏黒恵出现在了虎杖的面前……",
			"CName": "热血",
			"Score": "8.0"
		}, {
			"Id": 2782,
			"Name": "进击的巨人",
			"Author": "谏山创",
			"Img": "https://rmbqimg.cdn.bcebos.com/BookFiles/BookImage/rm/jinjidejuren.jpg",
			"HostKey": "rm",
			"Desc": "进击的巨人漫画简介：进击的巨人漫画。这部作品是日本漫画家谏山创所著。107年前（743年），世界上突然出现了人类的天敌“巨人”。面临着生存危机而残存下来的人类逃到了一个地方，盖起了三重巨大的城墙。人们在这隔绝的环境里享受了一百多年的和平，直到艾伦·耶格尔十二岁那年，60米高的“超大型巨人”突然出现，以压倒性的力量破坏城门，其后瞬间消失，巨人们成群的冲进墙内捕食人类。艾伦亲眼看着人们以及自己的母亲被",
			"CName": "热血",
			"Score": "9.7"
		}, {
			"Id": 2724,
			"Name": "无职转生",
			"Author": "フジカワユカ,理不尽な孫の手",
			"Img": "https://rmbqimg.cdn.bcebos.com/BookFiles/BookImage/rm/wuzhizhuansheng.jpg",
			"HostKey": "rm",
			"Desc": "34岁无职童贞尼特身无分文地被赶出家门，发现自己的人生已经完全走投无路。刚刚产生后悔的想法，他就被卡车撞死了。然后醒来的地方居然是——剑与魔法的异世界！！重生为名叫卢迪乌斯的婴儿的他下定决心，“这次一定要认真地活下去……！”，一定要度过一段不会后悔的人生。他利用前世的智力很快使得自己的魔术的才能开花结果，结果一位年轻的女孩子成了自己的家庭教师。并且又与一位有着绿宝石般美丽秀发的四分一血统的精灵相遇",
			"CName": "冒险",
			"Score": "8.8"
		}, {
			"Id": 2710,
			"Name": "一拳超人",
			"Author": "村田雄介",
			"Img": "https://rmbqimg.cdn.bcebos.com/BookFiles/BookImage/rm/yiquanchaoren.jpg",
			"HostKey": "rm",
			"Desc": "飘荡在战栗旋风中让飞雪似的落花，伟大的姐妹组合初登场！这个世界的英雄指的是…为了消灭给人类带来危害的生物或怪人！我曾经想成为英雄，我想拯救时间奈何能力有限！由本站收集自互联网本站，让你爱上漫画！",
			"CName": "热血",
			"Score": "9.5"
		}, {
			"Id": 2709,
			"Name": "龙珠超",
			"Author": "鸟山明 とよたろう",
			"Img": "https://rmbqimg.cdn.bcebos.com/BookFiles/BookImage/rm/longzhuchao.jpg",
			"HostKey": "rm",
			"Desc": "龙珠超漫画，新系列作的舞台为悟空与魔人布欧的壮绝战斗结束后，地球重新恢复和平之后发生的故事。与自漫长沉睡中觉醒的破坏神比鲁斯的相遇，加上曾经被人敬畏为“宇宙帝王”的弗利萨的复活，在此之上更有神秘的人物登场……",
			"CName": "热血",
			"Score": "8.0"
		}, {
			"Id": 2705,
			"Name": "海贼王",
			"Author": "尾田荣一郎",
			"Img": "https://rmbqimg.cdn.bcebos.com/BookFiles/BookImage/rm/haizeiwang.jpg",
			"HostKey": "rm",
			"Desc": "“我是要成为海贼王的男人!!!”蒙其.D.路飞神秘的恶魔果实给予了名为蒙其.D.路飞的男孩变橡胶人的能力却也让他再也不能游泳，然而这并没有动摇他的志向，为了传说中的大秘宝“ONEPIECE”，男主角草帽蒙其D路飞踏上了凶险无比同时也波澜壮阔“伟大航道”，一路上他先后结识了一位又一位可靠的伙伴，打倒了一个又一个强大的敌人，经历一次又一次殊死的恶斗，路飞也离传说中的“ONEPIECE”越来越近了……",
			"CName": "冒险",
			"Score": "9.4"
		}]
    },
    {
      "Category": "高分国漫",
      "ViewType": "3c3c",
      "NavIcon": "https://scmanhua.pysmei.com/pubimgs/recommend.png",
      "More": "https://scmanhua.pysmei.com/top/man/top/area/all/vote/week/{page}.html",
      "MoreFlag": "api",
      "ChangeFlag": "no",
      "Books": [{
			"Id": 8234,
			"Name": "仙武帝尊",
			"Author": "二次元动漫",
			"Img": "https://rmbqimg.cdn.bcebos.com/BookFiles/BookImage/rm/516.jpg",
			"HostKey": "rm",
			"Desc": "【独家/每周二、四、六、七更新】九千年前，仙武帝尊率领百万神将打入太古洪荒，却无一人归来，只有一缕真火遗留世间。 九千年后，门派废徒叶辰，被赶出宗门，无以为家，机缘巧合之下偶得真火，再踏仙武之路。 这是一个神魔仙佛并立的世界，这是一个诸天万域混乱的年代，叶辰的逆天征途，由此开始。《仙武帝尊》是一部类型为热血|玄幻|修真的高人气国漫漫画,仙武帝尊漫画免费完整版由网友上传完整版免费阅读,同时还提供了仙",
			"CName": "热血",
			"Score": "6.0"
		}, {
			"Id": 7956,
			"Name": "我独自盗墓",
			"Author": "图:3B2S/文:Yuns,L SEVEN·3号楼",
			"Img": "https://rmbqimg.cdn.bcebos.com/BookFiles/BookImage/rm/135.jpg",
			"HostKey": "rm",
			"Desc": "2025年世界各处惊现古墓，获得墓中“宝物”之人便能获得先人的异能。全世界为获得宝物而疯狂。无往不利盗墓者徐浩钧，在一次任务中落入陷阱，不幸丧命。然而他带着前世的记忆，回到了一切开始的地方。虽然失去了宝物，却获得了“系统”。这是重启的新生，还是命运的捉弄。在系统加持下，这一世徐浩钧能否告别蝼蚁的人生，登上王之宝座？《我独自盗墓》是一部类型为热血|冒险|奇幻的高人气国漫漫画,我独自盗墓漫画免费完整版",
			"CName": "热血",
			"Score": "6.0"
		}, {
			"Id": 6155,
			"Name": "全职高手",
			"Author": "阅文漫画",
			"Img": "https://acbqimg.cdn.bcebos.com/BookFiles/BookImage/acac/quanzhigaoshou.jpg",
			"HostKey": "acac",
			"Desc": "网游荣耀中被誉为教科书级别的顶尖高手，因为种种原因遭到俱乐部的驱逐，离开职业圈的他寄身于一家网吧成了一个小小的网管，但是，拥有十年游戏经验的他，在荣耀新开的第十区重新投入了游戏，带着对往昔的回忆，和一把未完成的自制武器，开始了重返巅峰之路。",
			"CName": "其它",
			"Score": "8.0"
		}, {
			"Id": 4557,
			"Name": "血姬与骑士",
			"Author": "SF轻小说/合火人工作室",
			"Img": "https://acbqimg.cdn.bcebos.com/BookFiles/BookImage/acac/xuejiyuqishi.jpg",
			"HostKey": "acac",
			"Desc": "身为圣骑士的我在一次与吸血种的遭遇战中失利被俘。“啊啦，让你死？想得美，接受我的初拥吧，以后，请多多指教哦~亲爱的女儿。”银发萝莉的血族女王轻挑起了我的下巴，戏谑的笑了笑，尖利的獠牙对准了我的脖子【每周三周六更新】",
			"CName": "其它",
			"Score": "6.0"
		}, {
			"Id": 4247,
			"Name": "领主什么的无所谓啦",
			"Author": "SF轻小说",
			"Img": "https://acbqimg.cdn.bcebos.com/BookFiles/BookImage/acac/lingzhushenmedewusuoweila.jpg",
			"HostKey": "acac",
			"Desc": "震惊！史上最摸鱼的领主利德，竟为了招募部下做出如此伤天害理之事！无口金发女骑士、魔族混血魔法师、性别不明的内政幕僚……他统统来者不拒。",
			"CName": "冒险",
			"Score": "7.6"
		}, {
			"Id": 4035,
			"Name": "无限使徒与十二战姬",
			"Author": "SF轻小说",
			"Img": "https://acbqimg.cdn.bcebos.com/BookFiles/BookImage/acac/wuxianshituyushierzhanji.jpg",
			"HostKey": "acac",
			"Desc": "他是公认最强的存在，伫立于世界顶尖。财富？名声？势力？在他眼里不值一提。最强使徒出逃，惊现人类大陆，原因竟是——“不要误会！老子是来找未来老婆的！”没错，这是一个关于史上最强单身狗找老婆的故事。【授权/每周四更新】",
			"CName": "冒险",
			"Score": "9.5"
		}]
    }
  ]
}

### 漫画书单详情
GET https://scmanhua.pigqq.com/shudan/detail/84.html HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
Content-Type: application/x-www-form-urlencoded
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Host: scmanhua.pigqq.com
Connection: Keep-Alive
Accept-Encoding: gzip

{"status":1,"info":"success","data":{"ListId":84,"UserName":"shudan666","Cover":"https://kkkbqimg.cdn.bcebos.com/BookFiles/BookImage/kkk/jueshiwushen.jpg","IsCheck":true,"IsRecycle":false,"Title":"武道，决定命运，决定生死","ForMan":true,"Description":"弱者受人欺凌，强者俯瞰天下","AddTime":"2020/02/13 20:12:25","UpdateTime":"2020/02/13 22:55:46","BookList":[{"Id":1125,"BookId":132,"BookName":"{{{}}}k061mpe8hvnImbXomdsFjg==","BookImage":"https://kkkbqimg.cdn.bcebos.com/BookFiles/BookImage/kkk/jueshiwushen.jpg","Author":"{{{}}}Sf7Gx7QMaToESyI84qYEciKJTYXZEpENsOLEaN8Yt8E=","CategoryName":"{{{}}}+a6U/XdOsUE=","Score":8.0,"Description":"{{{}}}S4KUTa0IMEHS0qXE++7uTFituT3hnrFDGtDko+NNfOv7SombZGbJusP7GdCGsTHrYCHR0gRzx/d06b52svWXUGqBM4suxOsPRHBM/atO/puLKGwYQB1145fYM8SRAUdzPxixLPzkZ+ZkjJWoxCXEQalduG77RbiQYYUHSMehBbG2IQUiiMF6Ou3IOB7mNJoc+nGHdPQtL+jt23+1UEWG6IuMSaucgB2//JrAn5+JQp18z+NwznBaqFsYkMOkbL0IBZRb6Sla73mGamWBL+fb1LUROmxpjZbSz1mrUJh+1o5IL8MyhisGuOkgN7PFg9OheDMtZi1bbn59wKSCG2l/s5LIdWDXL8k1kaA8vRCrcOA8VVs01IyRUAkdQdXoNdCqvnUVqcT19+VTP8blPwoylDxfSOcNEnr/pwQbDqdI8gE2VHZNHdnVK6bBaeIq41TCL7vQZ4zdLRgs3ejamWvZe9RkqWOOPeScT4DKlHQVSJ0C2Xma/iTYLu4NSAh0LZ0fWYiNorO9UNIxG7z1NhfZkw+1hOq+XiOerTmuRTC3QckCOVjE4JrO1u8SH/RPB8+cmFBaiUFkPlDVZ0JISsoqxE6J0by4EU9aOo8XQOy349KntVaY9wKaI+CoLQEZH8j/B+2vNmXM/v+FPNRY4Dnx6KgumtrfgdbxHOQhM66OkRq/bHPHDzb5Vlex7FHaec8taZxDlSHMDBueD8Wce9hR8l8YaTm+r4ZUC7JBIkWHGKg=","HostKey":"kkk"},{"Id":1126,"BookId":29,"BookName":"{{{}}}Nwyn9nz+162S28ZVakmI/g==","BookImage":"https://kkkbqimg.cdn.bcebos.com/BookFiles/BookImage/kkk/douluodalu.jpg","Author":"{{{}}}NuwAT1G8i/rJzGJCYs9+Bg==","CategoryName":"{{{}}}+a6U/XdOsUE=","Score":6.7,"Description":"{{{}}}pkoIyLu/FeBRoMYUYVdvePrafaZxMzUQTAgRLaY2uFny7Wr1Foqashk1BIvMJaG3fkfjPbnHGVVTR5BhodMWo+baNgNhiEL2dgxOpNy0xmEfGgwheDp3Qngpa1Rdv3Isf1QA+D6hbuoqjjAteDsqHtI7lfaHOBw7MhJ5W5o3oI3JqkBrbdP/qFFMVBfudVlZgXxAe1nJjyIUICXmAHClSJFgBRC2Rwb1WncxOt1h1ZDnNuk8nMcikktrWulOU1OjOn6sBt8gwirSVwqPykNP2cqUvgNHEfmw5D5JODinDYf6GlwpbmgDK64n7GN6KGRg2DTC2XvK88EX9SjRdyryp7UQLFF6UcBVtz35CH1gXncYUjZ30bBY1znxs3mes9tcFH/DNPiJ7SraspsshGhVQELGwrk/YmX+aq6sce2J3fE1+suKzYj+kQ6HmNAdeJxYltxTdsMbSqgH5oqlNIdeSQ==","HostKey":"kkk"},{"Id":1127,"BookId":1100,"BookName":"{{{}}}ZNtW7OQBfY9opQpIpZYuiQ==","BookImage":"https://acbqimg.cdn.bcebos.com/BookFiles/BookImage/acac/bailianchengshen.jpg","Author":"{{{}}}S8HT8v6O2wTieI7LrO5O8g==","CategoryName":"{{{}}}+a6U/XdOsUE=","Score":8.6,"Description":"{{{}}}nYaulf+4bscx2rt+kBOaEwWt+q8neAYiYkFA1hzqnRsvbHvsxBe8+l2nk37ACNzKszrxktxH9aC9eFIq2+lMga79dbvN6IxeyoRZk4L12XszDM1gPMwpSxCvzzAOJJzxRwXtb3u0i44njsoOo3iTr0iTyhxbsJrB6f38+1aZXi4p4KO2YFr6XTeIeL9S9r22lnTxX7j7VXl/aZEkHt0qArEvpjUk8V9Ur1Mw/MdVU3zJH5fh+vRKyfMuJKstJ/J86TpDvilxWpuTwGYYHIbJ5S4l2scg2JwkkATHfnmZWQgVToMrlIxmEKoZOjbmmQdOdphpdY3itXNl7SkN+v4cZGDgeiHAKwkB32ZU14t0vLxsnf5+7E04lLCbyLppGW92rcjuU2VUoIWIYolxgc1FXGWi3iIvdnNFIcnmOuZye9M1aUu4Urw8BceLeglFTWt50y70v7vzWzx7cdC1G/6qE5R+XSjT2EJ/7+e2uSNn3d4=","HostKey":"acac"},{"Id":1128,"BookId":540,"BookName":"{{{}}}u3Wk+DMC+dEgAtp5Os/7jA==","BookImage":"https://kkkbqimg.cdn.bcebos.com/BookFiles/BookImage/kkk/dubuxiaoyao.jpg","Author":"{{{}}}oxW7wymPl4RrSCGpkJKcwg==","CategoryName":"{{{}}}+a6U/XdOsUE=","Score":6.8,"Description":"{{{}}}nhH0BayzqB454Ip5ee8hpLaxp8tk6wg48eI2EVMwkUUmAjVY3p40abyuWEBd+w8sFXLQKgXBsmupr53wqMePVTGimehSbBATLmFxqjOfZqHMIKmA44u4bu4OoLYg0F3jJWxxD3AG/T/Xx99sBtRIH4IQhd4eIZ18LWcMpjydMbA6C4jzLgUFOy0v/meE0lGMR/zQcJjXntRKEKQfC/Ovur82dL0NFPrEsnazILlR+CTw7orHzwLVZtafmPSPa2pgfUdsx28t9VxdZ/aX8wp8Eg==","HostKey":"kkk"},{"Id":1129,"BookId":1054,"BookName":"{{{}}}NNvcJgSUXEMCUtMa/ogY4g==","BookImage":"https://acbqimg.cdn.bcebos.com/BookFiles/BookImage/acac/xiuzhenliaotianqun.jpg","Author":"{{{}}}8MYgLC7Kx0FpHSmTyurYrg==","CategoryName":"{{{}}}GzUp6ctmSII=","Score":9.8,"Description":"{{{}}}nYaulf+4bsfQTDDKVoPDlQxaHY1pC9BLMABUkFKUTLowR2xGucpZHt2vp5RGFu2G1hg3JM4OHV0nJScHSA8Oi5zfc0+HvpFO5Ylefb60R7K24k2+5/iiSGXwahAPP43jYmengGgASDw/NseCK8+s2vF0nekWJpIoQIv5Rxjyk6na2ufmSHKDJml/fM3kAhEJNwnaS9+fOFBPdUMZlJQ4nqdTwvzfH7Q3jXVISreymvOH2ZQTkQNDJcEZWwkNd4yGIUYjVhf57WiFlQARtjxO0XaRWKMCIRGl7l0fJEbKnuS3bHKNg+ISCmeVamaQvp6q9D2zio6IUU2VDJXSkCv9iXY7HNAQ+PBBJB4fncl/dRS53pcS9RHMa8CetVftXBQjRMkIBRo4/5CHS800T+ljKRSZhj0ypLisS9DJ/yEXJP8rbAXc+okgsYihf4Px3xDX95O/3uNDY88wqDt2uPJfMQDPQEG9zEtG3JniJZfgIaNvAdZl1Uigh7bUbUS6t8hq17e7M3T3NOQj9Fve/e5Bxd7Yf28PuH2jLqG/n/nFfgKJqAUi7/seQg==","HostKey":"acac"},{"Id":1130,"BookId":981,"BookName":"{{{}}}ITBm2Pg0nDoig7XLwdEMmA==","BookImage":"https://kkkbqimg.cdn.bcebos.com/BookFiles/BookImage/kkk/dajunfa.jpg","Author":"{{{}}}kBX4+/kETbEASaGSSjhoEw==","CategoryName":"{{{}}}+a6U/XdOsUE=","Score":6.0,"Description":"{{{}}}ITBm2Pg0nDpCA8yx0f9nvcdlYHN+nczLS3Wg4smpJh5lCSIsVM0c4aCmc0u4/llBRgDHck8CZ+QwxNl1kWtfGkv43gprtYZunieFgES8OFUrO6OZf3eZD1Vs70LxDqLqXLNrRfhXHp5Wr/HRUUUqZrPLChWAM+1al5gm6W8HNL7IHwWgOQIuAnhQme9ToqRNakQcJJ8DUKehfr2MrmzuOBzIFcOHbW5+x/S+WkoL5JEOqCUxyivZHAChTVeTsH0VYqEsD2bThjCg0RhlwbjTFbMqVukMf1UxirHKYSb5t+1CIARjyXv1T95G4zX/muZgPqLeFAr+XFBO+JTSVnGysvhrH8hlspNyaflQH9+lgyJNANGFoZ4lQeBM0931AU2vHPEKVUR4tvAxnOmla/GJHkML4EMHBD96I9HNIXXgmW4kywjXvXYAFVwPpL/t2ptk+aKccpsmLPlglTekP7PHArSJY6l3j5Nejgo5C7nu/NJj/yYsa3p64z6jHhUlNF2T78e9jwCoxU0Pv97H/EF3WU1vmKA0M2CbQDe7bBhSz4ZQdXv0aoUGKxBC5SP9Z6h9ymqLN7aDRulK7sYClBaClblaHsslIlhhy+LCCfHMVKZrQ5ZaB5GD+gFnl01jk2cpKw2Xgl3trOka3skp1bdgwdwbmzd4U4FARx7+Hm6l4PlU8CKzX0naamwh5kHN+PDkyUiKBNcJe4XP17z+FOC4AOzRf3hF9yoy/vSDQJFGPkXhB9MwfMwNpjobg7FjVpfpV7hshL6+OoVgXgj+mHcK2odDfUSTsqWY","HostKey":"kkk"},{"Id":1131,"BookId":1317,"BookName":"{{{}}}E2BSipgoE+fSByVnIXC4zg==","BookImage":"https://acbqimg.cdn.bcebos.com/BookFiles/BookImage/acac/yirenzhixia.jpg","Author":"{{{}}}0cD+b4E4WRw=","CategoryName":"{{{}}}GzUp6ctmSII=","Score":9.8,"Description":"{{{}}}OAjQx5kFR1t0pQt09A/kCu2wUZHl6TvY+tDNFKUQ1Y5Zx4pKhMysnzLrXol25KFCi9xf9JgEcvw+Y2WRF+XNfjhhzTMupHRGvyvVaZxYWuoLxTKEGO3t7F+3A5b2B+SIvOJoGxiGEbwEy7fBaOmMRONxboLIse+rgufVPF5zAkx9wr/JiE20zzxvF6Hp/UL2crzj6NCBg+rRV0Ti7zTuYqsY5YL2rdrUtYkjXX0Tpwj85O1fy1ausANZCrUtfcHuYRAkpIP3w39SWSIytAw3Ut4sVtJhjQKu9KEQaLi1HxMjYRs1bRApuuWC4k7+0ffQZMUlLNwysbPn3JjEAMNvxKvyXCsNk2uetrgBtJ0ey27wfv0sanBZcbBTRrItAdKqvKLIvqicG63/sQW+8xqMVwzBdsFSv8n9z7LGMuQXtic+6+g38fIKXQ==","HostKey":"acac"},{"Id":1132,"BookId":93,"BookName":"{{{}}}KRJVITY/l+kJQKjCzoqCrw==","BookImage":"https://kkkbqimg.cdn.bcebos.com/BookFiles/BookImage/kkk/yaodaozhizun.jpg","Author":"{{{}}}3dt7kpsk+R4lCAr5At21tw==","CategoryName":"{{{}}}+a6U/XdOsUE=","Score":6.8,"Description":"{{{}}}jmCK0PGZNSX56knG1YDzWuF3H4oNAi4ggOCyUN9shUFGYvoLcE2bNtGdVqNJMbZ7v5162A4mPR5hmQTKPMUJOaQK5vwOXRRFj+jnpkncVx2CiMlSKGfVLZhMsbsLD9JLJajWkOfyRnn/5ef402VM39hkiB4HHLDPAiaWJ0MzM5Itf9owF8fZB5Q0fqysZ8e0Ftd1fIzpkLxdCkXxm6hHQDkQCvGNkgxbngvj6h25/1M=","HostKey":"kkk"}]}}

### 漫画详情
GET https://infosmanhua.pigqq.com/BookFiles/Html/1/132/info.html HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
Content-Type: application/x-www-form-urlencoded
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Host: infosmanhua.pigqq.com
Connection: Keep-Alive
Accept-Encoding: gzip

{"status":1,"info":"success","data":{"Id":132,"Name":"{{{}}}k061mpe8hvnImbXomdsFjg==","Img":"https://kkkbqimg.cdn.bcebos.com/BookFiles/BookImage/kkk/jueshiwushen.jpg","Author":"{{{}}}Sf7Gx7QMaToESyI84qYEciKJTYXZEpENsOLEaN8Yt8E=","Desc":"{{{}}}S4KUTa0IMEHS0qXE++7uTFituT3hnrFDGtDko+NNfOv7SombZGbJusP7GdCGsTHrYCHR0gRzx/d06b52svWXUGqBM4suxOsPRHBM/atO/puLKGwYQB1145fYM8SRAUdzPxixLPzkZ+ZkjJWoxCXEQalduG77RbiQYYUHSMehBbG2IQUiiMF6Ou3IOB7mNJoc+nGHdPQtL+jt23+1UEWG6IuMSaucgB2//JrAn5+JQp18z+NwznBaqFsYkMOkbL0IBZRb6Sla73mGamWBL+fb1LUROmxpjZbSz1mrUJh+1o5IL8MyhisGuOkgN7PFg9OheDMtZi1bbn59wKSCG2l/s5LIdWDXL8k1kaA8vRCrcOA8VVs01IyRUAkdQdXoNdCqvnUVqcT19+VTP8blPwoylDxfSOcNEnr/pwQbDqdI8gE2VHZNHdnVK6bBaeIq41TCL7vQZ4zdLRgs3ejamWvZe9RkqWOOPeScT4DKlHQVSJ0C2Xma/iTYLu4NSAh0LZ0fWYiNorO9UNIxG7z1NhfZkw+1hOq+XiOerTmuRTC3QckCOVjE4JrO1u8SH/RPB8+cmFBaiUFkPlDVZ0JISsoqxE6J0by4EU9aOo8XQOy349KntVaY9wKaI+CoLQEZH8j/B+2vNmXM/v+FPNRY4Dnx6KgumtrfgdbxHOQhM66OkRq/bHPHDzb5Vlex7FHaec8taZxDlSHMDBueD8Wce9hR8l8YaTm+r4ZUC7JBIkWHGKg=","CId":4,"CName":"热血","LastTime":"2021/9/21 22:00:04","FirstChapterId":1013807,"LastChapter":"第431回 杀禹天行","LastChapterId":1234084,"BookStatus":"连载","UpUser":"U86******1","Declare":"该作品由 书友U86******1 上传贡献，仅供在线阅读，禁止下载，转载方式传播！","SameUserBooks":[],"SameCategoryBooks":[{"Id":4538,"Name":"{{{}}}K5QE9C5HXAe6oplMkK7w87tyDsifxoUpOZeDutlK5j8=","Img":"https://kkkbqimg.cdn.bcebos.com/BookFiles/BookImage/kkk/xiuxianzhedazhanchaonengli.jpg","Score":0.0,"HostKey":"kkk"},{"Id":132,"Name":"{{{}}}k061mpe8hvnImbXomdsFjg==","Img":"https://kkkbqimg.cdn.bcebos.com/BookFiles/BookImage/kkk/jueshiwushen.jpg","Score":0.0,"HostKey":"kkk"},{"Id":129,"Name":"{{{}}}s/P3RyKroZOhrp14M6QSdQ==","Img":"https://kkkbqimg.cdn.bcebos.com/BookFiles/BookImage/kkk/wanjiexianzong.jpg","Score":0.0,"HostKey":"kkk"},{"Id":95,"Name":"{{{}}}VEBs08KXBG062VJBAaaY1A==","Img":"https://kkkbqimg.cdn.bcebos.com/BookFiles/BookImage/kkk/difuwokaide.jpg","Score":0.0,"HostKey":"kkk"},{"Id":8958,"Name":"{{{}}}m0G4zZuhoWeCWOuYVjsUtZ8z/3ssFEzQwgXMA6Bz6Zk=","Img":"https://bilibqimg.cdn.bcebos.com/BookFiles/BookImage/bilibili/40.jpg","Score":0.0,"HostKey":"bilibili"},{"Id":1052,"Name":"{{{}}}h9Vi+JI024jHePJozFyn178DGRGIbrIf","Img":"https://acbqimg.cdn.bcebos.com/BookFiles/BookImage/acac/wodeshouhunvyou.jpg","Score":0.0,"HostKey":"acac"},{"Id":8115,"Name":"{{{}}}ipM4v1JBG0K57O4vZxsWwJ1Y/JcD5YNUwKzZIM43RF4=","Img":"https://rmbqimg.cdn.bcebos.com/BookFiles/BookImage/rm/380.jpg","Score":0.0,"HostKey":"rm"},{"Id":1257,"Name":"{{{}}}4INV2urGM4Ik9+vDYVk9fcSNLrcWgkwl","Img":"https://acbqimg.cdn.bcebos.com/BookFiles/BookImage/acac/woshenshangyoutiaolong.jpg","Score":0.0,"HostKey":"acac"},{"Id":1284,"Name":"{{{}}}ZmyxJL8JoTEZzPQtwsMWgjagsbOeJ3Jg","Img":"https://acbqimg.cdn.bcebos.com/BookFiles/BookImage/acac/xiuxianguilaizaixiaoyuan.jpg","Score":0.0,"HostKey":"acac"},{"Id":544,"Name":"{{{}}}EZOuMd+HNB8OERCAF9g1aw==","Img":"https://kkkbqimg.cdn.bcebos.com/BookFiles/BookImage/kkk/yaozheweiwang.jpg","Score":0.0,"HostKey":"kkk"},{"Id":533,"Name":"{{{}}}8wML++K6nf/XPEl1Dwwrhg==","Img":"https://kkkbqimg.cdn.bcebos.com/BookFiles/BookImage/kkk/xiandiguilai.jpg","Score":0.0,"HostKey":"kkk"},{"Id":165,"Name":"{{{}}}bFNy/FiZabBR3O9fYXjUgA==","Img":"https://kkkbqimg.cdn.bcebos.com/BookFiles/BookImage/kkk/zhongshengbawannian.jpg","Score":0.0,"HostKey":"kkk"}],"BookVote":{"BookId":132,"TotalScore":16,"VoterCount":2,"Score":8.0},"UpdateCycle":"","HostKey":"kkk"}}

### 漫画详情命中 猜测
POST https://usermanhua.pigqq.com/BookAction.aspx HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Content-Type: application/x-www-form-urlencoded
Content-Length: 24
Host: usermanhua.pigqq.com
Connection: Keep-Alive
Accept-Encoding: gzip

action=addhit&bookid=132

2

### 漫画 加入书架
POST https://usermanhua.pigqq.com/BookAction.aspx HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Content-Type: application/x-www-form-urlencoded
Content-Length: 29
Host: usermanhua.pigqq.com
Connection: Keep-Alive
Accept-Encoding: gzip

action=addbookcase&bookId=132

{"status":1,"info":"success","data":{"result": "2"}}

### 漫画 目录
GET https://infosmanhua.pigqq.com/BookFiles/Html/1/132/index.html HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
Content-Type: application/x-www-form-urlencoded
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Host: infosmanhua.pigqq.com
Connection: Keep-Alive
Accept-Encoding: gzip

### 漫画移除书架

POST https://usermanhua.pigqq.com/BookAction.aspx HTTP/1.1
Accept-Language: zh-CN,zh;q=0.8
User-Agent: okhttp-okgo/jeasonlzy
cookie: ASP.NET_SessionId=u42n5ljg33xkjb1t34w2v014; ; m_uid=504dabaa-edef-42d6-8c2d-e96cb83d27eb; expires=Thu, 21-Oct-2021 14:23:04 GMT; member_username=17712522763;
Content-Type: application/x-www-form-urlencoded
Content-Length: 33
Host: usermanhua.pigqq.com
Connection: Keep-Alive
Accept-Encoding: gzip

bookIds=132&action=removebookcase

{"status":1,"info":"批量移除书架成功！","data":{"result": "2"}}
