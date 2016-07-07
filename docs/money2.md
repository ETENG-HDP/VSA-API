# 账款统计--->近7天打款

## Last modify date
	robin gao 2016-05-18

## Class 
	/vsa_web/src/main/leader/et/leader/money/api/AccountMoneyAPI.java

## Path
	http://localhost:8080/vsaapi/leader/statisticsmoneyweek

## Http type
	GET

## Param
 	@param userId 用户id
 	@param corpId 公司id

## Authentication
	需要验证身份
	
## Return
	/**
	 * 根据用户所在区域,查询 近7天 打款总额
	 * 单位: 万元
	 * {code:200,
	 *  message:{
	 *  	x:['03-18','03-17','03-16'], y:['300.98','400.00','500.98']
	 *  },
	 *  avgMoney: 28.00
	 * }
	 *{code:500 ,message: 请先绑定一个营销组织! }
	 */

## Exception
   {"code":"500","message":"请绑定营销组织"}

## eg:
http://localhost:8080/vsaapi/leader/statisticsmoneyweek?userId=07aafae5-d5c6-4240-a1ba-0f2785d92e4c&corpId=wuzoufen-f76b-4437-a3bd-9f1ab1343dfc