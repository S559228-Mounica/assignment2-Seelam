# assignment2-Seelam
Webapps second asignment
# Mounica Seelam
###### My favourite team sport is CRICKET
Cricket is a sport that helps you build your **team-work skills**. It is a very **popular** sport back in my country,India. So, it has been my favourite sport since my childhood.
---
## Favourite Teams
1. Indian Team
    1. Kohli
    2. Dhoni
    3. Rohit
* Australian Team
* South African Team

[About me](https://github.com/S559228-Mounica/assignment2-Seelam/blob/main/AboutMe.md)
------
# Countries that you must visit
The below table contains details about the countries that you must visit atleast once in your life. The first coloumn specifies the Country name, second column specifies the reasons why you should visit the country and the third column specifies the no.of days to be spent.
| Country | Reasons | No.of Days|
| --- | --- | --- |
|India|Diverse country|15|
|Australia|Beautiful weather|13|
|France|Great Monuments|20|
|Canada|rivers and waterfalls|25|
------
# Pithy Quotes
> I'm sick of following my dreams, man. I'm just going to ask where they're going and hook up with ’em later. 

*-Mitch Hedberg*

> Two things are infinite: the universe and human stupidity. And I'm not sure about the universe.

*-Albert Einstein*

-----
# php code
> How to get latest Twitter Status <https://stackoverflow.com/questions/17049821/setting-up-twitter-api-getting-the-last-few-tweets>
```
<?php

function getTwitterStatus($userid){
$url = "https://api.twitter.com/1/statuses/user_timeline/$userid.xml?count=1&include_rts=1callback=?";

$xml = simplexml_load_file($url) or die("could not connect");

       foreach($xml->status as $status){
       $text = $status->text;
       }
       echo $text;
 }

// USAGE
getTwitterStatus("chriscoyier");

?>
```
Snippet source <https://css-tricks.com/snippets/php/get-latest-twitter-status/>