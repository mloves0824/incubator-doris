---
{
    "title": "BE Metrics",
    "language": "en"
}
---

<!-- 
Licensed to the Apache Software Foundation (ASF) under one
or more contributor license agreements.  See the NOTICE file
distributed with this work for additional information
regarding copyright ownership.  The ASF licenses this file
to you under the Apache License, Version 2.0 (the
"License"); you may not use this file except in compliance
with the License.  You may obtain a copy of the License at

  http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing,
software distributed under the License is distributed on an
"AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
KIND, either express or implied.  See the License for the
specific language governing permissions and limitations
under the License.
-->

<!-- Please sort the metrics alphabetically -->

# BE Metrics

This document mainly introduces the monitor metrics of BE.

## View Metrics

BE metrics can be viewed by visiting:

`http://be_host:be_webserver_port/metrics`

The default format is of [Prometheus](https://prometheus.io/).

You can get Json format by visiting:

`http://be_host:be_webserver_port/metrics?type=agent`

## Metrics List

### `doris_be_snmp{name="tcp_in_errs"}`

Value of the `Tcp: InErrs` field in `/proc/net/snmp`. Represents the number of error TCP packets currently received.

The incidence rate can be calculated in combination with the sampling period.

Usually used to troubleshoot network problems.

### `doris_be_snmp{name="tcp_retrans_segs"}`

Value of the `Tcp: RetransSegs` field in `/proc/net/snmp`. Represents the number of error TCP packets currently received.

The incidence rate can be calculated in combination with the sampling period.

Usually used to troubleshoot network problems.
