# Tests 

- (in src/test/java/com/example/myapp/service/ )

```java
package com.example.myapp.service;

import org.junit.*;
import static org.junit.Assert.assertEquals;
import org.junit.runner.RunWith;
import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.boot.test.context.SpringBootTest;
import org.springframework.test.context.junit4.SpringRunner;

@RunWith(SpringRunner.class)
@SpringBootTest
public class UserServiceTest {

    @Autowired
    UserService userService;

    @Before
    public void before(){
        System.out.println("BEFORE!");
    }

    @After
    public void after(){
        System.out.println("AFTER!");
    }

    @BeforeClass
    public static void beforeClass(){
        System.out.println("======= BEFORE_CLASS!");
    }

    @AfterClass
    public static void afterClass(){
        System.out.println("======= AFTER_CLASS!");
    }

    @Test
    public void doubleMeTest(){
        int expectedResult = 20;
        int actualResult = userService.doubleMe(10);

        assertEquals(expectedResult, actualResult);
    }

    @Test
    public void fooTest(){
        String expectedResult = "foo here from service";
        String actualResult = userService.foo();

        assertEquals(expectedResult, actualResult);
    }

}

```
