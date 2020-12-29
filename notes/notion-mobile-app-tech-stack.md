# Notion mobile app tech stack

I wondered how Notion app is implemented.

Googled a bit and found a [reddit post](https://www.reddit.com/r/Notion/comments/dz5li1/what_programming_language_is_notion_written_in/) in which it says that they seem to be using React Native. But in their github they forked the react native webview library and I was like: but why?

Simply enough, the app is indeed a webview but how do you support a webview on both platforms? Cross-platfrom webview framework. At the time when notion had an app, Flutter did not exist, so the choice was obvious. 

