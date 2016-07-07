# 账款统计--->账户余额和今日关注

## Last modify date
	robin gao 2016-05-18

## Class 
	/vsa_web/src/main/leader/et/leader/money/api/AccountMoneyAPI.java

## Path
	http://localhost:8080/vsaapi/leader/statisticsaccountmoney

## Http type
	GET

## Param
 	@param userId 用户id
 	@param corpId 公司id

## Authentication
	需要验证身份
	
## Return
     *单位: 万元
	 * {code:200
	 *  message:{
	 *  	accountAmount:40000.00, //账户余额
	 *		accountBalance:30000.00 //资金余额
	 *		accountRemain:10000.00   //剩余额度
	 *  	accountCredit:5000.00 //赊销欠款
	 *  }
	 * today:{
	 *  	payMoney:40000.00, //打款总额 openMoney:5000.00 ,//开单总额
	 *  	advanceMoney:5000.01, //预收货款  cash:3000.00//现收货款
	 *  }}

## Exception
   {"code":"500","message":"请绑定营销组织"}

## eg:
http://localhost:8080/vsaapi/leader/statisticsaccountmoney?userId=07aafae5-d5c6-4240-a1ba-0f2785d92e4c&corpId=wuzoufen-f76b-4437-a3bd-9f1ab1343dfc
