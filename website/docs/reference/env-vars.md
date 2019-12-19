---
title: Environment Variables
sidebar_label: Env Vars
description: Vector's environment variables
---

You can control Vector's behavior through select environment variables:

```bash
ENV_VAR1=val ENV_VAR2=val vector --config=/etc/vector/vector.toml
```

In addition, we recommend that you look at the [global configuration 
options][docs.global-options] as well.

<!--
     THIS FILE IS AUTOGENERATED!

     To make changes please edit the template located at:

     website/docs/reference/env-vars.md.erb
-->

## Variables

import Fields from '@site/src/components/Fields';

import Field from '@site/src/components/Field';

<Fields filters={true}>


<Field
  common={false}
  defaultValue={null}
  enumValues={null}
  examples={["AKIAIOSFODNN7EXAMPLE"]}
  name={"AWS_ACCESS_KEY_ID"}
  nullable={true}
  path={null}
  relevantWhen={null}
  required={false}
  templateable={false}
  type={"string"}
  unit={null}
  >

### AWS_ACCESS_KEY_ID

Used for AWS authentication when communicating with AWS services. See relevant [AWS components][pages.aws_components] for more info.


</Field>


<Field
  common={false}
  defaultValue={null}
  enumValues={null}
  examples={["wJalrXUtnFEMI/K7MDENG/FD2F4GJ"]}
  name={"AWS_SECRET_ACCESS_KEY"}
  nullable={true}
  path={null}
  relevantWhen={null}
  required={false}
  templateable={false}
  type={"string"}
  unit={null}
  >

### AWS_SECRET_ACCESS_KEY

Used for AWS authentication when communicating with AWS services. See relevant [AWS components][pages.aws_components] for more info.


</Field>


<Field
  common={false}
  defaultValue={"unix:///var/run/docker.sock"}
  enumValues={null}
  examples={["unix://path/to/socket","tcp://host:2375/path"]}
  name={"DOCKER_HOST"}
  nullable={false}
  path={null}
  relevantWhen={null}
  required={false}
  templateable={false}
  type={"string"}
  unit={null}
  >

### DOCKER_HOST

The docker host to connect to.


</Field>


<Field
  common={false}
  defaultValue={true}
  enumValues={null}
  examples={[true,false]}
  name={"DOCKER_VERIFY_TLS"}
  nullable={false}
  path={null}
  relevantWhen={null}
  required={false}
  templateable={false}
  type={"bool"}
  unit={null}
  >

### DOCKER_VERIFY_TLS

If `true` (the default), Vector will validate the TLS certificate of the remote host. Do NOT set this to `false` unless you understand the risks of not verifying the remote certificate.


</Field>


<Field
  common={true}
  defaultValue={null}
  enumValues={null}
  examples={["debug"]}
  name={"LOG"}
  nullable={false}
  path={null}
  relevantWhen={null}
  required={true}
  templateable={false}
  type={"string"}
  unit={null}
  >

### LOG

Sets Vector's log level. See the [log section in the monitoring guide][docs.monitoring#level] for more information on the available levels.


</Field>


<Field
  common={true}
  defaultValue={null}
  enumValues={null}
  examples={[true,false]}
  name={"RUST_BACKTRACE"}
  nullable={false}
  path={null}
  relevantWhen={null}
  required={true}
  templateable={false}
  type={"bool"}
  unit={null}
  >

### RUST_BACKTRACE

Enables backtraces when errors are logged. Use this when debugging only since it can degrade performance.


</Field>


</Fields>


[docs.global-options]: /docs/reference/global-options/
[docs.monitoring#level]: /docs/administration/monitoring/#level
[pages.aws_components]: /components?providers%5B%5D=aws/