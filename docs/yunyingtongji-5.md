# 运营统计--年任务完成率详情

## Last modify date
	robin gao 2016-05-10

## Class 
	/vsa_web/src/main/leader/et/vis/leader/api/OperationStatisticsAPI.java

## Path
	http://localhost:8080/vsaapi/leader/queryyeartaskcomplitepresent

## Http type
	GET

## Param
 	@param userId 用户id
 	@param corpId 公司id

## Authentication
	需要验证身份
	
## Return
	 * {"code" : "200",
	    //每月任务完成率
	 * 	"message" :[   
	 * 	{ "busdate" : "2016年1月",
	 * *  "renwulwanchenglv":"49.99",
	 *	  "sale": "12.00",
	 *	  "task": "42.98"
	 *   },{}
	 * ],
	  // 本年任务完成率,销售量,任务量
	 * "renwulwanchenglv":"49.99",
	 *	"sale": "12.00",
	 *	"task": "42.98"
	 * }
	 */

## Exception
   {"code":"200","message":"请绑定营销组织"}

## eg:
http://localhost:8080/vsaapi/leader/queryyeartaskcomplitepresent?userId=07aafae5-d5c6-4240-a1ba-0f2785d92e4c&corpId=wuzoufen-f76b-4437-a3bd-9f1ab1343dfc