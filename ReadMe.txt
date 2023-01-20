.NET MAUI Data Binding


With that app we use Data Binding to send property from an object to a label.

We use mainly the Binding built in class.


The code:


var person = new Person { Name = "Katsavaros", Phone = "99999", Address = "X Address" }; // Create an instance of the class.


// Create our first Binding as part of our application.        

Binding personBinding = new Binding();    // There is a class called Binding.

personBinding.Source = person;            // What is the source of information.
personBinding.Path = "Phone";             // Which property?

txtName.SetBinding(Label.TextProperty, personBinding);




Katsavaros Konstantinos

