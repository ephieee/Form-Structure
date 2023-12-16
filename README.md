# Form-Structure

<form>
Form controls live inside a <form> element. This element should always carry the action attribute and will usually have a method and id attribute too.
  action 
Every <form> element requires an action attribute. Its value is the URL for the page on the server that will receive the information in the form when it is submitted.
  method
Forms can be sent using one of two methods: get or post.
  
With the get method, the values from the form are added to the end of the URL specified in the action attribute. The getmethod is ideal for:
● short forms (such as search 
boxes)
● when you are just retrieving 
data from the web server (not sending information that 
should be added to or deleted 
from a database)

With the post method the values are sent in what are known as HTTP headers. As a rule of thumb you should use the post method if your form:
● allows users to upload a file
● is very long
● contains sensitive data (e.g. passwords)
● adds information to, or deletes information from, a database
If the method attribute is not used, the form data will be sent using the get method.

id
We look at the id attribute on page 183, but the value is used to identify the form distinctly from other elements on the page (and is often used by scripts — such 
as those that check you have entered information into fields that require values).

<form action="http://www.example.com/subscribe.php" method="get">
  <p>This is where the form controls will appear.
  </p>
</form>
