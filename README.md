Perl-skript that is called by VDR's recording-hook and hibernates the system

This script parses VDR's timers.conf and hibernates the system if this seems
reasonable. The script considers a certain temporal distance till the next
recording and also obtains the user's confirmation to hibernate the system using
the Kodi-plugin 'script.confirm_hibernate'
(https://github.com/Rosepeter/script.confirm_hibernate).

In order to setup this script, the following things have to be accomplished:
- enable the Kodi webserver/JSON API
- replace '[KODIURL]' with the URL of your Kodi-instance
- set RECORDCMD to this script in runvdr.conf
