# Progress Button Android

Android Button that morphs into a loading progress bar. 

  - Fully customizable in the XML
  - Really simple to use.
  - Makes your app looks cooler =D

## Installation

    compile 'br.com.simplepass:loading-button-android:1.1.0'

## How to Use / Sample
Add the button in your layout file and customize it the way you like it.

   

    <br.com.simplepass.loading_button_lib.CircularProgressButton
    	    android:id="@+id/btn_id"
    	    android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:background="#FFF"
            app:spinning_bar_width="4dp" <!-- Optional -->
            app:spinning_bar_color="#FFF" <!-- Optional -->
            app:spinning_bar_padding="6dp" <!-- Optional -->

Then, instanciate the button

        CircularProgressButton btn = (CircularProgressButton) findViewById(R.id.btn_id)

        btn.startAnimation();
        
    [do some async task. When it finishes]

		btn.stopAnimation(); 
		btn.revertAnimation();

And that's it! Enjoy!

## Bugs and Feedback


For bugs, feature requests, and discussion please use [GitHub Issues](https://github.com/leandroBorgesFerreira/LoadingButtonAndroid/issues).

## Credits



This libs was inspired in this repo: https://github.com/dmytrodanylyk/android-morphing-button

## License
The MIT License (MIT)

Copyright (c) 2015 Danylyk Dmytro

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.