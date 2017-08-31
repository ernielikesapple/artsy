fastlane documentation
================
# Installation

Make sure you have the latest version of the Xcode command line tools installed:

```
xcode-select --install
```

## Choose your installation method:

<table width="100%" >
<tr>
<th width="33%"><a href="http://brew.sh">Homebrew</a></td>
<th width="33%">Installer Script</td>
<th width="33%">Rubygems</td>
</tr>
<tr>
<td width="33%" align="center">macOS</td>
<td width="33%" align="center">macOS</td>
<td width="33%" align="center">macOS or Linux with Ruby 2.0.0 or above</td>
</tr>
<tr>
<td width="33%"><code>brew cask install fastlane</code></td>
<td width="33%"><a href="https://download.fastlane.tools">Download the zip file</a>. Then double click on the <code>install</code> script (or run it in a terminal window).</td>
<td width="33%"><code>sudo gem install fastlane -NV</code></td>
</tr>
</table>

# Available Actions
### test
```
fastlane test
```
Run all iOS tests on an iPad
### oss_keys
```
fastlane oss_keys
```

### oss
```
fastlane oss
```
Set all the API keys required for distribution
### deploy
```
fastlane deploy
```
Release a new beta version on Hockey

This action does the following:



- Verifies API keys are non-empty

- Ensures a clean git status

- Increment the build number

- Build and sign the app

- Upload the ipa file to hockey

- Post a message to slack containing the download link

- Commit and push the version bump
### storyboard_ids
```
fastlane storyboard_ids
```
Updates the storyboard identifier Swift values.

----

This README.md is auto-generated and will be re-generated every time [fastlane](https://fastlane.tools) is run.
More information about fastlane can be found on [fastlane.tools](https://fastlane.tools).
The documentation of fastlane can be found on [docs.fastlane.tools](https://docs.fastlane.tools).
