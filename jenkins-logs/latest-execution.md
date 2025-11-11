# Jenkins Execution Log

## Build Information
- **Job Name:** `MBP_Github_BlackduckSca_Async/main`
- **Build Number:** #2
- **Build Status:** 🟢 **SUCCESS**
- **Duration:** 1 min 13 sec and counting
- **Timestamp:** 2025-11-11 18:16:39 UTC

---

## Console Output

```
Branch indexing
Connecting to https://api.github.com using madhusud@blackduck.com/****** (Github_Username_PAT)
Obtained nodejs-npm/Jenkinsfile from 79b0f386dfac1c093b46bb149fc9d2d87e65b5b6
Loading library blackduck-logs-publisher@main
Attempting to resolve main from remote references...
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git ls-remote -h -- https://github.com/integrations-garage/blackduck-logs-publisher # timeout=10
Found match: refs/heads/main revision e969196a63b1be83b84541b022f7aa52928bd5e5
The recommended git tool is: NONE
using credential Github_Username_PAT
 > git rev-parse --resolve-git-dir /Users/madhusud/.jenkins/workspace/P_Github_BlackduckSca_Async_main@libs/a0dda568bac7bbb4a171f59ba3f2660c21c69edc6356524e9ae8bb4500c12bbb/.git # timeout=10
Fetching changes from the remote Git repository
 > git config remote.origin.url https://github.com/integrations-garage/blackduck-logs-publisher # timeout=10
Fetching without tags
Fetching upstream changes from https://github.com/integrations-garage/blackduck-logs-publisher
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git fetch --no-tags --force --progress -- https://github.com/integrations-garage/blackduck-logs-publisher +refs/heads/*:refs/remotes/origin/* # timeout=10
Checking out Revision e969196a63b1be83b84541b022f7aa52928bd5e5 (main)
 > git config core.sparsecheckout # timeout=10
 > git checkout -f e969196a63b1be83b84541b022f7aa52928bd5e5 # timeout=10
Commit message: "Phase 3 - 2"
 > git rev-list --no-walk e969196a63b1be83b84541b022f7aa52928bd5e5 # timeout=10
[Pipeline] Start of Pipeline
[Pipeline] node
Running on mac-sh in /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main@2
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Declarative: Checkout SCM)
[Pipeline] checkout
The recommended git tool is: NONE
using credential Github_Username_PAT
Cloning the remote Git repository
Cloning with configured refspecs honoured and without tags
Cloning repository https://github.com/blackducksca-jenkins-samples/async-mode.git
 > git init /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main@2 # timeout=10
Fetching upstream changes from https://github.com/blackducksca-jenkins-samples/async-mode.git
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git fetch --no-tags --force --progress -- https://github.com/blackducksca-jenkins-samples/async-mode.git +refs/heads/main:refs/remotes/origin/main # timeout=10
Avoid second fetch
Checking out Revision 79b0f386dfac1c093b46bb149fc9d2d87e65b5b6 (main)
Commit message: "Create Jenkinsfile"
First time build. Skipping changelog.
 > git config remote.origin.url https://github.com/blackducksca-jenkins-samples/async-mode.git # timeout=10
 > git config --add remote.origin.fetch +refs/heads/main:refs/remotes/origin/main # timeout=10
 > git config core.sparsecheckout # timeout=10
 > git checkout -f 79b0f386dfac1c093b46bb149fc9d2d87e65b5b6 # timeout=10
[Pipeline] }
[Pipeline] // stage
[Pipeline] withEnv
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Build)
[Pipeline] script
[Pipeline] {
[Pipeline] echo
JOB_NAME: MBP_Github_BlackduckSca_Async/main
[Pipeline] dir
Running in /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main@2/nodejs-npm
[Pipeline] {
[Pipeline] sh
+ node --version
v22.16.0
[Pipeline] sh
+ npm --version
10.9.2
[Pipeline] sh
+ npm install
npm warn deprecated fsevents@1.2.9: fsevents 1 will break on node v14+ and could be using insecure binaries. Upgrade to fsevents 2.
npm warn deprecated set-value@2.0.0: Critical bug fixed in v3.0.1, please upgrade to the latest version.
npm warn deprecated mixin-deep@1.3.1: Critical bug fixed in v2.0.1, please upgrade to the latest version.
npm warn deprecated ini@1.3.5: Please update to ini >=1.3.6 to avoid a prototype pollution issue
npm warn deprecated set-value@0.4.3: Critical bug fixed in v3.0.1, please upgrade to the latest version.
npm warn deprecated path-is-absolute@2.0.0: This package is no longer relevant as Node.js 0.12 is unmaintained.
npm warn deprecated urix@0.1.0: Please see https://github.com/lydell/urix#deprecated
npm warn deprecated har-validator@5.1.3: this library is no longer supported
npm warn deprecated to-iso-string@0.0.2: to-iso-string has been deprecated, use @segment/to-iso-string instead.
npm warn deprecated cryptiles@2.0.5: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated resolve-url@0.2.1: https://github.com/lydell/resolve-url#deprecated
npm warn deprecated bcrypt-nodejs@0.0.3: bcrypt-nodejs is no longer actively maintained. Please use bcrypt or bcryptjs. See https://github.com/kelektiv/node.bcrypt.js/wiki/bcrypt-vs-brypt.js to learn more about these two options
npm warn deprecated cryptiles@0.2.2: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated source-map-url@0.4.0: See https://github.com/lydell/source-map-url#deprecated
npm warn deprecated boom@0.4.2: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated debug@3.2.6: Debug versions >=3.2.0 <3.2.7 || >=4 <4.3.1 have a low-severity ReDos regression when used in a Node.js environment. It is recommended you upgrade to 3.2.7 or 4.3.1. (https://github.com/visionmedia/debug/issues/797)
npm warn deprecated debug@3.2.6: Debug versions >=3.2.0 <3.2.7 || >=4 <4.3.1 have a low-severity ReDos regression when used in a Node.js environment. It is recommended you upgrade to 3.2.7 or 4.3.1. (https://github.com/visionmedia/debug/issues/797)
npm warn deprecated debug@3.2.6: Debug versions >=3.2.0 <3.2.7 || >=4 <4.3.1 have a low-severity ReDos regression when used in a Node.js environment. It is recommended you upgrade to 3.2.7 or 4.3.1. (https://github.com/visionmedia/debug/issues/797)
npm warn deprecated debug@3.2.6: Debug versions >=3.2.0 <3.2.7 || >=4 <4.3.1 have a low-severity ReDos regression when used in a Node.js environment. It is recommended you upgrade to 3.2.7 or 4.3.1. (https://github.com/visionmedia/debug/issues/797)
npm warn deprecated boom@2.10.1: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated chokidar@2.1.6: Chokidar 2 does not receive security updates since 2019. Upgrade to chokidar 3 with 15x fewer dependencies
npm warn deprecated sntp@0.2.4: This module moved to @hapi/sntp. Please make sure to switch over as this distribution is no longer supported and may contain bugs and critical security issues.
npm warn deprecated minimatch@0.3.0: Please update to minimatch 3.0.2 or higher to avoid a RegExp DoS issue
npm warn deprecated chokidar@2.1.8: Chokidar 2 does not receive security updates since 2019. Upgrade to chokidar 3 with 15x fewer dependencies
npm warn deprecated sntp@1.0.9: This module moved to @hapi/sntp. Please make sure to switch over as this distribution is no longer supported and may contain bugs and critical security issues.
npm warn deprecated querystring@0.2.0: The querystring API is considered Legacy. new code should use the URLSearchParams API instead.
npm warn deprecated request@2.36.0: request has been deprecated, see https://github.com/request/request/issues/3142
npm warn deprecated mkdirp@0.3.0: Legacy versions of mkdirp are no longer supported. Please update to mkdirp 1.x. (Note that the API surface has changed to use Promises in 1.x.)
npm warn deprecated tough-cookie@2.2.2: ReDoS vulnerability parsing Set-Cookie https://nodesecurity.io/advisories/130
npm warn deprecated hoek@0.9.1: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated node-uuid@1.4.8: Use uuid module instead
npm warn deprecated node-uuid@1.4.8: Use uuid module instead
npm warn deprecated uuid@3.3.2: Please upgrade  to version 7 or higher.  Older versions may use Math.random() in certain circumstances, which is known to be problematic.  See https://v8.dev/blog/math-random for details.
npm warn deprecated source-map-resolve@0.5.2: See https://github.com/lydell/source-map-resolve#deprecated
npm warn deprecated har-validator@2.0.6: this library is no longer supported
npm warn deprecated mkdirp@0.5.1: Legacy versions of mkdirp are no longer supported. Please update to mkdirp 1.x. (Note that the API surface has changed to use Promises in 1.x.)
npm warn deprecated hoek@2.16.3: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated request@2.79.0: request has been deprecated, see https://github.com/request/request/issues/3142
npm warn deprecated request@2.88.0: request has been deprecated, see https://github.com/request/request/issues/3142
npm warn deprecated request@2.67.0: request has been deprecated, see https://github.com/request/request/issues/3142
npm warn deprecated readdir-scoped-modules@1.0.2: This functionality has been moved to @npmcli/fs
npm warn deprecated hawk@1.0.0: This module moved to @hapi/hawk. Please make sure to switch over as this distribution is no longer supported and may contain bugs and critical security issues.
npm warn deprecated hawk@3.1.3: This module moved to @hapi/hawk. Please make sure to switch over as this distribution is no longer supported and may contain bugs and critical security issues.
npm warn deprecated jade@0.26.3: Jade has been renamed to pug, please install the latest version of pug instead of jade
npm warn deprecated swig@1.4.2: This package is no longer maintained
npm warn deprecated bson@1.0.9: Fixed a critical issue with BSON serialization documented in CVE-2019-2391, see https://bit.ly/2KcpXdo for more details
npm warn deprecated nodeunit@0.9.5: you are strongly encouraged to use other testing options

added 962 packages, and audited 1412 packages in 11s

32 packages are looking for funding
  run `npm fund` for details

137 vulnerabilities (9 low, 35 moderate, 57 high, 36 critical)

To address issues that do not require attention, run:
  npm audit fix

To address all issues possible (including breaking changes), run:
  npm audit fix --force

Some issues need review, and may require choosing
a different dependency.

Run `npm audit` for details.
[Pipeline] }
[Pipeline] // dir
[Pipeline] }
[Pipeline] // script
[Pipeline] }
[Pipeline] // stage
[Pipeline] stage
[Pipeline] { (blackduck-security-scan)
[Pipeline] script
[Pipeline] {
[Pipeline] dir
Running in /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main@2/nodejs-npm
[Pipeline] {
[Pipeline] echo
DETECT_PROJECT_NAME will be set to: MBP_Github_BlackduckSca_Async
[Pipeline] withEnv
[Pipeline] {
[Pipeline] echo
Workspace is /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main@2
[Pipeline] security_scan
**************************** START EXECUTION OF BLACK DUCK SECURITY SCAN ****************************
[Security Scan] INFO: Jenkins Job name: MBP_Github_BlackduckSca_Async
-------------------------------- Connection to node --------------------------------
[Security Scan] INFO: Jenkins job is running on agent node remotely
-------------------------- Parameter Validation Initiated --------------------------
[Security Scan] INFO:  --- product = [BLACKDUCKSCA]
[Security Scan] INFO: Parameters for blackducksca:
[Security Scan] INFO:  --- blackducksca_waitForScan = false
[Security Scan] INFO:  --- blackducksca_token = ******************************************************************************
[Security Scan] INFO:  --- blackducksca_url = https://saastest.app.blackduck.com
[Security Scan] INFO:  --- detect_args = detect.source.path=${WORKSPACE}/nodejs-npm
------------------------------------------------------------------------------------
[Security Scan] INFO: Parameters for additional configuration:
[Security Scan] INFO:  --- network_airgap = false
[Security Scan] INFO: Black Duck SCA parameters are validated successfully
[Security Scan] INFO: Bridge download parameters are validated successfully
[Security Scan] INFO: Bridge download is not required. Found installed in: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm
------------------------------------------------------------------------------------
[Security Scan] INFO: Bridge CLI version is - 3.9.2
[Security Scan] INFO: Jenkins Job name: MBP_Github_BlackduckSca_Async
[Security Scan] INFO: Jenkins Job name: MBP_Github_BlackduckSca_Async
[Security Scan] INFO: Executable command line arguments: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm/bridge-cli --stage blackducksca --input /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main@2/blackducksca_input17841805286727654735.json --out .bridge/output/scan_info_out.json

******************************* START EXECUTION OF BRIDGE CLI *******************************
2025-11-11 18:15:51.6378 IST [Bridge CLI] INFO: Using cache directory: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm
2025-11-11 18:15:51.6551 IST [Bridge CLI] INFO: Found version "3.0.143" in registry for workflow "blackducksca", trying to load it from local cache
2025-11-11 18:15:51.7486 IST [Bridge CLI] INFO: Input Resources:
2025-11-11 18:15:51.7487 IST [Bridge CLI] INFO: resource = value [source]
2025-11-11 18:15:51.7487 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-11 18:15:51.7487 IST [Bridge CLI] INFO: blackducksca.token = ***************************************** [blackducksca_input17841805286727654735.json]
2025-11-11 18:15:51.7487 IST [Bridge CLI] INFO: blackducksca.url = https://saastest.app.blackduck.com [blackducksca_input17841805286727654735.json]
2025-11-11 18:15:51.7487 IST [Bridge CLI] INFO: blackducksca.waitForScan = false [blackducksca_input17841805286727654735.json]
2025-11-11 18:15:51.7487 IST [Bridge CLI] INFO: detect.args = detect.source.path=${WORKSPACE}/nodejs-npm [blackducksca_input17841805286727654735.json]
2025-11-11 18:15:51.7487 IST [Bridge CLI] INFO: network.airgap = false [blackducksca_input17841805286727654735.json]
2025-11-11 18:15:51.7487 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-11 18:15:51.7487 IST [Bridge CLI] INFO: Starting adapters for stage blackducksca
2025-11-11 18:15:51.7490 IST [Bridge CLI] INFO: Starting Adapter: Blackduck SCA Controller
2025-11-11 18:15:51.7536 IST [Bridge CLI] INFO: Starting Adapter: Default Black Duck SCA Scan Mode
2025-11-11 18:15:51.7576 IST [Bridge CLI] INFO: Starting Adapter: Check pull request
2025-11-11 18:15:51.7824 IST [Check pull request] INFO: Provided value for resource 'environment.scan.pull'
2025-11-11 18:15:51.7826 IST [Check pull request] INFO: Adapter finished
2025-11-11 18:15:51.7981 IST [Default Black Duck SCA Scan Mode] INFO: Provided value for resource 'blackducksca.scan.full'
2025-11-11 18:15:51.7983 IST [Default Black Duck SCA Scan Mode] INFO: Adapter finished
2025-11-11 18:15:52.6487 IST [Blackduck SCA Controller] INFO: Found Black Duck SCA Detect jar file "detect-11.0.0.jar" in "/Users/madhusud/.blackduck/bridge/tools/blackduck-detect/11.0.0"
2025-11-11 18:15:52.6490 IST [Blackduck SCA Controller] INFO: Scan is configured to run asynchronously, will not wait for the scan to complete.
2025-11-11 18:15:52.6490 IST [Blackduck SCA Controller] WARNING: 'blackducksca.waitForScan' is set to false, will skip any post scan features if configured.
2025-11-11 18:15:52.6541 IST [Blackduck SCA Controller] INFO: Provided value for resource 'detect.execution.path'
2025-11-11 18:15:52.6542 IST [Bridge CLI] INFO: Starting adapters for stage blackducksca-detect
2025-11-11 18:15:52.6550 IST [Bridge CLI] INFO: Starting Adapter: Blackduck SCA Detect Execution
2025-11-11 18:15:52.6552 IST [Blackduck SCA Controller] INFO: Adapter finished
2025-11-11 18:15:52.6887 IST [Blackduck SCA Detect Execution] INFO: Running command /Library/Java/JavaVirtualMachines/jdk-21.jdk/Contents/Home/bin/java -jar /Users/madhusud/.blackduck/bridge/tools/blackduck-detect/11.0.0/detect-11.0.0.jar --detect.cleanup=false --detect.bdio.file.name=scan --detect.bdio.output.path=/Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main@2/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/bdio/blackduck_artifact --detect.output.path=/Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main@2/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect --blackduck.offline.mode=false --blackduck.url=https://saastest.app.blackduck.com --blackduck.api.token= --detect.blackduck.scan.mode=INTELLIGENT detect.source.path=${WORKSPACE}/nodejs-npm
2025-11-11 18:15:53.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Detect-Self-Updater:  Checking https://saastest.app.blackduck.com/api/tools/detect API for centrally managed Detect version to download to /Users/madhusud/tmp.
2025-11-11 18:15:55.0000 IST [Blackduck SCA Detect Execution][main] WARNING: --- Detect-Self-Updater:  Unable to download jar from https://saastest.app.blackduck.com/api/tools/detect.
2025-11-11 18:15:55.0000 IST [Blackduck SCA Detect Execution][main] WARNING: --- Detect-Self-Updater:  Response code from https://saastest.app.blackduck.com/api/tools/detect was: 400 Bad Request
2025-11-11 18:15:55.6681 IST [Blackduck SCA Detect Execution] INFO: ______     _            _
2025-11-11 18:15:55.6682 IST [Blackduck SCA Detect Execution] INFO: |  _  \   | |          | |
2025-11-11 18:15:55.6682 IST [Blackduck SCA Detect Execution] INFO: | | | |___| |_ ___  ___| |_
2025-11-11 18:15:55.6682 IST [Blackduck SCA Detect Execution] INFO: | | | / _ \ __/ _ \/ __| __|
2025-11-11 18:15:55.6682 IST [Blackduck SCA Detect Execution] INFO: | |/ /  __/ ||  __/ (__| |_
2025-11-11 18:15:55.6682 IST [Blackduck SCA Detect Execution] INFO: |___/ \___|\__\___|\___|\__|
2025-11-11 18:15:55.6682 IST [Blackduck SCA Detect Execution] INFO: 
2025-11-11 18:15:55.7483 IST [Blackduck SCA Detect Execution] INFO: 
2025-11-11 18:15:55.7483 IST [Blackduck SCA Detect Execution] INFO: Detect Version: 11.0.0
2025-11-11 18:15:55.7483 IST [Blackduck SCA Detect Execution] INFO: 
2025-11-11 18:15:55.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 18:15:55.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Current property values:
2025-11-11 18:15:55.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- --property = value [notes]
2025-11-11 18:15:55.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ------------------------------------------------------------
2025-11-11 18:15:55.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- blackduck.api.token = **************************************************************************************************** [cmd] 
2025-11-11 18:15:55.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- blackduck.offline.mode = false [cmd] 
2025-11-11 18:15:55.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- blackduck.url = https://saastest.app.blackduck.com [cmd] 
2025-11-11 18:15:55.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- detect.bdio.file.name = scan [cmd] 
2025-11-11 18:15:55.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- detect.bdio.output.path = /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main@2/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/bdio/blackduck_artifact [cmd] 
2025-11-11 18:15:55.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- detect.blackduck.scan.mode = INTELLIGENT [cmd] 
2025-11-11 18:15:55.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- detect.cleanup = false [cmd] 
2025-11-11 18:15:55.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- detect.excluded.directories = /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main@2/nodejs-npm/.bridge [env] 
2025-11-11 18:15:55.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- detect.output.path = /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main@2/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect [cmd] 
2025-11-11 18:15:55.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- detect.project.name = MBP_Github_BlackduckSca_Async [env] 
2025-11-11 18:15:55.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ------------------------------------------------------------
2025-11-11 18:15:55.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 18:15:55.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Detect build date: 2025-10-30
2025-11-11 18:15:55.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Source directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main@2/nodejs-npm
2025-11-11 18:15:55.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Output directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main@2/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect
2025-11-11 18:15:55.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Run directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main@2/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/runs/2025-11-11-12-45-55-741
2025-11-11 18:15:55.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 18:16:01.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Successfully connected to Black Duck SCA (version 2025.7.1)!
2025-11-11 18:16:02.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-11 18:16:02.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Will include the Docker tool.
2025-11-11 18:16:02.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Docker actions finished.
2025-11-11 18:16:02.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-11 18:16:02.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Will include the Bazel tool.
2025-11-11 18:16:02.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Bazel actions finished.
2025-11-11 18:16:02.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-11 18:16:02.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Will include the Detectors tool.
2025-11-11 18:16:02.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Searching for detectors.
2025-11-11 18:16:02.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Evaluating detectors. This may take a while.
2025-11-11 18:16:02.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ======================================================================================================
2025-11-11 18:16:02.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Detector Report
2025-11-11 18:16:02.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ======================================================================================================
2025-11-11 18:16:02.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 	/Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main@2/nodejs-npm (depth 0)
2025-11-11 18:16:02.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 		NPM Package Lock: SUCCESS
2025-11-11 18:16:02.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 			Found file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main@2/nodejs-npm/package-lock.json
2025-11-11 18:16:02.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 			Found file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main@2/nodejs-npm/package.json
2025-11-11 18:16:02.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-11 18:16:02.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Detectors actions finished.
2025-11-11 18:16:02.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-11 18:16:02.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Project name: MBP_Github_BlackduckSca_Async
2025-11-11 18:16:02.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Project version: 1.3.0
2025-11-11 18:16:06.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Successfully completed package manager scan of file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main@2/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/bdio/blackduck_artifact/scan.bdio
2025-11-11 18:16:08.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Starting the codelocation file uploads.
2025-11-11 18:16:12.0000 IST [Blackduck SCA Detect Execution][pool-1-thread-1] INFO: --- Try #1 for task bdio upload (elapsed: 00:00:00.000)...complete!
2025-11-11 18:16:12.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Completed the codelocation file uploads.
2025-11-11 18:16:12.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-11 18:16:12.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Will include the Signature Scanner tool.
2025-11-11 18:16:12.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- No metadata file exists, assuming this is new installation and the signature scanner should be downloaded.
2025-11-11 18:16:14.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Downloading the Black Duck Signature Scanner.
2025-11-11 18:16:14.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- If the Signature Scanner on your Black Duck server has changed, the contents of /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main@2/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/tools/Black_Duck_Scan_Installation may change which could involve deleting files - please do not place items in the expansion directory as this directory is assumed to be under blackduck-common control.
2025-11-11 18:16:22.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Black Duck Signature Scanner downloaded successfully.
2025-11-11 18:16:22.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- The Black Duck Signature Scanner downloaded/found successfully: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main@2/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/tools
2025-11-11 18:16:22.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- No scan targets provided - registering the source path /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main@2/nodejs-npm to scan
2025-11-11 18:16:24.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Starting the Black Duck Signature Scan commands.
2025-11-11 18:16:24.0000 IST [Blackduck SCA Detect Execution][pool-3-thread-1] INFO: --- Black Duck CLI command: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main@2/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/tools/Black_Duck_Scan_Installation/scan.cli-1.0.6/jre/Contents/Home/bin/java -Done-jar.silent=true -Done-jar.jar.path=/Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main@2/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/tools/Black_Duck_Scan_Installation/scan.cli-1.0.6/lib/cache/scan.cli.impl-standalone.jar -Xmx4096m -jar /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main@2/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/tools/Black_Duck_Scan_Installation/scan.cli-1.0.6/lib/scan.cli-1.0.6-standalone.jar --no-prompt --scheme https --host saastest.app.blackduck.com --port 443 -v --logDir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main@2/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/runs/2025-11-11-12-45-55-741/scan/BlackDuckScanOutput/2025-11-11_12-46-24-691_1 --statusWriteDir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main@2/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/runs/2025-11-11-12-45-55-741/scan/BlackDuckScanOutput/2025-11-11_12-46-24-691_1 --project MBP_Github_BlackduckSca_Async --release 1.3.0 --name nodejs-npm/MBP_Github_BlackduckSca_Async/1.3.0 signature --exclude /node_modules/ --exclude /.bridge/ --scass-scan /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main@2/nodejs-npm
2025-11-11 18:16:36.0000 IST [Blackduck SCA Detect Execution][pool-3-thread-1] INFO: --- 
2025-11-11 18:16:36.0000 IST [Blackduck SCA Detect Execution][pool-3-thread-1] INFO: --- Black Duck Signature Scanner return code: 0
2025-11-11 18:16:36.0000 IST [Blackduck SCA Detect Execution][pool-3-thread-1] INFO: --- Signature Scanner log output directory: '/Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main@2/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/runs/2025-11-11-12-45-55-741/scan/BlackDuckScanOutput/2025-11-11_12-46-24-691_1'
2025-11-11 18:16:36.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Completed the Black Duck Signature Scan commands.
2025-11-11 18:16:36.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Signature Scanner actions finished.
2025-11-11 18:16:36.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-11 18:16:36.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Will include the Binary Scanner tool.
2025-11-11 18:16:36.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Binary scanner found nothing to upload.
2025-11-11 18:16:36.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Binary Scanner actions finished.
2025-11-11 18:16:36.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-11 18:16:36.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Will include the Container Scanner tool.
2025-11-11 18:16:36.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- No detect.container.scan.file.path property was provided. Skipping container scan.
2025-11-11 18:16:36.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Container Scanner actions finished.
2025-11-11 18:16:36.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-11 18:16:36.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Vulnerability Impact Analysis tool will not be run.
2025-11-11 18:16:36.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-11 18:16:36.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- IaC Scanner tool will not be run.
2025-11-11 18:16:36.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-11 18:16:36.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Checking to see if Detect should check policy for violations.
2025-11-11 18:16:37.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 18:16:37.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 18:16:37.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Creating status file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main@2/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/runs/2025-11-11-12-45-55-741/status/status.json
2025-11-11 18:16:37.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 18:16:37.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Skipping cleanup, it is disabled.
2025-11-11 18:16:38.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 18:16:38.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 18:16:38.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ======== Detect Result ========
2025-11-11 18:16:38.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 18:16:38.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Black Duck SCA Project BOM: https://saastest.app.blackduck.com/api/projects/c9772f41-effb-4436-bf2b-6352c5f20644/versions/4b2bd363-ea54-4c30-bf11-c44b3fca3a6c/components
2025-11-11 18:16:38.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 18:16:38.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ======== Detect Status ========
2025-11-11 18:16:38.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 18:16:38.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- NPM: SUCCESS
2025-11-11 18:16:38.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 18:16:38.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Signature scan / Snippet scan on /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main@2/nodejs-npm: SUCCESS
2025-11-11 18:16:38.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Overall Status: SUCCESS - Detect exited successfully.
2025-11-11 18:16:38.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 18:16:38.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ===============================
2025-11-11 18:16:38.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-11 18:16:38.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Detect duration: 00h 00m 45s 392ms
2025-11-11 18:16:38.6139 IST [Blackduck SCA Detect Execution] INFO: Provided value for resource 'detect.completed'
2025-11-11 18:16:38.6140 IST [Blackduck SCA Detect Execution] INFO: Provided value for resource 'detect.results.path'
2025-11-11 18:16:38.6143 IST [Blackduck SCA Detect Execution] INFO: Adapter finished
******************************* END EXECUTION OF BRIDGE CLI *******************************
[Security Scan] INFO: Retrieving the issue count from the scan results
[Security Scan] INFO: Issue count not found in output file
[Security Scan] INFO: Security Scan execution is successful
**************************** END EXECUTION OF BLACK DUCK SECURITY SCAN ****************************
[Pipeline] }
[Pipeline] // withEnv
[Pipeline] }
[Pipeline] // dir
[Pipeline] }
[Pipeline] // script
[Pipeline] }
[Pipeline] // stage
[Pipeline] stage
[Pipeline] { (Declarative: Post Actions)
[Pipeline] echo
Black Duck Logs Publisher - Starting log upload process
[Pipeline] echo
Configuration: [githubOrg:blackducksca-jenkins-samples, repoName:async-mode, credentialsId:github-pat-logs-publisher, maxRetries:3, retentionCount:5, jobNamePrefixes:[MBP_Github_, MBP_, Github_, Pipeline_, Job_, Build_]]
[Pipeline] echo
Job Name: MBP_Github_BlackduckSca_Async/main
[Pipeline] echo
Build Number: 2
[Pipeline] echo
GitHub Organization: blackducksca-jenkins-samples
[Pipeline] withCredentials
Masking supported pattern matches of $GITHUB_TOKEN
[Pipeline] {
[Pipeline] echo
Using configured repository name: async-mode
[Pipeline] echo
Target repository: blackducksca-jenkins-samples/async-mode
[Pipeline] echo
LogProcessor: captureJenkinsLogs called
```

---

*Log generated by Black Duck Logs Publisher*