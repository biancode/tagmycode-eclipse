TagMyCode Official Eclipse Plugin
=================================

This is the official Eclipse plugin for [TagMyCode](http://tagmycode.com).

## Getting started ##
### Dependencies###
To download all dependencies use Maven

```bash
mvn clean package
```

this command downloads all required dependencies into ```lib``` folder

###Consumer Id and Consumer secret###
You need to create a Java class ```Secret.java``` into ```plugin/com/tagmycode/eclipse```

```java
package com.tagmycode.intellij;

import com.tagmycode.plugin.AbstractSecret;

public class Secret extends AbstractSecret {
    @Override
    public String getConsumerId() {
        return "YOUR_CONSUMER_ID";
    }

    @Override
    public String getConsumerSecret() {
        return "YOUR_CONSUMER_SECRET";
    }
}

```
