# 运营统计--->本月任务完成率对比

## Last modify date
	helen li 2016-05-20

## Class 
	/vsa_web/src/main/leader/et/vis/leader/api/OperationStatisticsAPI.java

## Path
	http://localhost:8080/vsaapi/leader/ontaskcommitpercentage

## Http type
	GET

## Param
 	@param userId 用户id
 	@param corpId 公司id

## Authentication
	需要验证身份
	
## Return
	 * {
	 *	code:200,
	 *	vos:[{
	 *	  bilv：20%                   //本月任务完成率
	 *	  previous_bilv：30%          //上月任务完成率
	 *	  previous_sales:34           //上月销量
	 *	  previous_task:6500.0000	  //上月任务量
	 *	  ref_salesPercent:20%	      //销量的百分比
	 *	  region_id:b1059019-6e76-477a-a42a-917639a51268   //区域Id
	 *	  region_name:西北大区        //区域名称
	 *	  sales_num:0%                //本月任务完成率
	 *	  tasknum：31                 //本月任务量
	 *  }],
	 * }

## Exception
   {"code":"500","message":"请绑定营销组织"}

## eg:
http://localhost:8080/vsaapi/leader/ontaskcommitpercentage?userId=07aafae5-d5c6-4240-a1ba-0f2785d92e4c&corpId=wuzoufen-f76b-4437-a3bd-9f1ab1343dfc