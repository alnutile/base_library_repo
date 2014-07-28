## Base Install

See lib/Foo and test/Foo/Tests for the example files

Set composer.json to the right folder for psr


## Setting Environment Variables

Copy env_example to .env (which is in git ignore
Then put your variables in there

~~~
TOKEN=SECRET
~~~

Then in your app or class include


~~~
use Dotenv;

\Dotenv::load(__DIR__.'/../../');
~~~

Later on use it

~~~
$_ENV['TOKEN']
~~~

This allows you to not store this info in a db or git and then
it works in all the php frameworks independent of their gettings and settings for
variables. This makes testing easier as well.


## RoadMap

  * Test showing dot env files
