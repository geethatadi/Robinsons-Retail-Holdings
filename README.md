**Features:**
  Fetch data from a REST API.
  Sort items by date.
  Display items in a RecyclerView.
  View detailed information about each retail item by clicking on it.


**Technologies Used:**
  Kotlin: Programming language for Android app development.
  Retrofit: Library for handling API requests.
  RecyclerView: To display the list of retail items.
  Coroutines: For performing network requests asynchronously.

**Setup Instructions:**
Prerequisites:
Ensure that you have the following installed:
Android Studio: For building and running the Android project.
Java Development Kit (JDK): Make sure you have the latest JDK installed.
Retrofit: Retrofit library for handling API calls.

**Step 1: Clone the Repository**
Clone the repository to your local machine using the following command:
git clone https://github.com/yourusername/retail-app.git

**Step 2: Add Dependencies**
In your build.gradle file (Module: app), add the following dependencies for Retrofit, Gson converter, and coroutines:
// Retrofit Dependencies
implementation 'com.squareup.retrofit2:retrofit:2.9.0'
implementation 'com.squareup.retrofit2:converter-gson:2.9.0'
implementation 'com.squareup.okhttp3:logging-interceptor:4.9.0'
// Coroutines Dependency
implementation 'org.jetbrains.kotlinx:kotlinx-coroutines-android:1.4.3'
// RecyclerView Dependency
implementation 'androidx.recyclerview:recyclerview:1.2.0'

**Step 3: Set Up the API**
You need to replace the base URL of the API in the Retrofit instance to your own backend URL. In the RetailActivity class, find the line:
.baseUrl("https://your-api-base-url.com/") // Replace with your API base URL

**Step 4: Run the App**
Connect your Android device or use the Android Emulator.
Build and run the app from Android Studio.

**Step 5: Test the Application**
The app will fetch retail items from the API and display them in a sorted list by date.
Click on any item in the list to see more details about the retail item.

**Project Structure:**
RetailActivity.kt: The main activity that fetches data from the API, sorts it by date, and displays it in a RecyclerView.
RetailItem.kt: Data model representing a retail item.
RetailAdapter.kt: Adapter for displaying the list of retail items in the RecyclerView.
ItemDetailActivity.kt: Activity that displays the details of a selected retail item.
res/layout/activity_retail.xml: Layout for the main activity, including the RecyclerView.
res/layout/item_retail.xml: Layout for each item in the RecyclerView.

License
This project is licensed under the MIT License - see the LICENSE file for details.

**Acknowledgements**
Retrofit for API handling.

Android's RecyclerView and Coroutines for smooth UI and performance.
