# 存量分布--->库存分布

## Last modify date
	helen li 2016-05-20

## Class 
	/vsa_web/src/main/leader/et/leader/stockdistribution/api/StockdistributionAPI.java

## Path
	http://localhost:8080/vsaapi/leader/stockdistribution

## Http type
	GET

## Param
	@param produceId 产品id
 	@param userId 用户id
 	@param corpId 公司id

## Authentication
	需要验证身份
	
## Return
     *单位: 吨
	 * {code:200
	 *	stockNumSum:736.4000吨             //该产品的在库总量
	 *	Sum:736.4                          //该产品的在库总量(double型)
	 *    list:[{
	 *  	  stockName:菏泽自制半成品仓,     //仓库名称
	 *  	  stockNumString:147.0000       //该产品在某一仓库的在库量
	 *	    unitName:吨                   //产品的计量单位
	 *    }],
	 * }

## Exception
   {"code":"500","message":"请绑定营销组织"}

## eg:
http://localhost:8080/vsaapi/leader/stockdistribution?produceId=0012701c-a107-45a0-b707-21d759d378ef&userId=07aafae5-d5c6-4240-a1ba-0f2785d92e4c&keywords=%E9%92%99&corpId=wuzoufen-f76b-4437-a3bd-9f1ab1343dfc