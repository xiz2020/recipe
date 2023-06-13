**Description** 

Creative recipes. The API provides access to 231,637 creative recipes from all cuisines around the world.

**API:** 

https://rapidapi.com/zilinskivan/api/recipe64/

**Code Samples:** 

**-HTTP**

<pre>
GET /?q=taco HTTP/1.1
X-Rapidapi-Key: Your API Key
X-Rapidapi-Host: recipe64.p.rapidapi.com
Host: recipe64.p.rapidapi.com
</pre>

**-NodeJS**

<pre>
const axios = require('axios');

const options = {
  method: 'GET',
  url: 'https://recipe64.p.rapidapi.com/',
  params: {q: 'taco'},
  headers: {
    'X-RapidAPI-Key': 'Your API Key',
    'X-RapidAPI-Host': 'recipe64.p.rapidapi.com'
  }
};

try {
	const response = await axios.request(options);
	console.log(response.data);
} catch (error) {
	console.error(error);
}
</pre>

**-PHP**

<pre>
<?php

$curl = curl_init();
curl_setopt_array($curl, [
	CURLOPT_URL => "https://recipe64.p.rapidapi.com/?q=taco",
	CURLOPT_RETURNTRANSFER => true,
	CURLOPT_ENCODING => "",
	CURLOPT_MAXREDIRS => 10,
	CURLOPT_TIMEOUT => 30,
	CURLOPT_HTTP_VERSION => CURL_HTTP_VERSION_1_1,
	CURLOPT_CUSTOMREQUEST => "GET",
	CURLOPT_HTTPHEADER => [
		"X-RapidAPI-Host: recipe64.p.rapidapi.com",
		"X-RapidAPI-Key: Your API Key"
	],
]);

$response = curl_exec($curl);
$err = curl_error($curl);

curl_close($curl);

if ($err) {
	echo "cURL Error #:" . $err;
} else {
	echo $response;
}
</pre>
