# MvvmWithLive

#The Data Binding Library is a support library that allows you to bind UI components in your layouts to data sources in your app using a declarative format rather than programmatically.

TextView textView = findViewById(R.id.sample_text);
textView.setText(viewModel.getUserName());

#The following example shows how to use the Data Binding Library to assign text to the widget directly in the layout file. This removes the need to call any of the Java code shown above. Note the use of @{} syntax in the assignment expression:

<TextView
    android:text="@{viewmodel.userName}" />
