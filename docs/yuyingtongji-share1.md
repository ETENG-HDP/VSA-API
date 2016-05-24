
# 分享---运营统计首页提交数据

## Last modify date
	robin gao 2016-05-24

## Class 
	/vsa_web/src/main/leader/et/vis/share/api/HomeLeaderShareAPI.java

## Path
	http://localhost:8080/vsaapi/leader/share/homepagecommit

## Http type
	POST

## Param
 	@param user_id 用户id
 	@param corp_id 公司id
 	@param data json String
 	 * {
	 * 	share_title: 高建华分享运营统计,
	 * 	description: 运营统计分享2016-05-24 12:20:34数据,
	 *  content_data : {
	 *  	todayopen: 200.0000 , //今日开单量
	 *  	weekopen:  1,400.0000 ,//本周开单量
	 *  	monthopen: 6,000.0000,//本月开单量
	 *  	monthcompeleted: 14.00,//本月任务完成率
	 *  	yearcompeleted: 30.57,//本年任务完成率
	 *  	sevendateopen: {x:['05-20','05-19'],//日期
	 *						y:[30,80], // 开单量
	 *						monthavg:70 },//本月开单量平均值
	 *  	theremonthsaleandtask:{x:[2016-05,2016-06],//日期
	 *  						   y1:[600,800],//销量
	 *                             y2:[700,800]}//任务量
	 *   }
	 * }

## Authentication
	否
	
## Return
	 * {
	 *  code : '200',
	 *  message: 'http://www.baidu.com?share_id=1'
	 * }
## Exception
   {"code":"300","message":"分享失败"}

## eg:
http://localhost:8080/vsaapi/leader/share/homepagecommit?user_id=07aafae5-d5c6-4240-a1ba-0f2785d92e4c&corp_id=wuzoufen-f76b-4437-a3bd-9f1ab1343dfc



