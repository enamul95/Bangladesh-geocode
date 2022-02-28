# Bangladesh-geocode

Division, District, Upazila and, Union level fully mapped only one table MySQL,ORACLE etc. You just import the table or copy the insert 
statment & execute to any SQL support database. I just mapped  Division, District, Upazila and, Union in a signle table.

 1. GET DIVISION JUST USE Bellow QUERY:
   - SELECT * FROM `geocode` WHERE `hardcode` = 'DIV' 
   -
You will find Divison
    id	hardcode	softcode	name	 actflg	createdate
    
    1 	DIV 	CHA 	Chattagram 	চট্টগ্রাম 	Y 	2022-03-01 00:22:34
    2 	DIV 	RAJ 	Rajshahi         রাজশাহী    Y 	  2022-03-01 00:22:34
	
	
2. GET DISTRICT JUST USE Bellow QUERY:

 - SELECT * FROM `geocode` WHERE `hardcode` = <selected soft soft code of diviosn> or select drop down & add softcode value to execute query 
	like bellow:
	SELECT * FROM `geocode` WHERE `hardcode` = 'CHA'
	or
	SELECT * FROM `geocode` WHERE `hardcode` = 'RAJ'
	or etc...
	
	output:
	id	hardcode	softcode	name	bn_name	url	actflg	createdate 	
	9 	CHA 	COMI 	Comilla 	কুমিল্লা 	www.comilla.gov.bd 	Y 	2022-03-01 00:27:12
	10 	CHA 	FENI 	Feni 	ফেনী 	www.feni.gov.bd 	Y 	2022-03-01 00:27:12
	.....
	
	NOTE: softcode column will be hard code value like 
	
3. GET UPZILLA JUST USE Bellow QUERY:
	-SELECT * FROM `geocode` WHERE `hardcode` = 'COMI' or <selected drop down softcode of district>

4. GET Union JUST USE Bellow QUERY:
	-SELECT * FROM `geocode` WHERE `hardcode` = 'DEBUZ' or  <selected drop down softcode of upzilla>
	
