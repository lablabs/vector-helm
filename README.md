# Vector.dev Helm Chart

[<img src="ll-logo.png">](https://lablabs.io/)

We help companies build, run, deploy and scale software and infrastructure by embracing the right technologies and principles. Check out our website at https://lablabs.io/

---


## Description

A Helm chart for Vector.dev. Deploys vector agent as a DaemonSet.

![Version: 0.1.0](https://img.shields.io/badge/Version-0.1.0-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 0.11.1](https://img.shields.io/badge/AppVersion-0.11.1-informational?style=flat-square)

## Prerequisites

- Helm v3

## Contributing and reporting issues

Feel free to create an issue in this repository if you have questions, suggestions or feature requests.




## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| additionalServices | list | `[]` |  |
| affinity | object | `{}` |  |
| fullnameOverride | string | `""` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repository | string | `"timberio/vector"` |  |
| image.tag | string | `"0.11.1-alpine"` |  |
| imagePullSecrets | list | `[]` |  |
| metrics.enabled | bool | `true` |  |
| metrics.port | int | `9598` |  |
| metrics.serviceMonitor.enabled | bool | `true` |  |
| nameOverride | string | `""` |  |
| nodeSelector | object | `{}` |  |
| podAnnotations | object | `{}` |  |
| podSecurityContext | object | `{}` |  |
| resources | object | `{}` |  |
| securityContext | object | `{}` |  |
| service.port | int | `80` |  |
| service.topologyKeys[0] | string | `"kubernetes.io/hostname"` |  |
| service.topologyKeys[1] | string | `"topology.kubernetes.io/zone"` |  |
| service.topologyKeys[2] | string | `"topology.kubernetes.io/region"` |  |
| service.topologyKeys[3] | string | `"*"` |  |
| service.type | string | `"ClusterIP"` |  |
| serviceAccount.annotations | object | `{}` |  |
| serviceAccount.create | bool | `true` |  |
| serviceAccount.name | string | `""` |  |
| sinks | object | `{}` |  |
| sources | object | `{}` |  |
| tolerations | list | `[]` |  |

## License

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

See [LICENSE](LICENSE) for full details.

    Licensed to the Apache Software Foundation (ASF) under one
    or more contributor license agreements.  See the NOTICE file
    distributed with this work for additional information
    regarding copyright ownership.  The ASF licenses this file
    to you under the Apache License, Version 2.0 (the
    "License"); you may not use this file except in compliance
    with the License.  You may obtain a copy of the License at

      https://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing,
    software distributed under the License is distributed on an
    "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
