# Code Of Conduct

# Principles (boring stuff :p )
   > Single Responsibility Principles
   > 3 second reading of method


## Naming: 
  * General: 
    * Method Name should be self eplanatory
  
  * Method Name Rules:
    * Test Method name should end with Test
    

## Comments:
  No Comments unless you can not self explain with code. 
  
## Number Of lines: 
   * Method: 20 Max
   * Class: 100 Max
  
## Order or class members:
   * Within a class, struct or interface: 
        * Constant Fields
        * Fields
        * Constructors
        * Properties
        * Methods
   * Within each of these groups order by access:
      * public
      * internal
      * protected internal
      * protected
      * private
   * Within each of the access groups, order by static, then non-static: (SA1204)
      * static
      * non-static
   * Within each of the static/non-static groups of fields, order by readonly, then non-readonly : (SA1214 and SA1215)
      * readonly
      * non-readonly

## DI for sure
  > All dependent classes must be loaded throuh constructor. 
    Sitecore: Microsoft.Extensions.DependencyInjection 
    Promo: AutoFac
    Using Containers is optional.
    
## Exception Handling
   * Exception Should only be handled at entry point
   * Exception Handle should be in different method with Try Prefix
    Ex: TryCallHttpEndPoint() => should only handle error
        CallHttpEndPoint() => Should do actual http call
        
## Configuration
   * Configuration should be in dedicated class
   * Load Configuration through constructor for easy unit testability
 
