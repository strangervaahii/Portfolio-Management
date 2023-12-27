# PortfolioManagementSystem
The project used java, spring Boot,MVC,JPA-H2 frameworks.
1. Run all four microservices authorization,calculatenetworth,dailymutualfund and dailyshareprice
2. First get jwt token using authorization getmapping /getToken using username and password of users.
3. Using postman change GET method to POST inside body give json format user credientals.
4. Apply the token in Bearer Auth,to check authenication /getuname it will show username accessing.
5. Calculate networth running on port 8084, request mapping /calculateNetworth then / to calculateNetworth of the user.
6. DialyMutualFund NAV running on port 8083, request mapping /DailyMutualFundNAV then /allmf shows mutual fund price.
7. DialyShareprice running on port 8082 , request mapping /DailySharePrice then /allstock shows share price.


Local Host URLs:
	1.Authorization
	http://localhost:8081
	
	2.Calculate Networth
	http://localhost:8084
	
	3.DialyMutual Fund NAV
	http://localhost:8083
	
	4.DialyShare Price
	http://localhost:8082
	
H2-console
	Local Host URLs:
	1.Authorization
	http://localhost:8081/h2-console
	
	2.Calculate Networth
	http://localhost:8084/h2-console
	
	3.DialyMutual Fund NAV
	http://localhost:8083/h2-console
	
	4.DialyShare Price
	http://localhost:8082/h2-console



ECS loadbalancers URLs:
	1.Authorization
	http://authorization-load-1729719267.ap-south-1.elb.amazonaws.com
	
	2.Calculate Networth
	http://calculatenetworth-lb-1293029971.ap-south-1.elb.amazonaws.com
	
	3.DialyMutual Fund NAV
	http://mutualfund-lb-1825665396.ap-south-1.elb.amazonaws.com
	
	4.DialyShare Price
	http://shareprice-lb-1113004352.ap-south-1.elb.amazonaws.com


Elastic bean deployed URLs:
	1.Authorization
	http://cde043authorization-env.eba-4he7vvv7.ap-southeast-1.elasticbeanstalk.com/
	
	2.Calculate Networth
	http://cde43calculatenetworth-env.eba-5xc262m6.ap-southeast-1.elasticbeanstalk.com/
	
	3.DialyMutual Fund NAV
	http://cde43mutualfund-env.eba-ippygqpm.ap-southeast-1.elasticbeanstalk.com/
	
	4.DialyShare Price
	http://cde43shareprice-env.eba-dms4nptr.ap-southeast-1.elasticbeanstalk.com/