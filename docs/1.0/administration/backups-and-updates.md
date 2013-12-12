# Backups and updates

The Elefant CMS framework has a simple way of backing up and updating your
sites. It provides a set of commands on the command line, which are great
for system administrators who can automate tasks or integrate backups and
updates into existing processes.

To backup your site, run the following command from the document root of
your website:

	./elefant backup /path/to/backups

This will create an archived copy of your site in the specified folder with
the current date/time in the file name. In the archive, the database is
exported to a file named `dump.sql`.

To update your site when a new release of the software is available, first
backup your site then run the following command:

	./elefant update all

This will fetch the latest versions of the Elefant CMS and any installed
apps, including Lemur Learning, and apply the updates to your site.

Next: [[:Using the Lemur API]]