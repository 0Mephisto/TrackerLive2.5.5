# Tracker for Flowstate 4.5, vGameSDK013_patch, sdk: 2.5 rc5 base.
 Drag and drop all files into root R5Reloaded folder. 

# For verified hosts, generate your config file here:
 https://r5r.dev/cp/?tab=config

# Otherwise, move R5Reloaded/tracker/examples/r5rdev_config.json to R5Reloaded/platform/
# Finally: Ensure default tracker playlists settings are correct:
 \
 \
 \
 \
 \
/////////////////////////////////////////////////////////////////////////////////// \
//// THE FOLLOWING SETTINGS REQUIRE TRACKER DLL (add-on mod)				/////// \
/////////////////////////////////////////////////////////////////////////////////// \
 \
logging_enabled 								1		// Enabling this will run the tracker system ( TODO: rename to tracker_enabled ) \
logging_encryption								1 \
logging_shipstats 								1		// Enabling this will transfer data at end of match ( TODO: rename to tracker_shipstats ) \
use_global_stats								1		// Enabling this will use API data ( which only transfers at the start/end of a match or when a non batched player connects for stat queries ) \
use_online_motd 								0		// Still indev ( don't enable ) \
tracker_max_wait								7.0		// Max wait for batch load. Reducing means faster loading of data, at the trade off of missing some connecting players still loading, who will get individually queue tasks to fetch stats and codecallback when complete for each player respectively.\
 \
// You should configure the following in "platform/r5rdev_config.json", but also set to 1 to enable here. \
stats_discord_webhook_player_count				0		// Sends player join and disconnect data to a discord webhook \
stats_discord_webhook_matches_enabled			0		// Sends recap data to a discord webhook \
 \
// Restricted Servers \
restricted_server								0		// Enables restricted (private) server settings \
restricted_join_message							"Welcome to the restricted server. \n\n You meet the minimum requirements to play on this server." \
restricted_whitelist_message					"You have been whitelisted for this restricted server" \
restricted_kills								500		// Minimum kills required to join \
restricted_kd									0.7		// Minimum K/D ratio required to join \
restricted_playtime								10000	// Minimum play time in seconds required to join \
restricted_gamesplayed							10		// Minimum games played required to join \
restricted_rank									200		// Minimum rank required to join \
restricted_kick_log								1
