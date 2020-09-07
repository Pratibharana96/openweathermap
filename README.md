# openweathermap
 weather API in Php and curl using openweathermap.org free 
 
# Using Weather Api From https://openweathermap.org/
Here you can download Examples of Forecast bulk files:
http://bulk.openweathermap.org/sample/
# Using php curl call the api :
api.openweathermap.org/data/2.5/weather?q={city name}&appid={your api key}
Add city id from the json file and api_key after 
registering your account in key section get your keys 
# weather API  demo 
![alt text](https://github.com/Pratibharana96/openweathermap/blob/master/weatherapi.PNG?raw=true)



#                       ABOUT CURL
# cURL Supported Operations
For handling remote file access, the cURL as an intermediary is used for,

# Form submitting
# Authentication
# File upload
# File transfer
Without cURL, we can use PHP file system functionsallow_url_fopen configuration directive which is not preferable because of security reasons. For example, file_get_contents() returns remote data including some untrusted internet content.

# PHP cURL Delimiters
In a PHP program, the cURL portion should be enclosed within this two pair of functions.

$ch = curl_init(URL Syntax);
...
curl_close($ch);
The curl_init() function returns cURL session handle with respect to the given file URL. And then, curl_close() function will be an end delimiter to close cURL session with respect to its handle.

# cURL Options
PHP curl_setopt() function is used to set options. It receives cURL handle, option’s name and value as its parameters.

We can use another cURL function curl_setopt_array() to set an array of multiple options at a push.

curl_setopt ($ch, CURLOPT_HEADER, 1);
# cURL Option Constants
CURLOPT_FILE – target file to write cURL result.
CURLOPT_URL – URL from where we need to get data. If this URL is specified with curl_init(), then no need to set this option
CURLOPT_RETURNTRANSFER – to return the result in string format into a variable instead of printing it to the browser.
CURLOPT_HTTPHEADER – to set header fields as an array.
CURLOPT_POST – set to TRUE to perform HTTP POST.
CURLOPT_USERPWD – to set username/password if required to connect remote server.
php_curl

# PHP cURL Request
Like PHP, the GET and POST methods are used for sending cURL request where GET is the default. The CURLOPT_POST constant is used for sending POST request. And the parameters CURLOPT_POSTFIELDS is for sending parameter array of the field: value pairs.

cURL Execution
After setting request methods and parameters, curl_exec() function is used for executing cURL request.

$result = curl_exec($ch);
This function returns either boolean values or string data based on the value of option CURLOPT_RETURNTRANSFER.

