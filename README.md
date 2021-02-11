SourceQuery
===========

A simple PHP class to query a [Source engine](http://en.wikipedia.org/wiki/Source_%28game_engine%29) server.

How to use
----------

### Example

PHP:

	require_once 'lib/SourceQuery.php';
	
	$server = new SourceQuery('217.70.184.250', 27015);
	$infos  = $server->getInfos();
	echo $infos['players'];
	// $infos['name'] - Server Name
	// $infos['players'] - Count of players
	// $infos['places'] - Slot server
	// $infos['map'] - Current Map
	// $infos['ip'] - Ip
	// $players[$i]['name'] - Nickname of $i(int) player 
