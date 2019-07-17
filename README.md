<h1><b>How to show chatbot?</b></h1>

 open build.gradle project, add maven { url "https://jitpack.io" } and mavenCentral() at the repositories

     allprojects {
             repositories {
             google()
             jcenter()
             maven { url "https://jitpack.io" }
             mavenCentral()
             }
     }

open build.gradle app and implementation :

     implementation 'com.github.achmadabrar:libchatbotvouch:1.0.0'

add ChatActivity on your click listener. Examples :

     yourbuttonid.setOnClickListener {
         startActivity(Intent(this, ChatActivity::class.java))
     }

3rd party library by Naoyuki Kanezawa:

      com.github.nkzawa:socket.io-client:0.5.0
