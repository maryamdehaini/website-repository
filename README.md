## AWS Workshop repository

Welcome to the AWS Workshop Repository. If you wish to add a reource, please use the copy the following json object into a file, fill it out, and push it to this repository: 

    { 
        "category": "",
        "name": "",
        "tags": "",
        "time": "",
        "externallyaccessible": "",
        "level": "",
        "type": "",
        "description": "",
        "location": ""
    }
    
| Object   | Description| 
|----------|--------------------------------------------------------------------|
| Category | Main AWS concept covered by the workshop i.e. Security, data, etc. |
|Tags | Topics covered by the workshop  |
|Time | Total time needed to complete workshop |  
|Externally Accessible | Available without VPN yes or no |  
|Level | Level of lab  |
|Type | Format of lab i.e. workshop, builder session, immersion day  |
|Description | Any information/comments about the lab  |
|Location | Link to the lab  |

<body>
<form>
  <label for="category">Category: </label>
  <select id="category" name = "Category">
	<option value="" selected>Choose An Option</option>
	<option value="Data">Data</option>
	<option value="Security">Security</option>
  </select><br><br>
  <label for="name">Name:</label>
  <input type="text" id="name" name="name" value=""><br><br>
  <label for="tags" >Tags:</label>
  <input type="text" id="tags"  name="tags"  value=""><br><br>
  <label for="time" >Time:</label>
  <input type="text" id="time" name="time" value=""><br><br>
  <label for="externallyaccessible" >Externally Accessible:</label>
  <select id="externallyaccessible" name = "externallyaccessible">
	<option value="" selected>Choose An Option</option>
	<option value="Yes">Yes</option>
	<option value="no">No</option>
  </select><br><br>
  <label for="level" >Level:</label>
  <input type="text" id="level" name="level" value=""><br><br>
  <label for="wtype" >Type: </label>
  <input type="text" id="wtype" name="wtype" value=""><br><br>
  <label for="description" >Description: </label>
  <input type="text" id="description" name="description" value=""><br><br>
  <label for="location">Location:</label>
  <input type="text" id="location" name="location" value=""><br><br>
  <input type="button" onclick="myPrint()" value="Submit"></p>
</form>
	<p id="json"></p>
</body>

<script>
function myPrint(){
	document.getElementById("json").innerHTML = "{<br>    \"category\": \"" + document.getElementById("category").value + "\",<br>\"name\": \"" + document.getElementById("name").value + "\",<br> \"tags\": \"" + document.getElementById("tags").value + "\",<br> \"time\": \"" + document.getElementById("time").value + "\",<br> \"externallyaccessible\": \"" + document.getElementById("externallyaccessible").value + "\",<br> \"level\": \"" + document.getElementById("level").value + "\",<br>\"type\": \"" + document.getElementById("time").value + "\", <br> \"description\": \"" + document.getElementById("description").value + "\",<br> \"location\": \"" + document.getElementById("location").value + "\" <br>}";
}
</script>
