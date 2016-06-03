
# 分享---运营统计首页查询

## Last modify date
	robin gao 2016-05-24

## Class 
	/vsa_web/src/main/leader/et/vis/share/api/HomeLeaderShareAPI.java

## Path
	http://localhost:8080/vsaapi/leader/share/homepagequery

## Http type
	POST

## Param
 	@param share_id 用户share_id

## Authentication
	否
	
## Return

	 * {share_id:id,
	 * 	share_title: 高建华分享运营统计,
	 * 	description: 运营统计分享2016-05-24 12:20:34数据,
	 *  avatar: http://www.baidu.com,
	 * 	share_date: 2016-05-24,
	 * 	share_time: 2016-05-24 12:20:34,
	 *  type : homepage,
	 *  user_id: user_id,
	 *  user_name: 高建华,
	 *  read_count: 20, //阅读次数
	 *  validity_date: 3000-01-01, //有效期
	 *  content_data : {
	 *  	todayopen: 200.0000 , //今日开单量
	 *  	weekopen:  1,400.0000 ,//本周开单量
	 *  	monthopen: 6,000.0000,//本月开单量
	 *  	monthcompeleted: 14.00,//本月任务完成率
	 *  	yearcompeleted: 30.57,//本年任务完成率
	 *  	sevendateopen: {x:['05-20','05-19'],y:[30,80],monthavg:70,month:06 },//近7天开单量
	 *  	theremonthsaleandtask:{x:[2016-05,2016-06],//日期
	 *  						   y1:[600,800],//销量
	 *                             y2:[700,800]}//任务量
	 *  }
	 * }

## Exception
   {"code":"300","message":"查询失败"}

## eg:
http://localhost:8080/vsaapi/leader/sahre/homepagequery?share_id=1



