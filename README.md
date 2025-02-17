# Intellij IDEA File and Live Templates
Custom [File Templates](https://www.jetbrains.com/help/idea/using-file-and-code-templates.html) and [Live templates](https://www.jetbrains.com/help/idea/using-live-templates.html)

File templates
`Settings -> Editor -> File and Code Templates`

Live templates
`Settings -> Editor -> Live Templates`

## File templates
### Pattern
> Singleton
```<java>
#if (${PACKAGE_NAME} && ${PACKAGE_NAME} != "")package ${PACKAGE_NAME};#end

import lombok.AccessLevel;
import lombok.NoArgsConstructor;

@NoArgsConstructor(access = AccessLevel.PRIVATE)
public class ${NAME} {

    private static final ${NAME} INSTANCE = new ${NAME}();

    public static ${NAME} getInstance() {
        return INSTANCE;
    }
}
```
