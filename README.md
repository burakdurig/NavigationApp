Navigation Framework:
- The Navigation Architecture Component simplifies implementing navigation, while also helping you visualize your app’s navigation flow The library provides several benefits, including:
    - Automatic handling of fragment transactions
    - Correctly handling up and back by default
    - Default behaviors for animations and transitions
    - Deep linking as a first-class operation
    - Implementing navigation UI patterns (like navigation drawers and bottom navigation) with little additional work
    - Type safety when passing information while navigating
    - Android Studio tooling for visualizing and editing the navigation flow of an app.

Navigation parts:
- The Navigation component consists of three key parts, working together in harmony. Such as:
    - Navigation Graph (New XML resource) - this is a resource that contains all navigation-related information in one centralized location. This includes all the places in your app. Known as Destinations, and possible pats a user could take through your app
    - NavHostFragment (layout XML view) - this is a special widget you add to your layout. It displays different destinations for you Navigation Graph.
    - NavController (Kotlin.Java object) - This is an object that keeps track of the current position within the navigation graph. It orchestrates swapping destination content in the NavHostFragment as you move through a navigation graph.

Navigation Graph:
- A navigation graph is a new resource type that defines all possible paths a user can take through an app. It shows visually all the destinations that can be reached from a given destination. Android Studio displays the graph in its Navigation Editor

Nav Host Fragment
- NavHostFragment provides an area within your layout for self-contained navigation to occur.
- NavHostFragment is intended to be used as the content area within a layout resource defining your app’s chrome around it.
- Each NavHostFragment has a NavController that defines valid navigation within the navigation host.
- This includes the NavGraph as well as navigation state such as current location and back stack that will be saved and restored along with the navHostFragment itself.

Nav Controller
- Navigation to a destination is done using a NavController, an object that manages app navigation within a NavHost.
- Each NavHost has its own corresponding NavController. You can retrieve a NavController by using one of the following methods:
    - Fragment.findNavController()
    - View.findNavController()
    - Activity.findNavController(viewId: int)
- Actions: The routes user can take between your app’s destinations. Which are represented by the arrow sign in the design view.;


Credits go to Abbass Masri
from The Complete Android 14 Developer Course
