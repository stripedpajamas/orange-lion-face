# olf
proof of concept


### resources

- will need to create a custom AMI with browser installed but wallet not initialized
- the custom AMI should auto login on reboot, bc olf will be desktop-interactive
  - https://stackoverflow.com/questions/10357313/launching-multiple-ec2-windows-servers-with-auto-logon-from-a-custom-ami
- olf should first run automated wallet initialization and save a file to mark that this step does not need to be run again
- on subsequent runs, olf should execute the main automation flow
  - provide user activity (browse to a website, click a link perhaps)
    - should browse to very low bandwidth websites to save transfer data (possibly stand up a website for this purpose)
  - stay idle (not sure if activity or idleness triggers browser logic)
  - click the close/view button of the ad on a timer
    - detecting the presence of the ad may be out of scope; it would be easier to click where the button would be every few seconds and then resume user activity
- http://robotjs.io

