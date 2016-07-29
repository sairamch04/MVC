# MVC
A very basic MVC framework developed using Java servlets

## Design
The DispatchServlet(front-controller) is responsible for routing the url to the corresponding application controller. Application router uses Model to render View

Usage:
    Add the url mappings in the **init** method of **DispatchServlet**
    
    Here, we define 2 routes in this case, we maped  “/hello” to Index2 and “/” to Index
    
    public void init() {	
        ..
        ..
  	pathToViewname.put("/hello", "Index2");
  	pathToViewname.put("/", "Index");		
    }
    
  Index2 and Index are to be added  in  org.Framework.Handler and implement 
  AppController interface. The interface is responsible to render corresponding view using  Model.
  
  Here, The views for Index and Idex2 controllers are Index.jsp and Index2.jsp respectively
  
  Please have a look into  code for clarity
