# 存量分布--->选择商品

## Last modify date
	helen li 2016-05-20

## Class 
	/vsa_web/src/main/leader/et/leader/stockdistribution/api/ChooseAPI.java

## Path
	http://localhost:8080/vsaapi/leader/queryall

## Http type
	GET

## Param
 	@param userId 用户id
 	@param corpId 公司id
 	@param page 页面已有记录数目
	 @param keywords 输入框内容

## Authentication
	需要验证身份
	
## Return
     *单位: 吨
	 * {code:200
	 *  list:[{
	 *  	produceName:液体钙肥,          //产品名称
	 *  	produceCode:F29-1              //产品编码
	 *	  sort:2     //产品类型  1.产品 2.原材料 3.包装袋 4.半成品
	 *	  produceId:073baa38-695d-4a41-a9ef-4027e5432081  //产品Id
	 *  }],
	 * }

## Exception
   {"code":"500","message":"请绑定营销组织"}

## eg:
http://localhost:8080/vsaapi/leader/queryall?corpId=wuzoufen-f76b-4437-a3bd-9f1ab1343dfc&userId=07aafae5-d5c6-4240-a1ba-0f2785d92e4c&keywords=%E9%92%99