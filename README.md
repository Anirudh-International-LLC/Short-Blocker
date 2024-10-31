# Short-Blocker
After making a website blocker as an extension for google chrome to block ourselves from viewing excessive short form content. We slowly began to transition from watching the short form content on our phones instead of our computers. So we have found a smaller Alternative (Hopefully). Over the next few weeks, we will update it here. In this project though, we are only dealing with Android Phones, as None of us have iPhones.





# The way it works
The Premise is simple, On youtube the app, the short form and long form content both use google's CDN, so they will make a DNS request to google's CDN network, the CDN network will be the first DNS request, but if its any normal youtube video, it will show hyperlinks (recommends) other videos along with the thumbnail. We have foundout that the thumbnails are on a separate DNS altogether, so, if a DNS request for gstatic.com fails to materialize, we can be sure we are viewing short content and then use androids built-in features to close the app. 



# Potential Issues
Users with very low speeds might suffer issues with this approach, as it might take more than the time alloted by the script , to be able to send a DNS request to the thumbnail server. 
