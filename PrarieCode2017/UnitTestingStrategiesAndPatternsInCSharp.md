# Unit Testing Strategies & Patterns in C#

## Speaker

Bill Dinger
https://github.com/BillDinger/BikeShop

Ensure your code does what it's supposed to

Reduce brittleness of code

Unit Test:
- Fast
- Pass/Fail
- Repeatable
- Order Independent
- Easy to set up
- Test ONE small piece of functionality
- Test public interfaces only

1. Use Dependency Injection
2. Rely On Abstraction
3. Avoid Static Classes
    a. They cannot be mocked (easily)
4. The smaller your classes and methods, the easier your life

MSTest tips:
- Can analyze code coverage
- Live Unit Testing (VS 2017)

## AutoFixture
Test data container, deseigned to minimize the amount of "arrange" code you need

Object Creation
	
## AutoMock

Mocks an implementation of an interface

Freeze => Use this behavior
Inject => Use this instance	
		
Customize
    - Lets you customize object creation
		
	
## Mocking
			
### MoQ

- Matching Values with It.Is
- Verify Services Are called
- Mocking a DbSET
	
## Helpful tips
	
Handling HttpContext

Mocking HttpClient Calls
	
