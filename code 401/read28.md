#### Create dynamic lists with RecyclerView   
* RecyclerView makes it easy to efficiently display large sets of data. You supply the data and define how each item looks, and the RecyclerView library dynamically creates the elements when they're needed.

#### Key classes :
* Several different classes work together to build your dynamic list.

 - RecyclerView is the ViewGroup that contains the views corresponding to your data. It's a view itself, so you add RecyclerView into your layout the way you would add any other UI element.

 * Each individual element in the list is defined by a view holder object. When the view holder is created, it doesn't have any data associated with it. After the view holder is created, the RecyclerView binds it to its data. You define the view holder by extending RecyclerView.ViewHolder.

 * The RecyclerView requests those views, and binds the views to their data, by calling methods in the adapter. You define the adapter by extending RecyclerView.Adapter.

 * The layout manager arranges the individual elements in your list. You can use one of the layout managers provided by the RecyclerView library, or you can define your own. Layout managers are all based on the library's LayoutManager abstract class.


### Steps for implementing your RecyclerView : 
 - 1 - First of all, decide what the list or grid is going to look like. Ordinarily you'll be able to use one of the RecyclerView library's standard layout managers.
 - 2 - Design how each element in the list is going to look and behave. Based on this design, extend the ViewHolder class.
 - 3 -  Define the Adapter that associates your data with the ViewHolder views.

![implementing](https://www.andreasjakl.com/wp-content/uploads/2018/01/Android-RecyclerView-Adapter-Flow-2000x1200.png) 

  * most common layout situations:
   - 1 -LinearLayoutManager :arranges the items in a one-dimensional list..
 - 2 - GridLayoutManager  :arranges all items in a two-dimensional grid.
 - 3 -  StaggeredGridLayoutManager : is similar to GridLayoutManager, but it does not require that items in a row have the same height (for vertical grids) or items in the same column have the same width (for horizontal grids). The result is that the items in a row or column can end up offset from each other.

 ## Implementing your adapter and view holder :
  * Once you've determined your layout, you need to implement your Adapter and ViewHolder. 
  * These two classes work together to define how your data is displayed :
  * 1- ViewHolder is a wrapper around a View that contains the layout for an individual item in the list.
  * 2- Adapter creates ViewHolder objects as needed, and also sets the data for those views. The process of associating views to their data is called binding.

 * then  you need to override three key methods:
 *  1- onCreateViewHolder()
 *  2 - getItemCount()
 *  3 - onBindViewHolder()
