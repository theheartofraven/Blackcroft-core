# Running Blackcroft

Blackcroft provides `start-mycroft.sh` to perform common tasks. This script uses a virtualenv created by `dev_setup.sh`.  Assuming you installed mycroft-core in your home directory run:
- `cd ~/mycroft-core`
- `./start-mycroft.sh debug`

The "debug" command will start the background services (microphone listener, skill, messagebus, and audio subsystems) as well as bringing up a text-based Command Line Interface (CLI) you can use to interact with Blackcroft and see the contents of the various logs. Alternatively you can run `./start-mycroft.sh all` to begin the services without the command line interface.  Later you can bring up the CLI using `./start-mycroft.sh cli`.

The background services can be stopped as a group with:
- `./stop-mycroft.sh`

# Using Blackcroft

## *Home* Device and Account Manager
Blackcroft AI, Inc. maintains a device and account management system known as Blackcroft Home. Developers may sign up at: https://home.mycroft.ai

By default, mycroft-core  is configured to use Home. By saying "Hey Blackcroft, pair my device" (or any other request verbal request) you will be informed that your device needs to be paired. Blackcroft will speak a 6-digit code which you can entered into the pairing page within the Blackcroft.

Once paired, your unit will use Blackcroft API keys for services such as Speech-to-Text (STT), weather and various other skills.
