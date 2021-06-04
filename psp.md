* Programming platforms:
    * Why do we have different programming platforms (as opposed to a single general purpose platform)?
    * List at least two platforms and describe the key properties of each

* Web platform:
    * Briefly describe the underlying technologies supporting the Web platform
        HTML (hyper text mark up language) is a markup language for hyper text, which is a text that points to another resource 
        HTTP -> is a client-server communication protocol where client sends the request and server responds with response. It has multiple methods: GET, POST, PUT, DELETE...
        URL -> is a unified way of referencing resources on the web 
    * What is Hypertext? Briefly describe its historical role in the Web.
        Hyper text is text that a points to another resource.
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
        He meant by this that every page stated that it works best with certain version of a certain browser. I don't think this is the case today since all of the browsers follow the standards posted by W3C and most of the world uses a chromium based browser anyway. There are ofcourse small discrepencies between different browsers but they are not noticeable for the average user, since they are mostly found in nitche application
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
        Microwave oven -- ussualy do not have software for debugging and upgrades once deployed are impossible

* Embedded platform:
    * List at least four applications of embedded computing technology (note: don’t list specific applications, but application areas)
        - agriculture
        - IoT
        - Weapons
        - Space exploration
    * What are the key properties of embedded systems?
        They tend to be specifically designed systems for a single task or operation. They are very efficient in what they do. They are programmed in low level programming languages to improve performance. Ussualy they are also resource constrained. 
    * What is a sensor?
        Sensor is a device which reads phisical properties from enviroment and converts it electrical signal
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
        They tend to have embedded systems for safety critical systems such as ABS breaking. They need to work 100% of the time and they need to respond ASAP. That is why they are seperatly developed and put in a car. On the other hand we have systems which deal with non safety critical functions such as operating radio from the stearing wheel buttons. 
    * What are the main threats for embedded systems’ wireless communication? Hint: Estrin et al. paper.
    * Why, even more so than with conventional desktop systems, we must ensure that embedded networked systems are correctly programmed?
    * “Failures we have in today’s technologies could be disastrous in embedded networked systems” warn Estrin et al. in 2001. Argue for or against this statement.
    * Discuss a potential use of embedded systems in precision agriculture.
    * Present at least one means of saving energy in an embedded system that senses the humiditiy in the field and notifies about potential floods.
    * Describe in one sentence each: IP Core, FPGA, and MCU.
    * List key properties of a sensor that you should be aware of when deciding to use one in your system.
    * Describe the basics of analogue-digital conversion (ADC).
    * List different storage components often available in an MCU. List their properties.
    * What is cross-compilation?
    * What is a toolchain?
    * What are the main differences between an embedded operting system and a conventional (desktop) operating system?
    * What is a process? What are the process states? Draw a state transition diagram.
    * Is Arduino a real-time OS?
    * Describe the following terms: input pin, output pin
    * What is the difference between analogue and digital input pin? Give an example use of an analogue input pin.
    * What are the two basic functions of an Arduino sketch? Describe their use.

* Gaming platform:
    * What is a Gaming engine?
    * What is a GPU?
        Graphics processing unit, is a special processor designed for graphicly intensive operations (such as floating point computations) operations

* Android Programming:
    * What is “sandboxing” in Android OS?
    * Explain how permissions work in Android?
    * Sketch and describe the Android compilation process.
    * A few years ago Google engineers decided to replace Dalvink, a just-in-time compiler, with ART, an ahead-of-time compiler. Briefly describe the differences and present some reasons that support the engineers’ decision.
    * What is the purpose of “res” folder in Android projects?
    * How are non-compiled application resources accessed in Android programmes?
    * Describe different means of storing data locally in Android applications
    * What is the meaning of "?" and "!!" before accessing a property of an object in Kotlin?
    * What is "smart cast" in Kotlin?
    * What is a companion object in Kotlin?
    * You are a chief architect of the next most popular app on the market - the app allows users to record videos of themselves singing and dancing over popular tunes. You have to think about data storage for different parts of the app. Decide which method to use to store the following (explain!)
    * - Video files created by the app
    * - Audio tracks used during the video generation
    * - User settings
    * What are SharedPreferences used for?
    * Activity lifecycle - draw diagram and clearly mark when activity exists, is visible, in the foreground
    * Activity lifecycle - why did engineers decide to implement that way
    * How can we save an activity state and restore it when the activity is recreated?
    * Assume that each of the lifecycle callbacks (onCreate, onStart, etc.) print an associated log message with the callback and the activity name when called (e.g. “onCreate from Activity 1”, “onStart from Activity 1”, etc.). Write one after another all the log messages that will be printed at the end of the example shown in the figure: https://bit.ly/2Ei4X29
    * What are Android Intents used for?
    * Describe implicit and explicit intents
    * How are implicit Intents resolved?
    * Where can IntentFilters be specified?
    * Sketch code that calls a function doSomething() when a user clicks on a button in an Activity.
    * What is the MainLooper?
    * Describe the difference between match_parent and wrap_content
    * How are views organised in Android
    * Discuss the difference between Fragments and Activities
    * How can we share information among different fragments of the same app (connected to the same Activity).
    * Describe the best design practices in asking users for permissions in Android applications.
    * Name two different approaches to implementing concurrency in Android and briefly describe them (pick only two)
    * What is IntentService and what is it used for?
    * How do you handle results from IntentService?
    * What is the difference between IntentService and JobIntentService?
    * Describe the basics of AsyncTask
    * You are a chief architect of a mobile sensing app that is used to help telecoms get a better idea of the LTE network coverage. The app runs a network connectivity speed test and saves the result to the local database. When a user is connected on WiFi, the app uploads the data to the server.
    * - Explain how you would implement network connectivity speed testing so that it starts when a user clicks on a button, runs the test in the background, and then shows the result back to the user, when ready.
    * - Explain how you would implement upload on the server, so that it doesn’t conflict with the regular app use.
    * You are a chief architect of a mobile music player. The app should play music even when the user is not actively using your app, even when the user is not using the phone. Which class would you use for running the music player? Why?
    * Explain Threads and Handlers
    * Which of the following is true for Service class:
        - Service by default runs on the main thread
        - Calling an Intent in order to start a service, will, if the Service is already running, skip onCreate and just call onStart
        - Service can be bound to another component through onBind call
        - Service can be run in either background or foreground
    * What is a wake lock? Explain how to acquire it and release it.
    * Describe the main functionalities of AlarmManager
    * Why are tasks scheduled via WorkManager more energy efficient than tasks scheduled via AlarmManager?
    * List and briefly describe different scales of mobile sensing applications
    * Describe one application in each of the listed scale categories
    * Explain why background processing is important in mobile computing (in particular for mobile sensing)
    * How would you design an application for detecting face-to-face conversation and frequency?
    * How would you design an application for inferring sleep duration?
    * How would you design a contact tracing app for epidemiology research? Ensure that the app is as much privacy-preserving as possible.
    * Describe adaptive duty cycling,
    * Explain what hierarchical sensor activation is.
    * Describe the process of inferring a smartphone user’s physical activity from sensor readings.
    * Explain how InterruptMe project uses mobile sensing and machine learning or propose own approach towards inferring interruptibility of a mobile user
    * Give an example of an Android app designed with the MVC paradigm. Exaplain what "M", "V", and "C" are in this case.
    * What is the drawback of MVC in Android? What is the alternative?
    * Describe the components you would use in an app where the data are not stored in persistent storage (e.g. database, SharedPreferences), but they have to survive configuration changes (phone rotation).
    * What is LiveData? Describe a use case for LiveData in an Android app.
    * Draw a diagram and describe the data flow of a modern Android app using a Room database.
    * What is the purpose of Object-Relational Mapping?
    * Pick two wireless technologies supported by modern smartphones and discuss their range, power requirements, throughput, and list at least one application where each of the technologies might be used.
    * What are the benefits of OkHttp versus HttpUrlConnect method for accessing remote APIs?
    * You are designing an app that helps a user find a place to park a car. How would you communicate the data about the spot vacancy from the server to your app in the most efficient way?
    * List the benefits of hybrid application development.
    * What is the purpose of plugins in Apache Cordova?
