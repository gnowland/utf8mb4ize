=== Utf8mb4ize ===
Contributors: gnowland, PressLabs
Tags: utf8mb4ize, utf8ize, gnowland, database, convert, sql, alter, table
Requires at least: 3.5.1
Tested up to: 5.5.1
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

Convert all your database character sets to utf8mb4, trying to follow Codex guides. 

== Description ==
Convert all your database character sets to utf8mb4, in line with <a href="https://make.wordpress.org/core/2015/04/02/the-utf8mb4-upgrade/">WordPress recommendations</a>.

It works by scanning all you tables and columns and generating a list of SQL statements which allow you to convert to convert your content to utf8mb4.

!!! CAUTION !!!
The execution time of the next SQL statements may take a lot of time(even days), related to dimensions of your database and the amount of the content.

== Installation ==

= Installation =
1. Upload `utf8mb4ize.zip` to the `/wp-content/plugins/` directory;
2. Extract the `utf8mb4ize.zip` archive into the `/wp-content/plugins/` directory;
3. Activate the plugin through the 'Plugins' menu in WordPress.

= Usage =
Use your plugin from the `Tools->Utf8mb4ize` page;

Update your <pre>wp-config.php</pre> file:
<pre>
define('DB_CHARSET', 'utf8mb4');
define('DB_COLLATE', 'utf8mb4_unicode_ci');
</pre>

== Frequently Asked Questions ==

= Why should I use this plugin? =
You should use this if you are using encoding other than utf8mb4.

== Changelog ==

= 2.0 =
Updated mysql to mysqli (for PHP >= 7)
Updated utf8 to utf8mb4

= 1.1 =
Updated to WP 4.5

= 1.0 =
Start version on WP.

