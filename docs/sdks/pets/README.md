# pets

### Available Operations

* [createPets](#createpets) - Create a pet
* [listPets](#listpets) - List all pets
* [showPetById](#showpetbyid) - Info for a specific pet

## createPets

Create a pet

### Example Usage

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


### Response

**[ryan_test.test_language_tags.models.operations.CreatePetsResponse](../../models/operations/CreatePetsResponse.md)**


## listPets

List all pets

### Example Usage

```java
package hello.world;

import ryan_test.test_language_tags.TestLanguageTags;
import ryan_test.test_language_tags.models.operations.ListPetsRequest;
import ryan_test.test_language_tags.models.operations.ListPetsResponse;

public class Application {
    public static void main(String[] args) {
        try {
            TestLanguageTags sdk = TestLanguageTags.builder()
                .build();

            ListPetsRequest req = new ListPetsRequest() {{
                limit = 548814;
            }};            

            ListPetsResponse res = sdk.pets.listPets(req);

            if (res.pets != null) {
                // handle response
            }
        } catch (Exception e) {
            // handle exception
        }
    }
}
```

### Parameters

| Parameter                                                                                                    | Type                                                                                                         | Required                                                                                                     | Description                                                                                                  |
| ------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                    | [ryan_test.test_language_tags.models.operations.ListPetsRequest](../../models/operations/ListPetsRequest.md) | :heavy_check_mark:                                                                                           | The request object to use for the request.                                                                   |


### Response

**[ryan_test.test_language_tags.models.operations.ListPetsResponse](../../models/operations/ListPetsResponse.md)**


## showPetById

Info for a specific pet

### Example Usage

```java
package hello.world;

import ryan_test.test_language_tags.TestLanguageTags;
import ryan_test.test_language_tags.models.operations.ShowPetByIdRequest;
import ryan_test.test_language_tags.models.operations.ShowPetByIdResponse;

public class Application {
    public static void main(String[] args) {
        try {
            TestLanguageTags sdk = TestLanguageTags.builder()
                .build();

            ShowPetByIdRequest req = new ShowPetByIdRequest("provident");            

            ShowPetByIdResponse res = sdk.pets.showPetById(req);

            if (res.pet != null) {
                // handle response
            }
        } catch (Exception e) {
            // handle exception
        }
    }
}
```

### Parameters

| Parameter                                                                                                          | Type                                                                                                               | Required                                                                                                           | Description                                                                                                        |
| ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ |
| `request`                                                                                                          | [ryan_test.test_language_tags.models.operations.ShowPetByIdRequest](../../models/operations/ShowPetByIdRequest.md) | :heavy_check_mark:                                                                                                 | The request object to use for the request.                                                                         |


### Response

**[ryan_test.test_language_tags.models.operations.ShowPetByIdResponse](../../models/operations/ShowPetByIdResponse.md)**

