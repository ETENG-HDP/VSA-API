# 账款统计-->近三月预收款和总打款对比

## Last modify date
	robin gao 2016-05-18

## Class 
	/vsa_web/src/main/leader/et/leader/money/api/AccountMoneyAPI.java

## Path
	http://localhost:8080/vsaapi/leader/statisticsmoneyquarter

## Http type
	GET

## Param
 	@param userId 用户id
 	@param corpId 公司id

## Authentication
	需要验证身份
	
## Return
	 * 单位: 万元

	 * {code:200
	 *  message:{
	 *  x:['2016-01','2016-02','2016-03'],     // 日期月份
	    y1:['300.98','400.00','500.98']  // 预收款
	    y2:['300.98','400.00','500.98']  //总打款
	 *  }}

## Exception
   {"code":"500","message":"请绑定营销组织"}

## eg:
http://localhost:8080/vsaapi/leader/statisticsmoneyquarter?userId=07aafae5-d5c6-4240-a1ba-0f2785d92e4c&corpId=wuzoufen-f76b-4437-a3bd-9f1ab1343dfc