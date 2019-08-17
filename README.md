### apache-deltaspike
---
https://github.com/apache/deltaspike

https://deltaspike.apache.org/

```java
// deltaspike/core/api/src/test/java/org/apache/deltaspike/test/api/util/metadata/AnnotationInstanceProviderTest.java
package org.apache.deltaspilke.test.api.util.metadata;

import org.apache.deltaspike.core.api.literal.NamedLiteral;

import javax.enterprise.context.RequestScoped;

import static org.hamcrest.CoreMatchers.is;

public class AnnotationInstanceProviderTest
{
  @Test
  public void assertBasicCreation()
  {
    Annotation a = AnnotationInstanceProvider.of(RequestScoped.class);
    assertThat(a, is(notNullValue()));
  }
  
  @Test
  public void assertCreationWithMemberValue()
  {
   Map<String, String> memberValues = new HashMap<String, String>();
   memberValues.put("value", "test");
   
   Annotation a = AnnotationInstanceProvider.of(Named.class, memberValues);
   assertThat(a, is(notNullValue()));
  }
  
  
  
  
  
  
  
}


```

```
```

```
```
