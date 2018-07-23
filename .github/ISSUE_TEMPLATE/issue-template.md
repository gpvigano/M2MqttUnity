---
name: Issue template
about: Generic template for issues

---

### Precheck

> * For proposing a new feature, please check existing open and closed issues before creating a duplicate
> * For bugs, do a quick search and make sure the bug has not yet been reported
> * Finally, follow the code of conduct (at <https://github.com/gpvigano/AsImpL/blob/master/CODE_OF_CONDUCT.md>)

### Environment
>Please specify:
> * version of AsImpL (Github master commit hash or at least date/hour when you downloaded it)
> * version of Unity3D (e.g. Unity 5.4.4f1)

### Steps to reproduce

> For general bugs, attempt to recreate the issue with a simple example code and provide steps to reproduce if possible. Include code samples, errors and stacktraces if appropriate.
> If you change M2Mqtt files, unless your changes affect only the integration with Unity (`#if ... UNITY_...`), you should also access the [paho.mqtt.m2mqtt](https://github.com/eclipse/paho.mqtt.m2mqtt) repository to raise issues or make pull requests, this is especially important if you ask for a possible bug fix in M2MQTT.

### Expected behavior

> For general bugs, briefly describe what you expect should happen.

### Current behavior

> For general bugs, briefly describe what is actually happening.
