# Calibrated!

This is a middleware for django which gives same structure in django success and error case.

When frontend softwares integrate apis, then they expect response structure should remain same in case of both error and success. By adding this middleware onne can achive sam structure through out.

{
	"status":  false,
	"detail":  {},
	"error_detail":  {
}
}

The above payload is the structure which one can recive by applying the package to django appliaction.

> Description to payload

 

 - status field can be true or false in success and error case respectively
 - detail field will always be in form of dict and will hold value only in case of success(2xx)
 - error_detail will have detail in cases excluding (2xx)
 


 

# Steps to install

This is quite easy to use 

pip install calibrated

After installing pip package, go to you django settings and add middeware

calibrated.Response
