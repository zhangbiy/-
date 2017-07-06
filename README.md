# python
简单封装python常用方法：

1.excelToJson 把excel格式化为json对象。
	例：eg.xls
	------------------
	|名称1	|名称2  |			    {
	------------------				"hosuser":{
	|hosuser	|					"hosId":"fe248c58621411e7aa9f94de806bed23",
	------------------					"hosEge":""
	|	|hosId  |				 },	
	------------------	   --->			"hosName":"",
	|	|hosEge |				 "depaName":"",
	------------------  				 "perNum":"" ,     		
    	|hosName|	|				 "signNum":""				   
        ------------------ 			     }				         
       	|depaName|	|						 
    	------------------					   
    	|perNum	|	|					    
    	------------------					   
    	|signNum|	|					   
    	------------------					   
						
	commUtils.excelToJson('eg.xls')
	
		
2. formatJson json格式化。
3. formatSql sql替换。
	eg:
	sql = 'insert into hos_user (hos_id, sys_user_id, hos_name, busi_lic_num, org_code, tax_reg_ctf, legp_idc, org_hono_ctf, brief_intr, add_prov,add_city,add_dist,address,address, comp_main, hos_intr, bank_num, open_bank_name, acnt_name, cta_name, cta_tel, cta_name2, cta_tel2, create_by, create_date, update_by, update_date, del_flag, main_img,cust_ser_name,cust_ser_tel_num,cust_ser_email, cust_ser_name2,cust_ser_tel_num2,cust_ser_email2 ) values (?, ?, ?, ?, ?, ?, ?, ?, ?, ?,?,?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?,?,?, ?,?,? )'	
	param = '2447372957568949(Long), 0cae3071cd8b4ac58e87a9d1210d13be(String), 3hos001(String), hos001hos001(String), null, null, null, null, null, 110000(String), 110100(String), 110101(String), 18211111111(String), null, null, 12312312312312(String), 12312312312(String), null, hos001(String), 18211111111(String), hos001(String), 18211111111(String), 63b0cf2e354a497b99b2d422c1b8b9df(String), 2017-07-04 13:40:26.26(Timestamp), 63b0cf2e354a497b99b2d422c1b8b9df(String), 2017-07-04 13:40:26.26(Timestamp), 0(String), null, 18211111111(String), 18211111111(String), 18211111111@aa.com(String), 18211111111(String), 18211111111(String), 18211111111@aa.com(String)'
	
	insert into hos_user (hos_id, sys_user_id, hos_name, busi_lic_num, org_code, tax_reg_ctf, legp_idc, org_hono_ctf, brief_intr, add_prov,add_city,add_dist,address,address, comp_main, hos_intr, bank_num, open_bank_name, acnt_name, cta_name, cta_tel, cta_name2, cta_tel2, create_by, create_date, update_by, update_date, del_flag, main_img,cust_ser_name,cust_ser_tel_num,cust_ser_email, cust_ser_name2,cust_ser_tel_num2,cust_ser_email2 ) values ('2447372957568949', '0cae3071cd8b4ac58e87a9d1210d13be', '3hos001', 'hos001hos001', null, null, null, null, null, '110000','110100','110101', '18211111111', null, null, '12312312312312', '12312312312', null, 'hos001', '18211111111', 'hos001', '18211111111', '63b0cf2e354a497b99b2d422c1b8b9df', '2017-07-04 13:40:26.26', '63b0cf2e354a497b99b2d422c1b8b9df', '2017-07-04 13:40:26.26', '0', null, '18211111111','18211111111','18211111111@aa.com', '18211111111','18211111111','18211111111@aa.com' )
4. formatUrl 获取url参数。返回json
5. getDate 获取当前日期。
6. jsonToExcel json转excel
7. random 随机数
8. uuid 获取uuid
9. replaceName 下划线名称字段取出转大写 ui_id -> uiId	
10.parsing_sql sql 字段信息打印	
