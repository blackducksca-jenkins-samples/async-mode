# Jenkins Execution Log

## Build Information
- **Job Name:** `MBP_Github_BlackduckSca_Async/main`
- **Build Number:** #3
- **Build Status:** 🟢 **SUCCESS**
- **Duration:** 1 min 40 sec and counting
- **Timestamp:** 2025-11-16 22:34:36 UTC

---

## Console Output

```
Started by user admin
Connecting to https://api.github.com using madhusud@blackduck.com/****** (Github_Username_PAT)
Obtained nodejs-npm/Jenkinsfile from 3491a204c8a650f0b0d1c1dfe154b6992fc2d950
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
Running on mac-sh in /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Declarative: Checkout SCM)
[Pipeline] checkout
The recommended git tool is: NONE
using credential Github_Username_PAT
Fetching changes from the remote Git repository
Fetching without tags
 > git rev-parse --resolve-git-dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main/.git # timeout=10
 > git config remote.origin.url https://github.com/blackducksca-jenkins-samples/async-mode.git # timeout=10
Fetching upstream changes from https://github.com/blackducksca-jenkins-samples/async-mode.git
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git fetch --no-tags --force --progress -- https://github.com/blackducksca-jenkins-samples/async-mode.git +refs/heads/main:refs/remotes/origin/main # timeout=10
Checking out Revision 3491a204c8a650f0b0d1c1dfe154b6992fc2d950 (main)
Commit message: "Delete jenkins-logs directory"
 > git config core.sparsecheckout # timeout=10
 > git checkout -f 3491a204c8a650f0b0d1c1dfe154b6992fc2d950 # timeout=10
 > git rev-list --no-walk 79b0f386dfac1c093b46bb149fc9d2d87e65b5b6 # timeout=10
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
Running in /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main/nodejs-npm
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

up to date, audited 1412 packages in 23s

32 packages are looking for funding
  run `npm fund` for details

137 vulnerabilities (9 low, 38 moderate, 55 high, 35 critical)

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
Running in /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main/nodejs-npm
[Pipeline] {
[Pipeline] echo
DETECT_PROJECT_NAME will be set to: MBP_Github_BlackduckSca_Async
[Pipeline] withEnv
[Pipeline] {
[Pipeline] echo
Workspace is /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main
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
[Security Scan] INFO:  --- network_ssl_trustAll = false
[Security Scan] INFO:  --- network_airgap = false
[Security Scan] INFO: Black Duck SCA parameters are validated successfully
[Security Scan] INFO: Bridge download parameters are validated successfully
[Security Scan] INFO: Bridge download is not required. Found installed in: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm
------------------------------------------------------------------------------------
[Security Scan] INFO: Bridge CLI version is - 3.9.2
[Security Scan] INFO: Jenkins Job name: MBP_Github_BlackduckSca_Async
[Security Scan] INFO: Jenkins Job name: MBP_Github_BlackduckSca_Async
[Security Scan] INFO: Executable command line arguments: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm/bridge-cli --stage blackducksca --input /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main/blackducksca_input17997203775186675050.json --out .bridge/output/scan_info_out.json

******************************* START EXECUTION OF BRIDGE CLI *******************************
2025-11-16 22:33:37.5083 IST [Bridge CLI] INFO: Using cache directory: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm
2025-11-16 22:33:37.5200 IST [Bridge CLI] INFO: Found version "3.0.143" in registry for workflow "blackducksca", trying to load it from local cache
2025-11-16 22:33:37.6144 IST [Bridge CLI] INFO: Input Resources:
2025-11-16 22:33:37.6144 IST [Bridge CLI] INFO: resource = value [source]
2025-11-16 22:33:37.6144 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-16 22:33:37.6145 IST [Bridge CLI] INFO: blackducksca.token = ***************************************** [blackducksca_input17997203775186675050.json]
2025-11-16 22:33:37.6145 IST [Bridge CLI] INFO: blackducksca.url = https://saastest.app.blackduck.com [blackducksca_input17997203775186675050.json]
2025-11-16 22:33:37.6146 IST [Bridge CLI] INFO: blackducksca.waitForScan = false [blackducksca_input17997203775186675050.json]
2025-11-16 22:33:37.6146 IST [Bridge CLI] INFO: detect.args = detect.source.path=${WORKSPACE}/nodejs-npm [blackducksca_input17997203775186675050.json]
2025-11-16 22:33:37.6146 IST [Bridge CLI] INFO: network.airgap = false [blackducksca_input17997203775186675050.json]
2025-11-16 22:33:37.6146 IST [Bridge CLI] INFO: network.ssl.trustAll = false [blackducksca_input17997203775186675050.json]
2025-11-16 22:33:37.6146 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-16 22:33:37.6147 IST [Bridge CLI] INFO: Starting adapters for stage blackducksca
2025-11-16 22:33:37.6150 IST [Bridge CLI] INFO: Starting Adapter: Blackduck SCA Controller
2025-11-16 22:33:37.6194 IST [Bridge CLI] INFO: Starting Adapter: Default Black Duck SCA Scan Mode
2025-11-16 22:33:37.6236 IST [Bridge CLI] INFO: Starting Adapter: Check pull request
2025-11-16 22:33:37.6519 IST [Check pull request] INFO: Provided value for resource 'environment.scan.pull'
2025-11-16 22:33:37.6520 IST [Check pull request] INFO: Adapter finished
2025-11-16 22:33:37.6780 IST [Default Black Duck SCA Scan Mode] INFO: Provided value for resource 'blackducksca.scan.full'
2025-11-16 22:33:37.6783 IST [Default Black Duck SCA Scan Mode] INFO: Adapter finished
2025-11-16 22:33:38.7012 IST [Blackduck SCA Controller] INFO: Found Black Duck SCA Detect jar file "detect-11.0.0.jar" in "/Users/madhusud/.blackduck/bridge/tools/blackduck-detect/11.0.0"
2025-11-16 22:33:38.7025 IST [Blackduck SCA Controller] INFO: Scan is configured to run asynchronously, will not wait for the scan to complete.
2025-11-16 22:33:38.7025 IST [Blackduck SCA Controller] WARNING: 'blackducksca.waitForScan' is set to false, will skip any post scan features if configured.
2025-11-16 22:33:38.7387 IST [Blackduck SCA Controller] INFO: Provided value for resource 'detect.execution.path'
2025-11-16 22:33:38.7388 IST [Bridge CLI] INFO: Starting adapters for stage blackducksca-detect
2025-11-16 22:33:38.7393 IST [Bridge CLI] INFO: Starting Adapter: Blackduck SCA Detect Execution
2025-11-16 22:33:38.7395 IST [Blackduck SCA Controller] INFO: Adapter finished
2025-11-16 22:33:38.7921 IST [Blackduck SCA Detect Execution] INFO: Running command /Library/Java/JavaVirtualMachines/jdk-21.jdk/Contents/Home/bin/java -jar /Users/madhusud/.blackduck/bridge/tools/blackduck-detect/11.0.0/detect-11.0.0.jar --detect.cleanup=false --detect.bdio.file.name=scan --detect.bdio.output.path=/Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/bdio/blackduck_artifact --detect.output.path=/Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect --blackduck.offline.mode=false --blackduck.url=https://saastest.app.blackduck.com --blackduck.api.token= --detect.blackduck.scan.mode=INTELLIGENT detect.source.path=${WORKSPACE}/nodejs-npm
2025-11-16 22:33:39.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Detect-Self-Updater:  Checking https://saastest.app.blackduck.com/api/tools/detect API for centrally managed Detect version to download to /Users/madhusud/tmp.
2025-11-16 22:33:42.0000 IST [Blackduck SCA Detect Execution][main] WARNING: --- Detect-Self-Updater:  Unable to download jar from https://saastest.app.blackduck.com/api/tools/detect.
2025-11-16 22:33:42.0000 IST [Blackduck SCA Detect Execution][main] WARNING: --- Detect-Self-Updater:  Response code from https://saastest.app.blackduck.com/api/tools/detect was: 400 Bad Request
2025-11-16 22:33:43.5738 IST [Blackduck SCA Detect Execution] INFO: ______     _            _
2025-11-16 22:33:43.5738 IST [Blackduck SCA Detect Execution] INFO: |  _  \   | |          | |
2025-11-16 22:33:43.5739 IST [Blackduck SCA Detect Execution] INFO: | | | |___| |_ ___  ___| |_
2025-11-16 22:33:43.5739 IST [Blackduck SCA Detect Execution] INFO: | | | / _ \ __/ _ \/ __| __|
2025-11-16 22:33:43.5739 IST [Blackduck SCA Detect Execution] INFO: | |/ /  __/ ||  __/ (__| |_
2025-11-16 22:33:43.5739 IST [Blackduck SCA Detect Execution] INFO: |___/ \___|\__\___|\___|\__|
2025-11-16 22:33:43.5740 IST [Blackduck SCA Detect Execution] INFO: 
2025-11-16 22:33:43.6662 IST [Blackduck SCA Detect Execution] INFO: 
2025-11-16 22:33:43.6663 IST [Blackduck SCA Detect Execution] INFO: Detect Version: 11.0.0
2025-11-16 22:33:43.6663 IST [Blackduck SCA Detect Execution] INFO: 
2025-11-16 22:33:43.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-16 22:33:43.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Current property values:
2025-11-16 22:33:43.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- --property = value [notes]
2025-11-16 22:33:43.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ------------------------------------------------------------
2025-11-16 22:33:43.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- blackduck.api.token = **************************************************************************************************** [cmd] 
2025-11-16 22:33:43.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- blackduck.offline.mode = false [cmd] 
2025-11-16 22:33:43.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- blackduck.url = https://saastest.app.blackduck.com [cmd] 
2025-11-16 22:33:43.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- detect.bdio.file.name = scan [cmd] 
2025-11-16 22:33:43.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- detect.bdio.output.path = /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/bdio/blackduck_artifact [cmd] 
2025-11-16 22:33:43.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- detect.blackduck.scan.mode = INTELLIGENT [cmd] 
2025-11-16 22:33:43.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- detect.cleanup = false [cmd] 
2025-11-16 22:33:43.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- detect.excluded.directories = /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main/nodejs-npm/.bridge [env] 
2025-11-16 22:33:43.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- detect.output.path = /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect [cmd] 
2025-11-16 22:33:43.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- detect.project.name = MBP_Github_BlackduckSca_Async [env] 
2025-11-16 22:33:43.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ------------------------------------------------------------
2025-11-16 22:33:43.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-16 22:33:43.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Detect build date: 2025-10-30
2025-11-16 22:33:43.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Source directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main/nodejs-npm
2025-11-16 22:33:43.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Output directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect
2025-11-16 22:33:43.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Run directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/runs/2025-11-16-17-03-43-658
2025-11-16 22:33:43.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-16 22:33:50.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Successfully connected to Black Duck SCA (version 2025.10.0)!
2025-11-16 22:33:52.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-16 22:33:52.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Will include the Docker tool.
2025-11-16 22:33:52.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Docker actions finished.
2025-11-16 22:33:52.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-16 22:33:52.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Will include the Bazel tool.
2025-11-16 22:33:52.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Bazel actions finished.
2025-11-16 22:33:52.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-16 22:33:52.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Will include the Detectors tool.
2025-11-16 22:33:52.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Searching for detectors.
2025-11-16 22:33:52.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Evaluating detectors. This may take a while.
2025-11-16 22:33:52.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ======================================================================================================
2025-11-16 22:33:52.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Detector Report
2025-11-16 22:33:52.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ======================================================================================================
2025-11-16 22:33:52.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 	/Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main/nodejs-npm (depth 0)
2025-11-16 22:33:52.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 		NPM Package Lock: SUCCESS
2025-11-16 22:33:52.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 			Found file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main/nodejs-npm/package-lock.json
2025-11-16 22:33:52.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 			Found file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main/nodejs-npm/package.json
2025-11-16 22:33:52.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-16 22:33:52.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Detectors actions finished.
2025-11-16 22:33:52.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-16 22:33:52.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Project name: MBP_Github_BlackduckSca_Async
2025-11-16 22:33:52.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Project version: 1.3.0
2025-11-16 22:33:56.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Successfully completed package manager scan of file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/bdio/blackduck_artifact/scan.bdio
2025-11-16 22:33:58.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Starting the codelocation file uploads.
2025-11-16 22:34:04.0000 IST [Blackduck SCA Detect Execution][pool-1-thread-1] INFO: --- Try #1 for task bdio upload (elapsed: 00:00:00.000)...complete!
2025-11-16 22:34:04.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Completed the codelocation file uploads.
2025-11-16 22:34:04.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-16 22:34:04.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Will include the Signature Scanner tool.
2025-11-16 22:34:07.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- The signature scanner should be downloaded. Locally installed signature scanner is 1.0.6, but the latest version is 1.0.7
2025-11-16 22:34:07.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Downloading the Black Duck Signature Scanner.
2025-11-16 22:34:07.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- If the Signature Scanner on your Black Duck server has changed, the contents of /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/tools/Black_Duck_Scan_Installation may change which could involve deleting files - please do not place items in the expansion directory as this directory is assumed to be under blackduck-common control.
2025-11-16 22:34:14.0000 IST [Blackduck SCA Detect Execution][main] WARNING: --- There were items in /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/tools/Black_Duck_Scan_Installation that are being deleted. This may happen under normal conditions, but please do not place items in the expansion directory as this directory is assumed to be under the integration's control.
2025-11-16 22:34:17.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Black Duck Signature Scanner downloaded successfully.
2025-11-16 22:34:17.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- The Black Duck Signature Scanner downloaded/found successfully: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/tools
2025-11-16 22:34:17.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- No scan targets provided - registering the source path /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main/nodejs-npm to scan
2025-11-16 22:34:19.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Starting the Black Duck Signature Scan commands.
2025-11-16 22:34:19.0000 IST [Blackduck SCA Detect Execution][pool-3-thread-1] INFO: --- Black Duck CLI command: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/tools/Black_Duck_Scan_Installation/scan.cli-1.0.7/jre/Contents/Home/bin/java -Done-jar.silent=true -Done-jar.jar.path=/Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/tools/Black_Duck_Scan_Installation/scan.cli-1.0.7/lib/cache/scan.cli.impl-standalone.jar -Xmx4096m -jar /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/tools/Black_Duck_Scan_Installation/scan.cli-1.0.7/lib/scan.cli-1.0.7-standalone.jar --no-prompt --scheme https --host saastest.app.blackduck.com --port 443 -v --logDir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/runs/2025-11-16-17-03-43-658/scan/BlackDuckScanOutput/2025-11-16_17-04-19-055_1 --statusWriteDir /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/runs/2025-11-16-17-03-43-658/scan/BlackDuckScanOutput/2025-11-16_17-04-19-055_1 --project MBP_Github_BlackduckSca_Async --release 1.3.0 --name nodejs-npm/MBP_Github_BlackduckSca_Async/1.3.0 signature --exclude /node_modules/ --exclude /.bridge/ --scass-scan /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main/nodejs-npm
2025-11-16 22:34:33.0000 IST [Blackduck SCA Detect Execution][pool-3-thread-1] INFO: --- 
2025-11-16 22:34:33.0000 IST [Blackduck SCA Detect Execution][pool-3-thread-1] INFO: --- Black Duck Signature Scanner return code: 0
2025-11-16 22:34:33.0000 IST [Blackduck SCA Detect Execution][pool-3-thread-1] INFO: --- Signature Scanner log output directory: '/Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/runs/2025-11-16-17-03-43-658/scan/BlackDuckScanOutput/2025-11-16_17-04-19-055_1'
2025-11-16 22:34:33.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Completed the Black Duck Signature Scan commands.
2025-11-16 22:34:33.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Signature Scanner actions finished.
2025-11-16 22:34:33.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-16 22:34:33.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Will include the Binary Scanner tool.
2025-11-16 22:34:33.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Binary scanner found nothing to upload.
2025-11-16 22:34:33.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Binary Scanner actions finished.
2025-11-16 22:34:33.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-16 22:34:33.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Will include the Container Scanner tool.
2025-11-16 22:34:33.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- No detect.container.scan.file.path property was provided. Skipping container scan.
2025-11-16 22:34:33.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Container Scanner actions finished.
2025-11-16 22:34:33.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-16 22:34:33.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Vulnerability Impact Analysis tool will not be run.
2025-11-16 22:34:33.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-16 22:34:33.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- IaC Scanner tool will not be run.
2025-11-16 22:34:33.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ----------------------------------
2025-11-16 22:34:33.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Checking to see if Detect should check policy for violations.
2025-11-16 22:34:34.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-16 22:34:34.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-16 22:34:34.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Creating status file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main/nodejs-npm/.bridge/blackduck_sca_detect_execution/detect/runs/2025-11-16-17-03-43-658/status/status.json
2025-11-16 22:34:34.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-16 22:34:34.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Skipping cleanup, it is disabled.
2025-11-16 22:34:35.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-16 22:34:35.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-16 22:34:35.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ======== Detect Result ========
2025-11-16 22:34:35.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-16 22:34:35.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Black Duck SCA Project BOM: https://saastest.app.blackduck.com/api/projects/c9772f41-effb-4436-bf2b-6352c5f20644/versions/4b2bd363-ea54-4c30-bf11-c44b3fca3a6c/components
2025-11-16 22:34:35.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-16 22:34:35.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ======== Detect Status ========
2025-11-16 22:34:35.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-16 22:34:35.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- NPM: SUCCESS
2025-11-16 22:34:35.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-16 22:34:35.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Signature scan / Snippet scan on /Users/madhusud/Jenkins_Testing/Nodes/workspace/P_Github_BlackduckSca_Async_main/nodejs-npm: SUCCESS
2025-11-16 22:34:35.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Overall Status: SUCCESS - Detect exited successfully.
2025-11-16 22:34:35.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-16 22:34:35.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- ===============================
2025-11-16 22:34:35.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- 
2025-11-16 22:34:35.0000 IST [Blackduck SCA Detect Execution][main] INFO: --- Detect duration: 00h 00m 56s 498ms
2025-11-16 22:34:35.8268 IST [Blackduck SCA Detect Execution] INFO: Provided value for resource 'detect.completed'
2025-11-16 22:34:35.8269 IST [Blackduck SCA Detect Execution] INFO: Provided value for resource 'detect.results.path'
2025-11-16 22:34:35.8272 IST [Blackduck SCA Detect Execution] INFO: Adapter finished
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
Build Number: 3
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