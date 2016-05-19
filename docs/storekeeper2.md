# 库管看板--->待出库量

## Last modify date
	helen li 2016-05-19

## Class 
	/vsa_web/src/main/leader/et/leader/storekeeper/api/StorekeeperAPI.java

## Path
	http://localhost:8080/vsaapi/leader/waitquantitycount

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
	 	waitQuantityMax:50,                //最大待出库量
	 *  list:[{
	 *  	waitQuantityMax:50,            //待出库量
	 *  	customerName:OD16051910304601  //出库单号
	 *  }],
	 *	waitQuantitySum:                   //待出库量总和   
	 * }

## Exception
   {"code":"500","message":"请绑定营销组织"}

## eg:
http://localhost:8080/vsaapi/leader/waitquantitycount?userId=07aafae5-d5c6-4240-a1ba-0f2785d92e4c&corpId=wuzoufen-f76b-4437-a3bd-9f1ab1343dfc