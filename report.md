
# SETUP
1.Preparation-We'll need several Maven dependencies for running the integration tests we'll use in this article. First and foremost, we'll need the latest junit-jupiter-engine, junit-jupiter-api, and Spring test dependencies

2.Spring MVC Test Configuration - Then see how to configure and run the Spring enabled tests.

3.Enable Spring in Tests with JUnit 5 - We can enable this extension by adding the @ExtendWith annotation to our test classes and specifying the extension class to load. To run the Spring test, we use SpringExtension.class.We'll also need the @ContextConfiguration annotation to load the context configuration and bootstrap the context that our test will use.Finally, we'll also annotate the test with @WebAppConfiguration, which will load the web application context.

4.The WebApplicationContext Object- WebApplicationContext provides a web application configuration. It loads all the application beans and controllers into the context.

5.Mocking Web Context Beans- MockMvc provides support for Spring MVC testing. It encapsulates all web application beans and makes them available for testing.We'll initialize the mockMvc object in the @BeforeEach annotated method, so that we don't have to initialize it inside every test.

6.Verify Test Configuration-Let's verify that we're loading the WebApplicationContext object (webApplicationContext) properly. We'll also check that the right servletContext is being attached

7.Writing Integration Tests

8.Verify View Name-We can invoke the /homePage endpoint from our test

9.Verify Response Body-We'll invoke the some needed endpoints from our test.

10.Send GET Request With Path Variable

11.Send GET Request With Query Parameteres

12.Send POST Requests

# Conclusion
In this repository I implemented a few simple Spring-enabled integration tests following the steps above.

