
DefaultListableBeanFactory
------

![img.png](img.png)

AliasRegistry
------


![img_1.png](img_1.png)

SimpleAliasRegistry:
------

以map实现AliasRegistry

```java
/**
 * Simple implementation of the {@link AliasRegistry} interface.
 * <p>Serves as base class for
 * {@link org.springframework.beans.factory.support.BeanDefinitionRegistry}
 * implementations.
 */
public class SimpleAliasRegistry implements AliasRegistry {
    /** Map from alias to canonical name. */
    private final Map<String, String> aliasMap = new ConcurrentHashMap<>(16);
}
```

SingletonBeanRegistry
------
Interface that defines a registry for **shared bean instances** (singleton instance).

![img_2.png](img_2.png)