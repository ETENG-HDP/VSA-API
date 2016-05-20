# 运营统计--->近30天销量

## Last modify date
	helen li 2016-05-20

## Class 
	/vsa_web/src/main/leader/et/vis/leader/api/OperationStatisticsAPI.java

## Path
	http://localhost:8080/vsaapi/leader/recentopenquantity

## Http type
	GET

## Param
 	@param corpId 公司id
 	@param userId 用户id

## Authentication
	需要验证身份
	
## Return
     *单位: 吨
	 * {
	 *  list1:[{
	 *    rkdlMax:261.3               //近30天的最大开单量
	 *  }],
	 *	code:200,
	 *	list:[{
	 *    rkdl:261.3                 //开单量(double型)
	 *    RKDL:261.3000              //开单量(String型)
	 *    day:2016-05-19             //开单日期
	 *  }],
	 * }

## Exception
   {"code":"500","message":"请绑定营销组织"}

## eg:
http://localhost:8080/vsaapi/leader/recentopenquantity?corpId=wuzoufen-f76b-4437-a3bd-9f1ab1343dfc&userId=07aafae5-d5c6-4240-a1ba-0f2785d92e4c