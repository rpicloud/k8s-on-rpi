<!---
 Copyright 2015 Arjen Wassink

 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at

     http://www.apache.org/licenses/LICENSE-2.0

 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
--->

Kubernetes on Raspberry PI
==========================
This repository is a fork of Arjen Wassink's "Kubernetes on Raspberry Pi".

Additions in this fork (very soon)
* Timeout values tweaked for demo purposes (see Ray Tsang's [blog post](https://medium.com/google-cloud/everything-you-need-to-know-about-the-kubernetes-raspberry-pi-cluster-2a2413bfa0fa#.mf0burwfa)).
  * Marking unresponsive nodes unhealthy after 10 seconds insted of 40 seconds (--node-monitor-grace-period=10s)
  * Rescheduling/deletion of pods on failed nodes after 5 seconds instead of 5 minutes (--pod-eviction-timeout=5s)
  * [Deployment script](https://github.com/rpicloud/rpi-docker-deploy-script) for hypriot/rpi-java projects that builds docker image and uploads to Docker Hub
