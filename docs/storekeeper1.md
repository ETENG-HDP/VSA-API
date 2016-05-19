# 库管看板--->今日开单量和今日出库量

## Last modify date
	helen li 2016-05-19

## Class 
	/vsa_web/src/main/leader/et/leader/storekeeper/api/StorekeeperAPI.java

## Path
	http://localhost:8080/vsaapi/leader/todaycount

## Http type
	GET

## Param
 	@param userId 用户id
 	@param corpId 公司id

## Authentication
	需要验证身份
	
## Return
     *单位: 吨
	 * {code:200
	 *  message:{
	 *  	billingQuantity:261.3000, //今日开单量
	 *  	outboundQuantity:85.0000 //今日出库量
	 *  }
	 * }

## Exception
   {"code":"500","message":"请绑定营销组织"}

## eg:
http://localhost:8080/vsaapi/leader/todaycount?userId=07aafae5-d5c6-4240-a1ba-0f2785d92e4c&corpId=wuzoufen-f76b-4437-a3bd-9f1ab1343dfc