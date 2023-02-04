#### Add TextViews to Layout

- Everytime you create a view in Java code, you need to pass in a context, so that the view knows the theme and other information about the app in which it will be displayed.
- So it kind of gives the context as to what's going on around it.
- Therefore in the NumbersActivityClass, this will also be a context.

#### View Recycling
- View Recycling means reusing views that are no longer visible on the screen anymore.
- Using the ListView and ArrayAdapter, we can create just enough views, meaning list item rows, based on what we need to fill up the screen. This means if we scroll upwards, we no longer need to see the views at the bottom of the screen.
- Now furthermore, we can recycle three types of views. ListView, GridView and RecyclerView.

#### ListView and ArrayAdapter
- We can think of ListView as being powered by the ArrayAdapter.
- So without the adapter, the ListView is just an empty container.
- Array adapter holds onto the set of data that should be shown onto screen.
- For example, it can hold onto an array or even a list of data.
- So  the ArrayAdapter knows how to translate this data or adapt it into a list item view that will be displayed in the ListView.
- ![[ArrayAdapter.png]]
- Therefore in the code
```Java
        ArrayAdapter<String> itemsAdapter = new ArrayAdapter<String>(this, android.R.layout.simple_list_item_1, words);
        ListView listView = (ListView) findViewById(R.id.list);
        listView.setAdapter(itemsAdapter);
```
- We are creating an Array Adapter which contains a list of Strings as its data source.
- Then we are searching through the view hierarchy for the listview which is defined in our XML layout.
- And then we are associating arrayAdapter with the listview.
- R.layout : 
https://developer.android.com/reference/android/R.layout
- Generics in Java : 
https://www.geeksforgeeks.org/generics-in-java/