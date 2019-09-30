# 0day-php-7.x
Use after free with json serializer

This exploit utilises a use after free vulnerability in json serializer in order to bypass disable_functions and execute a system command. It should be fairly reliable and work on all server apis, although that is not guaranteed.


source : https://bugs.php.net/bug.php?id=77843

Targets:

[ * ] 7.1 - all versions to date

[ * ] 7.2 < 7.2.19 (released: 30 May 2019)

[ * ] 7.3 < 7.3.6 (released: 30 May 2019)

Poc: http(s)://vulnerablesite.com/exp.php?cmd=ls


