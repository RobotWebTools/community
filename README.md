# ROS WebTools Working Group

This document defines the scope and governance of the ROS WebTools Working Group (WG).

The WebTools Working Group's mission is to provide high quality integrations for ROS and ROS 2 to the browser / web-development space.
Its core focus is to enable developers to easily create browser and server applications to monitor and control ROS-based robotic and simulation applications.

The scope of this working group includes language clients for the browser and the server, the bridge communication protocol, and basic web components to help kickstart more complex applications.

## Subprojects

This Working Group owns and maintains the following Subprojects.
Its meetings and membership are largely focused on the direction, design, and work on the projects.

### Subproject List

The following subprojects are owned by the Working Group:

* Organization Infrastructure
  * Description: Repositories to manage the working group itself - these are not products for users
  * Repositories:
    * https://github.com/RobotWebTools/community
    * https://github.com/RobotWebTools/robotwebtools.github.io
    * https://github.com/RobotWebTools/starter-template
    * https://github.com/RobotWebTools/rwt_dockers
    * https://github.com/RobotWebTools/robot_web_tools
* `roslibjs`
  * Description: ROS 1 Javascript language client - for use in the browser
  * Repositories:
    * https://github.com/RobotWebTools/roslibjs
    * https://github.com/RobotWebTools/roslibjs_integration_tests
* `rclnodejs`
  * Description: ROS 2 native NodeJS client
  * Repositories
    * https://github.com/RobotWebTools/rclnodejs
    * https://github.com/RobotWebTools/rclnodejs-cli
* Rosbridge protocol
  * Description: A protocol and tools for passing ROS messages to and from web applications
  * Repositories:
    * https://github.com/RobotWebTools/ros2-web-bridge
    * https://github.com/RobotWebTools/rosbridge_suite
* Visualization components
  * Description: Common web components/libraries for building ROS visualizers
  * Repositories:
    * https://github.com/RobotWebTools/ros3djs
    * https://github.com/RobotWebTools/ros2djs
    * https://github.com/RobotWebTools/interactive_marker_proxy
* Specific Data Streaming
  * Description: Libraries for streaming ROS data effectively
  * Repositories:
    * https://github.com/RobotWebTools/web_video_server
    * https://github.com/RobotWebTools/tf2_web_republisher
    * https://github.com/RobotWebTools/webrtc_ros
    * https://github.com/RobotWebTools/ros_web_video
    * https://github.com/RobotWebTools/mjpeg_server
    * https://github.com/RobotWebTools/depthcloud_encoder

### Standards for subprojects

Subprojects must meet the following criteria (and the WG agrees to maintain them upon adoption).

* Build passes against ROS 2 master
* The ROS 2 standard linter set is enabled and adhered to
* If packages are part of nightly builds on the ROS build farm, there are no reported warnings or test failures
* Quality builds are green (address sanitizer, thread sanitizer, clang thread safety analysis)
* Test suite passes
* Code coverage is measured, and non-decreasing level is enforced in PRs
* Issues and pull requests receive prompt responses
* Releases go out regularly when bugfixes or new features are introduced
* The backlog is maintained, avoiding longstanding stale issues

### Adding new subprojects

To request introduction of a new subproject, add a list item to the "Subprojects" section and open a Pull Request to this repository, following the default Pull Request Template to populate the text of the PR.

PR will be merged on unanimous approval from Approvers.

### Subproject changes

Modify the relevant list item in the "Subprojects" section and open a Pull Request to this repository, following the default Pull Request Template to populate the text of the PR.

PR will be merged on unanimous approval from Approvers.

### Deprecating subprojects

Projects cease to be useful, or the WG can decide it is no longer in their interest to maintain.
We do not commit to maintaining every subproject in perpetuity.

To suggest removal of a subproject, remove the relevant list item in the "Subprojects" section and open a Pull Request in this repository, following instructions in the Pull Request Template to populate the text of the PR.

PR will be merged on unanimous approval from Approvers.

If the repositories of the subproject are under the WG's GitHub organization, they will be transferred out of the organization or deleted at this time.

## Governance

### Meetings

* Regular WG Meeting: TBD
  * Meetings will be announced on discourse.ros.org and the ROS Events calendar.
  * Recordings will be posted to the YouTube channel "ROS 2 Working Groups" https://www.youtube.com/playlist?list=PLpUh4ScdBhSMb98_C0q_zIT8GNMehYBd_

### Communication Channels

* Email list: https://groups.google.com/g/ros-webtools-working-group
* ROS Discourse

### Backlog Management

* TBD

### Membership, Roles and Organization Management

Working Group members may act in one or more of the following roles:

* **Member**
  * Prerequisite: Attend at least one out of the last three Working Group meetings
  * Responsible for triaging issues
* **Reviewer**
  * All reviewers are members
  * Prerequisite: Proven track record of high-quality reviews to WG Subprojects
  * Responsible for reviewing pull requests
* **Approver**
  * All approvers are reviewers
  * Prerequisite: Proven track record of high-quality contributions and reviews to WG Subprojects
  * Responsible for approving and merging pull requests
  * Responsible for vetting and accepting new projects into the Working Group
* **Lead**
  * TSC member or their delegate
  * Responsible for organizing and moderating working group meetings
  * Responsible for posting meeting materials (minutes, recordings, etc.)
  * Responsible for breaking ties

To become a member or change role, create an issue in this repository using the appropriate issue template.
Such applications are accepted upon unanimous agreement from Approvers, and are typically based on the applicant's history with the subprojects of the Working Group.
The Lead role cannot be applied for, as it is an appointee of the ROS 2 TSC.

### Modifying this governance document

Changes to this document will be made via Pull Request.
The PR will be merged on unanimous agreement from Approvers.
