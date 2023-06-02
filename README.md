# actions-vms
Short-living VMs abusing Github Actions for testing all kinds of things. :eyes:

## How to use
1. Fork this repository
2. Set the fork to private for security reasons[^1]
3. Navigate to the "Actions" tab and enable Github Actions for your fork
4. Select one of the workflows and press the "Run workflow" button
5. Wait until the workflow logs a message similar to `Web shell: https://tmate.io/t/xyz`, then open that link
6. You might have to press <kbd>Control</kbd>+<kbd>C</kbd> once to use the web terminal
7. You can now use the web terminal to test any kinds of things on the Github Actions machine

**Note:** every workflow automatically stops after 15 minutes to prevent stale or forgotten workflows from wasting minutes.
<br>You can change this by editing the `timeout-minutes` field in the workflow file.

[^1]: Note that private repositories do not have unlimited workflow minutes and thus using the scripts here frequently may cost you money.
