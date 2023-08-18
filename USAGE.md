<!-- Start SDK Example Usage -->


```java
package hello.world;

import ryan_test.test_language_tags.TestLanguageTags;
import ryan_test.test_language_tags.models.operations.CreatePetsResponse;

public class Application {
    public static void main(String[] args) {
        try {
            TestLanguageTags sdk = TestLanguageTags.builder()
                .build();

            CreatePetsResponse res = sdk.pets.createPets();

            if (res.statusCode == 200) {
                // handle response
            }
        } catch (Exception e) {
            // handle exception
        }
    }
}
```
<!-- End SDK Example Usage -->