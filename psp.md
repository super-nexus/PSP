* Programming platforms:
    * Why do we have different programming platforms (as opposed to a single general purpose platform)?
    * List at least two platforms and describe the key properties of each

* Web platform:
    * **Briefly describe the underlying technologies supporting the Web platform**  
        HTML (hyper text mark up language) is a markup language for hyper text, which is a text that points to another resource 
        HTTP -> is a client-server communication protocol where client sends the request and server responds with response. It has multiple methods: GET, POST, PUT, DELETE...
        URL -> is a unified way of referencing resources on the web 
    * **What is Hypertext? Briefly describe its historical role in the Web.**  
        Hyper text is text that points to another resource.
        It got invented in the 1963 and by 1968 there were already exmaple usages of hyper text on local file storage systems. In 1989 Tim Berners Lee connected hyper text with url and http and with that created the www 
    * What is WWW? List its main components.  
        WWW is a service which runs on the internet. Main components already listed above
    * Describe the functioning of HTTP.  
        Http is a client-server communication protocol, thus the client sends the request with certain http method and the server responds once it processes the request. After that the http connection is closed
    * What does HTTP response code 200 mean?  
        It means OK (Successful request)
    * Explain the difference between a single-tier and a multi-tier Web architecture  
        Single tier -> presentation, logic and data are all in a single program
        Multi tier -> different layers for presentation, logic and data. This allows for easier scalability and upgradeability of layers
    * List main functionalities of each: Presentation layer, Application/Business layer, Data layer in a multi-tier Web architecture.  
        Presentation layer -> deals with UI. It presents the data and handles user events
        Buisness layer -> it processes requests, fetches the data and with that connects the data and presentation layer
        Data layer -> deals with storing and the structure of the data. 
    * In his 1996 article, Tim Berners Lee expresses a concern that the Web looks like a lot of television channels. Explain what he means by this? In your opinion, is the Internet today still “a lot of television channels”? Defend your argument.  
        He meant by this that every page stated that it works best with certain version of a certain browser. I don't think this is the case today since all of the browsers follow the standards posted by W3C and most of the world uses a chromium based browser anyway. There are of course small discrepencies between different browsers but they are not noticeable for the average user, since they are mostly found in nitche applications
    * Changing URLs were a problem in the early Web. How is it solved nowadays?  
        It is solved with redirects. Http 301 states that resource has been permanently moved to another location, thus the redirect happens
    * What are content-delivery networks? How do they help with the network load?  
    * Explain how AJAX web pages work.  
        AJAX webpages are webpages which make AJAX requests, i.e they send asynchrounus requests to the server. This is why they are more interactive since the webpage does not need to be reloaded everytime a user interacts with the page 
    * What is Information-centric networking?
    * What is REST? List its main rules?  
        Rest (Representational state transfer) is a software architecture style used for writing web services
        Rules:  
        - stateless
        - cacheable
        - uniform interface
        - client-server (black boxes to eachother)
        - layered system
    * Describe constraints of REST and MEAN.  
        Rest:
        - stateless (client needs to send the context with each request)
        - weak security
        MEAN:
        - Does not use rleational databases which some projects require
    * Why does TCP work poorly over slow links (such as satellites)?  
        Because TCP waits for confirmation after it sends data. Since the satellites are far away that confirmation can take longer to come than the defined TCP timeout, because of that the requests can fail.
    * Why is HTTP often not used for low-resource devices in the Internet of Things?  
        Because http connections use additional resources compared to other alternatives (such as mqtt, lora...). They keep the connection open for longer since the client needs to wait for the response, which uses more battery 

* Mobile platform:
    * List at least four applications of mobile computing technology (note: don’t list specific applications, but application areas)  
        - Productivity applications (Todoist, Planner, Keep...)
        - Games (Candy crush, clash of clans...)
        - Workout trackers (S Health, Google fit, )
        - Messeging apps (Messenger, Viber, WhatsApp...)
    * Present some arguments about why you think that Symbian operating system failed to reach the popularity of Android or iOS.  
        - it wasn't optimized for capacitive touchscreens
        - it didn't have an appstore 
        - bad developing experience (for developers)
    * What is Android? (max 3 sentences)  
        Android is an open source, Linux based, mobile operating system from Google. 
    * What are the key affordances of the mobile platform?  
        - lot of user interactions
        - personalized devices 

    * What are the main constraints of the mobile platform?  
        - limited energy
        - limited processing power, limited resources are shared among apps, and background processing is limited in order preserve energy
        - wireless connection (is not always perfect or available at all)
        - security risks (people can lose their phones)
        - uniform user experience (due to large amount of different devices)
        - inaccurate sensors due to compact shape of devices and energy savings 
    * What should we be careful about when designing user interaction for a mobile application?  
        The Ui shouldn't contain really small elements, since the devices are small and have touch screens. The app should also use standard gestures if possible as the users don't want to learn different gestures for every app. 
    * Discuss ability to troubleshoot and upgrade software built and deployed in: 1) Android phones; 2) microwave ovens.  
        Android phones -- Android sutdio provides the ability to stop the program at a wanted line and observe the in memory data. Apps can be upgraded over the air with google play or other appstores
        Microwave oven -- ussually do not have software for debugging and upgrades are impossible after the product has already been deployed.

* Embedded platform:
    * List at least four applications of embedded computing technology (note: don’t list specific applications, but application areas)  
        - agriculture
        - IoT
        - Weapons
        - Space exploration
    * What are the key properties of embedded systems?  
        They tend to be specifically designed systems for a single task or operation. They are very efficient in what they do. They are programmed in low level programming languages to improve performance. Ussualy they are also resource constrained. 
    * What is a sensor?  
        Sensor is a device which reads physical properties from enviroment and converts it to electrical signal
    * What is an actuator?  
        It is a device which interacts/affects the enviroment. Usually it is driven by signals from embedded system and requires additional power for running (Not all of the time)
    * List at least two programming languages used for embedded programming.  
        C++, C, Assembler
    * Why do we use low-level programming languages for embedded programming?  
        They improve performance and allow developers to manage memory.
    * What is a real-time operating system?  
        System which processes the events/requests in real time, there is no buffer delay.
    * What is an interrupt routine in embedded programming?  
        It is a process of switching current running process with the interrupt program and than returning back the process (which was previously running) along with its context
    * What are the main constraints of embedded networked systems discussed in Estrin et al. article?
    * A vehicle often contains (at least two) independent embedded systems. Why?  
        They tend to have embedded systems for safety critical systems such as ABS breaking. They need to work 100% of the time and they need to respond ASAP. That is why they are seperatly developed and put in a car. On the other hand we have systems which deal with non safety critical functions such as operating radio from the stearing wheel buttons, this systems should not influence the safety critical ones, that is why they are seperated. 
    * What are the main threats for embedded systems’ wireless communication? Hint: Estrin et al. paper.
    * Why, even more so than with conventional desktop systems, we must ensure that embedded networked systems are correctly programmed?
    * “Failures we have in today’s technologies could be disastrous in embedded networked systems” warn Estrin et al. in 2001. Argue for or against this statement.
    * Discuss a potential use of embedded systems in precision agriculture.
    * Present at least one means of saving energy in an embedded system that senses the humiditiy in the field and notifies about potential floods.  
        Since humidity doesn't change so fast, we can measure humidity every 10 minutes and notify user only if necessery. In the mean time embedded system can sleep
    * Describe in one sentence each: IP Core, FPGA, and MCU.  
        - IP Core (Intellectual property core) is a reusable unit of logic or unit of functionality (Network controllers, Video/Audio chip...)
        - FPGA A reconfigurable integrated cuircat, which contains an array of programmable logic blocks.
        - MCU is a scaled down microprocessor, which needs to be programmed and is connected to other components
    * List key properties of a sensor that you should be aware of when deciding to use one in your system.  
        - Type (Analog/Digital)
        - Accuracy
        - Sensing range
        - Sensing interval
    * Describe the basics of analogue-digital conversion (ADC).  
        Analog signal, represented in voltage level, is converted to digital signal (by ADC) with n-bits. Because of limited number of bits, there will always a quantatization error 
    * List different storage components often available in an MCU. List their properties.  
        - Registers: extremly fast (ussualy can be accessed in under a clock cycle), very expensive, very small amount of storaga
        - Register file : is a set of registers, still very fast and expensive, very few of them in a system
        - Cache : fast, cheaper than registers but still expensive, larger memory cpacitiy than previous options
        - Main memory: slow (compared to other mentioned options), inexpensive, much larger memeroy capacity than before mentioned options
    * What is cross-compilation?  
        It is a process of compiling a program for different system architecture than the one you are compiling on (cross-compiling code for Arduino)
    * What is a toolchain?  
        It is a set of tools required to perform certain software development task
    * What are the main differences between an embedded operting system and a conventional (desktop) operating system?
    * What is a process? What are the process states? Draw a state transition diagram.  
        Process is an abstraction encapsulating set of processing tasks:  
        - Instructions
        - Resources assigned to it
        - Context --> processor state while the process is being executed
        TODO add diagram RUNING --<> READY <-- BLOCKED

    * Is Arduino a real-time OS?  
        Arduino does not have an OS, it only has a bootloader which loads your programm at the start.
    * Describe the following terms: input pin, output pin  
        Input pin is used for reading voltage from sensors/actuators. It can be digital or analogue  
        Output pin is a pin on which you can control the voltage level. If it is digital it can be high or low (on/off), if it's analog than you can state a specific voltage level
    * What is the difference between analogue and digital input pin? Give an example use of an analogue input pin.  
        Analog input pin is used to read analog signals from sensors, which are than converted to digital by ADC. Digital pins on the other hand can only read HIGH or LOW state of the pin.  
        They are used for reading the state of certain device (or maybe even sensor), which has only two states
    * What are the two basic functions of an Arduino sketch? Describe their use.  
        - setup() this function gets executed only once at the beginning of your programm and it is used for initialization (of variables, pins, serial communcation etc.)
        - loop() this function runs in a loop (after setup() is completed) while the Arduino is powered on and here you implement the main logic of your program

* Gaming platform:
    * What is a Gaming engine?  
        Is a piece of software which is used for game development. It often comes with already implemented physics and objects which can be directly put into game scenes
    * What is a GPU?  
        A graphics processing unit is a specialized electronic circuit designed to rapidly manipulate and alter
        memory to accelerate the creation of images in a frame buffer intended for output to a display device

* Android Programming:
    * What is “sandboxing” in Android OS?  
        Each app on Android is running in its own sandbox (container), which means its resources are protected from other potentially malicious applications.
    * Explain how permissions work in Android?  
        Normal permissions(flashlight, vibrate) are granted automatically by the os. Dangerous permissions on the other hand (location, contact list...) must be granted by the user. Since API 23 asking user for dangerous permission should be done right before the feature (which requires that permission) is about to be used
    * Sketch and describe the Android compilation process.  
        Firstly we compile the kotlin/java code into the java bytecode (.class). After that we can use proguard to get minimized bytecode, but it is not necessary. Once that is done we recompile the code into the .dex bytecode in order to save space and from there it is compiled to machine/native code which android devices use to run apps. 
    * A few years ago Google engineers decided to replace Dalvink, a just-in-time compiler, with ART, an ahead-of-time compiler. Briefly describe the differences and present some reasons that support the engineers’ decision.  
        The difference between the two is that ART uses ahead of time compiler, which compiles the applications during the installation and never again, meanwhile the Dalvik compiles the application when it needs it, so before launching the application.
        The reason google has opted for ART is that the applications only get installed once so it worth trading longer install times for faster app load times. 
    * What is the purpose of “res” folder in Android projects?  
        It holds applications static resources such as layouts, strings, drawables, styles...
    * How are non-compiled application resources accessed in Android programmes?  
        They are accessed through the R object (for example R.layout.main_layout)
    * Describe different means of storing data locally in Android applications  
        - Shared preferences -> used for storing primitive data in key-value pairs. Nice for storing users preferences. It is deleted once the app is uninstalled
        - Internal storage -> used for storing files to devices storage. This storage is always accessible only by your application and it gets deleted once the app gets uninstalled
        - External storage -> used for storing files to device or external storage. This storage may not be always accessible and other applications can access it. It does not get deleted once the app is uninstalled
        - Sql database -> its a relational database which gets deleted once your app is uninstalled 
    * What is the meaning of "?" and "!!" before accessing a property of an object in Kotlin?  
        The !! always returns the non-null value (we guarantee kotling that this value will not be null) and because of that it can throw a NullPointerException (if the value is null). 
        The ? returns the value if its not null or null if value is null 
        So the a!!.length would return a.length if a is not null and Null pointer exception otherwise.
        a?.length would return a.length if a is not null and null otherwise
    * What is "smart cast" in Kotlin?  
        it is a feature in kotlin which allows us to use variables without safe cast inside of if statements where we checked that the value of the variable is not null
        So something like this would be allowed
        ```  
            var foo: String? = "Hello"
            if(foo != null){
                print(foo.length)
            }
        ```
        Meanwhile something like this will not be accepted
        ```
            var foo: String? = "Hello"
            print(foo.length)
            // this is correct print(foo?.length)
        ```

    * What is a companion object in Kotlin?  
        companion object is an object whose variables are static i.e tied to the class and not the instance
    * You are a chief architect of the next most popular app on the market - the app allows users to record videos of themselves singing and dancing over popular tunes. You have to think about data storage for different parts of the app. Decide which method to use to store the following (explain!)  
        - Video files created by the app --> I would use external storage so the videos users create do not get deleted if they uninstall the app
        - Audio tracks used during the video generation --> I would use internal storage as they are still files so they can't be saved to sql db or shared preferences. But I would want them to be deleted once the app is uninstalled 
        - User settings --> I would use shared preferences since they are easy to read and write from and android can generate activitys which display and allow users to edit their preferences
    * What are SharedPreferences used for?  
        They are used for storing primitive data types in key-value pairs. Ussually for storing user preferences (such as theme of the app, remember login ....)
    * Activity lifecycle - draw diagram and clearly mark when activity exists, is visible, in the foreground  
        On the slides
    * Activity lifecycle - why did engineers decide to implement that way  
        Because users interact with the activitys and developers need to know in which state an activity is in order to do specific functions. Furthermore android OS can also kill your activities to optimize battery life and certain actions should be taken before that (saving state and users unsaved data, killing cpu intensive processes). That is why the lifecycle of activities exist  
    * How can we save an activity state and restore it when the activity is recreated?  
        We can save the activity state into a bundle in OnSaveInstanceState and later receive that bundle in OnRestoreInstanceState
    * Assume that each of the lifecycle callbacks (onCreate, onStart, etc.) print an associated log message with the callback and the activity name when called (e.g. “onCreate from Activity 1”, “onStart from Activity 1”, etc.). Write one after another all the log messages that will be printed at the end of the example shown in the figure: https://bit.ly/2Ei4X29
    * What are Android Intents used for?  
        Intent is an abstract description of an operation to be preformed or event that has happened. You can use it for starting an activity, service, bind to service, or send data via broadcast receiver.
    * Describe implicit and explicit intents  
        Explicit intents provide a component which they want to run  
        Implicit intents provide enough data to android to decide what is the most suitable component for the described task
    * How are implicit Intents resolved?  
        Android uses the data provided in the implicit intent and loops through the list of applications intent filters until it finds the one which accepts that implicit intent. Once it finds it, it calls onCreate of that activity and passes the intent to it
    * Where can IntentFilters be specified?  
        They can be specified statically in Android manifest file or dynamically during the app runtime (With kotlin or java)
    * Sketch code that calls a function doSomething() when a user clicks on a button in an Activity.  
        ```
    	    public fun onCreate(savedInstanceState: Bundle?){
                .
                .
                .
                var button = binding.myButton
                button.setOnClickListener(){ doSomething() }
            }
        ```

    * What is the MainLooper?  
        Looper keeps the thread alive in an infinite loop. MainLooper is the looper for the main (UI) thread
    * Describe the difference between match_parent and wrap_content  
        setting width/height to match_parent on element, causes it to receive same width/height as its parent  
        setting the width/height to wrap_content on element, causes element to receive sam width/height as the total width/height of its children
    * How are views organised in Android  
        They are organized in a Tree structure
    * Discuss the difference between Fragments and Activities  
        Fragments need activities in order to run. They attach to an activity and can be reused. There can also be multiple fragments in a single activity, but they can't talk to eachother directly.
    * How can we share information among different fragments of the same app (connected to the same Activity).  
        We can create an interface which the activity holding the two fragments will implement. In the two fragments we can set the object (which implements that interface) in onAttach method. 
        The other method for fragment communication is by using view models. Two fragments observe the data from a common view model. 
    * Describe the best design practices in asking users for permissions in Android applications.  
        Don't ask for permission unless you need them. Show emediate benefit of granting the permission. if the user denies a necessary permission educate them about why your app needs the permission and ask one more time.  
    * Name two different approaches to implementing concurrency in Android and briefly describe them (pick only two)  
        - Threads and handlers -> create a new HandlerThread which already contains task queue and a looper for the thread. Send tasks to it with a handler instance from your main thread and receive information 
        - Kotlin coroutines -> it is a light abstraction over threads. You define a scope and choose an already existing thread on which your task will run on (Default, Main, IO). After that you use suspend functions inside of the scopes to run    operations in background
    * What is IntentService and what is it used for?  
        IntentService is a particular kind of service which is used to do long running one-off background
        tasks and then quit. It works on a separate thread.
    * How do you handle results from IntentService?  
        You can write a broadcast receiver which will receive an intent once from the IntentService, once it completes the task.
    * What is the difference between IntentService and JobIntentService?
    * Describe the basics of AsyncTask
        AsyncTask is used for
    * You are a chief architect of a mobile sensing app that is used to help telecoms get a better idea of the LTE network coverage. The app runs a network connectivity speed test and saves the result to the local database. When a user is connected on WiFi, the app uploads the data to the server.
    * - Explain how you would implement network connectivity speed testing so that it starts when a user clicks on a button, runs the test in the background, and then shows the result back to the user, when ready.
    * - Explain how you would implement upload on the server, so that it doesn’t conflict with the regular app use.
    * You are a chief architect of a mobile music player. The app should play music even when the user is not actively using your app, even when the user is not using the phone. Which class would you use for running the music player? Why?
    * Explain Threads and Handlers
    * Which of the following is true for Service class:
        - Service by default runs on the main thread True
        - Calling an Intent in order to start a service, will, if the Service is already running, skip onCreate and just call onStart --> Maybe since there is OnStartCommand function but no onstart
        - Service can be bound to another component through onBind call True
        - Service can be run in either background or foreground True
    * What is a wake lock? Explain how to acquire it and release it.
    * Describe the main functionalities of AlarmManager  
        The main functionality of alarma manager is running periodic or one-off tasks at nearly specific time or with specific times between operations.
    * Why are tasks scheduled via WorkManager more energy efficient than tasks scheduled via AlarmManager?  
        Because tasks scheduled with work manager do not have to be executed at exact time, that is why the WorkManager can group a lot of tasks and execute them at once. This method does not wake up the device as often.
    * List and briefly describe different scales of mobile sensing applications  
        - Individual/Personal focuses on individual, his behaviour
        - Group sensing sensing common group activities
        - Urban-scale large number of people have the same application, sensing large scale data
    * Describe one application in each of the listed scale categories
        - Workout trackers
        - Student applications 
        - Covid tracking applications (OstaniZdrav)
    * Explain why background processing is important in mobile computing (in particular for mobile sensing)  
        Because it allows us to create much more complex and user friendly application. For example you wouldn't want to build a fitness tracker application from which you couldn't exit to change a song, because it will stop tracking you.
        Furthermore it allows us to capture much more data, which we can use to infer higher level concepts more easily
    * How would you design an application for detecting face-to-face conversation and frequency?  
        First of all I would need to build a classifier which lets me know if the user is talking with somebody. For this I would use microphone data transformed with FFT to frequencies to feed my machine learning model. To get the correct labels needed for learning I would prompt users to let the app know once its talking to somebody by clicking on a button (once user starts and once he ends). Once the classification accuracy of the model is high enough I would enable the detection of face-to-face conversation  
        In order to get readings from the microphone I would use AlarmManager to schedule a periodic task which would run every 2 minutes. The task would be created and registered (to AlarmManager) inside of a Foreground service in order to avoid my application being killed before the task has been registered. The task would also contain a pending intent which would be used in case a conversation has been detected. It would start an IntentService which would update the frequencie of conversations inside of the apps relational database.
    * How would you design an application for inferring sleep duration?  
        Firstly I would need to build a model to detect if user is sleeping. For this I would use microphone, light and location data. In order to train the model I would ask user to let me know when he goes to sleep and when he wakes up. Once the classification accuracy of the model is high enough I would enable sleep detection. For the data processing, I would get the mean and variance from microphone and light sensor. For location I would use Google play Location Service to get the users location.
        For sensig I would register a task with AlarmManager in order to periodically get and process the data from the sensors. I would check if the user is sleeping every 20 minutes. The task would be registered inside of foreground service in order to avoid the issue of my application being closed by the user or by the OS. Every time User starts sleeping the task would use the pending intent to start an intent service which would create a new sleep record along with the starting time of the sleep in the apps relational database. Once the user exits from sleep, I would also use the pending intent to start an intent service which would set the duration and end time of the current sleeping session.  
        The apps UI would be used to display the data from the relational database. 
    * How would you design a contact tracing app for epidemiology research? Ensure that the app is as much privacy-preserving as possible.
    * Describe adaptive duty cycling,  
        Adaptive duty cycling allows device to sleep by sensing in a defined interval. Once it detects an event it will shorten that interval and once it stops detecting events it will longer the interval until it reaches the original value. 
    * Explain what hierarchical sensor activation is.  
        In order to perserve power, the inaccurate but energy efficient sensors are activated first and if they detect the wanted event or data, other more accurate sensors will be turned on for accurate detection
    * Describe the process of inferring a smartphone user’s physical activity from sensor readings.  
        To infer physical activity we need to train a machine learning model to recognize the type of the activity. So firstly we'll ask the user to repeat a move continuously and then prompt him to write the name of that move. During execution of the move we will use the  mean, variance and mean crossing rate from gyroscope and accelorometer. Every second we would calculate those parameters and use them for training the classifier. Once the classifier is trained we can infer phyisical activities. I cannot state which ML model is best for the job but we can use random forests for example.
    * Explain how InterruptMe project uses mobile sensing and machine learning or propose own approach towards inferring interruptibility of a mobile user
    * Give an example of an Android app designed with the MVC paradigm. Exaplain what "M", "V", and "C" are in this case.
    * What is the drawback of MVC in Android? What is the alternative?
        The drawback of this model is that view and controller are tightly connected and often when updating one of them, we need to update the other as well. The alternative would be to use MVVM, which stands for Model-View-ViewModel.
    * Describe the components you would use in an app where the data are not stored in persistent storage (e.g. database, SharedPreferences), but they have to survive configuration changes (phone rotation).
        I would either use a ViewModel which survives the lifecycle changes of the activity or store the data in a bundle in OnSaveInstanceState function.
    * What is LiveData? Describe a use case for LiveData in an Android app.
        LiveData is an object which wraps some data and allows it to be observed. What is more it is also lifecycle aware so it will only notify the observer when needed.  
    * Draw a diagram and describe the data flow of a modern Android app using a Room database.
    * What is the purpose of Object-Relational Mapping?  
        It converts table entries to Kotlin/Java objects and vice versa. It makes development of applications much easier since it allows programmers to interact with database through objects and not queries.
    * Pick two wireless technologies supported by modern smartphones and discuss their range, power requirements, throughput, and list at least one application where each of the technologies might be used.  
        - NFC --> very short range, very low power consumption, very low throughput. It is used for contactless payment
        - Wifi --> medium range, medium power consumption, high throughput. Used by almost all applications which connect to the internet (example. Twitch and streaming services, since they require high throughput for good video quality)
    * What are the benefits of OkHttp versus HttpUrlConnect method for accessing remote APIs?  
        It compresses the data, it will automatically retry if the connection has failed, it takes less code to do the same thing. 
    * You are designing an app that helps a user find a place to park a car. How would you communicate the data about the spot vacancy from the server to your app in the most efficient way?  
        I would use firebase messaging. So I would probably have a system which will post to a ceratin topic on Firebase when a spot is available. Android app will subscribe to that topic (with firebase library), it will get notified and from there I can create a JobIntentService which will create a notification for the user
    * List the benefits of hybrid application development.
        You need to maintain a single code base, you do not need to have seperate teams developing for seperate platforms. This reducec the cost of development aswell as speeds up the whole development cycle for application development
    * What is the purpose of plugins in Apache Cordova?  
        Their purpose is to enable access to devices native capabilities

