# REDCapCalendarCrawler
parses RedCap calendar and finds subjects that have no scheduled visits.

# Instalation
In the hooks file of your REDCap (path to this file may be set in the Control Center under General Configuration->REDCap Hooks) has to contain:

function redcap_project_home_page ( int $project_id ) {
        include_once "hooks/REDCapCalendarCrawler.php";
}

and there has to be a directory named hooks that contains the REDCapCalendarCrawler.php file.
