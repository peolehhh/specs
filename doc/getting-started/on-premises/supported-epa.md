```text
SPDX-License-Identifier: Apache-2.0
Copyright (c) 2019-2020 Intel Corporation
```
<!-- omit in toc -->
# OpenNESS OnPremises - Enhanced Platform Awareness Features supported 
- [Overview](#overview)
- [Features](#features)

## Overview 
Enhanced Platform Awareness features are supported in OnPremises using EVA APIs. The flow looks like this:
1. From the OpenNESS controller UI user would use create the HTTP REST POST API to set the required EPA features (from the list of supported) for a given application. Key=value methodology is used for this. 
2. Controller send the API over gRPC to the EVA agent on the Edge node 
3. EVA APIs has Enhanced Application Configuration (EAC) handler that will detect if the EPA feature is requested for Application running in a VM or Container. Once this is done required configuration is generated by the EVA agent. 
4. Application is started (VM or Container based)

## Features 
Following are the EPA features supported in OpenNESS OnPremises Edge
1. [<b>openness_hddl.md</b>: Using Intel® Movidius™ Myriad™ X High Density Deep Learning (HDDL) solution in OpenNESS](https://github.com/open-ness/specs/blob/master/doc/enhanced-platform-awareness/openness_hddl.md)
2. [<b>openness-environment-variables.md</b>: Support for setting Environment Variables in OpenNESS](https://github.com/open-ness/specs/blob/master/doc/enhanced-platform-awareness/openness-environment-variables.md)
3. [<b>openness-dedicated-core.md</b>: Dedicated CPU core allocation support for Edge Applications and Network Functions](https://github.com/open-ness/specs/blob/master/doc/enhanced-platform-awareness/openness-dedicated-core.md)
4. [<b>openness-tunable-exec.md</b>: Tunable executable command in OpenNESS On-Prem mode](https://github.com/open-ness/specs/blob/master/doc/enhanced-platform-awareness/openness-tunable-exec.md)
5. [<b>openness-sriov-mulitple-interfaces.md</b>: Multiple Interface and PCIe SRIOV support in OpenNESS](https://github.com/open-ness/specs/blob/master/doc/enhanced-platform-awareness/openness-sriov-multiple-interfaces.md)
6. [<b>openness-port-forward.md</b>: Support for setting up port forwarding of a container in OpenNESS On-Prem mode](https://github.com/open-ness/specs/blob/master/doc/enhanced-platform-awareness/openness-port-forward.md)
