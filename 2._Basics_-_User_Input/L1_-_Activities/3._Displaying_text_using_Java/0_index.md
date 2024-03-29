# 3. Displaying text using Java
Created Friday 30 October 2020


* Java code is run as methods. It is not like JavaScript.
* Specify the callback method in the ``onClick`` attribute. The callback executes on clicking.
* This callback function must be ``public`` have one ``View`` argument.
* The argument passed(by the app) to the callback function is the host view itself(having the 'onClick' attribute). This makes it easy to interact with the host view, we don't have to locate it using an ``id``.


*****


#### Understanding Java code

* onCreate() function runs as soon as our app is started.
* It injects the views on the screen.

	package com.example.justjava;
	
	import androidx.appcompat.app.AppCompatActivity;
	
	import android.os.Bundle;
	import android.view.View;
	import android.widget.TextView;
	
	import java.text.NumberFormat;
	
	public class MainActivity extends AppCompatActivity {
	
	    @Override
	    protected void onCreate(Bundle savedInstanceState) {
	        super.onCreate(savedInstanceState);
	        setContentView(R.layout.activity_main);
	    }
	
	    /**
	     * This method is called when the order button is called
	     */
	    public void submitOrder(View view) {
	        display(011);
	        displayPrice(23);
	    }
	
	    /**
	     * This method displays the given quantity value on the screen.
	     It is set as an onClick attribute
	     Note that onClick needs a function name, and not code. The function will be executed when the button is clicked.
	     */
	    private void display(int number) {
	        TextView quantityTextView = (TextView) findViewById(R.id.quantity_text_view);
	        number += 1;
	        quantityTextView.setText("" + number);
	    }
	
	    /**
	     * This method displays the given price on the screen.
	     */
	    private void displayPrice(int number) {
	        TextView priceTextView = (TextView) findViewById(R.id.price_text_view);
	        priceTextView.setText(NumberFormat.getCurrencyInstance().format(number));
	    }
	
	}

the XML
![](./3._Displaying_text_using_Java/pasted_image.png)

the app, intial and after clicking the button.
![](./3._Displaying_text_using_Java/pasted_image001.png)  ![](./3._Displaying_text_using_Java/pasted_image002.png)

*****

The TextView changes size according to the text, because it set to wrap_content.

