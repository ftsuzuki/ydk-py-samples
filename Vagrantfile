# -*- mode: ruby -*-
# vi: set ft=ruby :
#
# Copyright 2016 Cisco Systems, Inc.
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
#     http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.
#

# Multi-machine configuration extensible to multiple distros
Vagrant.configure(2) do |config|
  # Ubuntu as primary box
  config.vm.define "ydk-py-ubuntu", primary: true do |ydk_py_ubuntu|
    ydk_py_ubuntu.vm.box = "ydk-py-ubuntu"
    ydk_py_ubuntu.vm.box_url = "http://ydk.cisco.com/vagrant/ydk-py-ubuntu/"
    ydk_py_ubuntu.vm.synced_folder "samples", "/home/vagrant/samples"
    ydk_py_ubuntu.vm.synced_folder "projects", "/home/vagrant/projects"
  end
end