# MvvmWithLive

#The Data Binding Library is a support library that allows you to bind UI components in your layouts to data sources in your app using a declarative format rather than programmatically.

     TextView textView = findViewById(R.id.sample_text);
     textView.setText(viewModel.getUserName());

#The following example shows how to use the Data Binding Library to assign text to the widget directly in the layout file. This removes the need to call any of the Java code shown above. Note the use of @{} syntax in the assignment expression:

                <TextView
                    android:text="@{viewmodel.userName}" />


* This can also improve your app's performance and help prevent memory leaks and null pointer exceptions.








Put And Get Data one activity to another activity

get Data
     testData= new Gson().fromJson(bundle.getString("testData"), TestData.class);



put data
      intent.putExtra("testData" ,new Gson().toJson(testData, TestData.class));

# MVVM Why we use:
# P1:- 
Supose we have list of user details with bitmap image url so we cant use onSavedInstanceState and restore data with the save bcz of this is large amount of data. It is use only in case of small amount data that can serialized and deserialized.

#A ViewModel must never hold a referance of a view.
This design also means you can write tests to cover a ViewModel more easily as it doesn't know about view and Lifecycle objects.

# The lifecycle of a ViewModel:
1. Scope of activity is till its not finish and in Fragment till detached Fragment.
2. We can use ViewModelProvider when getting the ViewModel Object instance.
3. 
