#################################################################
# 
#        Copyright 2013, Big Switch Networks, Inc. 
# 
# Licensed under the Eclipse Public License, Version 1.0 (the
# "License"); you may not use this file except in compliance
# with the License. You may obtain a copy of the License at
# 
#        http://www.eclipse.org/legal/epl-v10.html
# 
# Unless required by applicable law or agreed to in writing,
# software distributed under the License is distributed on an
# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND,
# either express or implied. See the License for the specific
# language governing permissions and limitations under the
# License.
# 
#################################################################
include ../../../init.mk

MODULE := FME_utest
TEST_MODULE :=  FME
DEPENDMODULES := AIM BigList uCli IOF PPE OS

GLOBAL_CFLAGS += -DFME_CONFIG_INCLUDE_UTM=1 -DAIM_CONFIG_INCLUDE_POSIX=1
GLOBAL_CFLAGS += -DAIM_CONFIG_INCLUDE_VALGRIND=1
GLOBAL_CFLAGS += -DAIM_CONFIG_INCLUDE_MODULES_INIT=1
GLOBAL_CFLAGS += -DAIM_CONFIG_INCLUDE_MAIN=1
GLOBAL_CFLAGS += -DUCLI_CONFIG_INCLUDE_FGETS_LOOP=1

OS_MAKE_CONFIG_AUTOSELECT := 1
PEDANTIC := 1

include $(BUILDER)/build-unit-test.mk

