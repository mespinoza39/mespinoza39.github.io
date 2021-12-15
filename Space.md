
<html lang="en">
<script>
    var myAudio = new Audio('https://github.com/mespinoza39/Assignment-UAT-Space-Program---We-Have-SOUND-/blob/main/The_X_Files_theme.mp3?raw=true');

// Create the function to enable stop button and disable start buton
function start(){
    //change the start button  by getElementByID. Disable it by making value trye
    document.getElementById("startButton").disabled = true;
    //Similar to top portion, except false to enabe
    document.getElementById("stopButton").disabled = false;
    //Actually have the audio play
    myAudio.play();
}
//Create function to enable start and disable stop
function stop(){
    //Similar to top function
    document.getElementById("startButton").disabled = false;
    document.getElementById("stopButton").disabled = true;
    myAudio.pause();
    myAudio.currentTime = 0;
}
</script>
<style>
#logo{

    /* Chooses where to put image and attempt to remove border */
   float: left;
  height: 75px;
  width: 235px;
  border-style: none;
  border: 0;
}
#Title {
    /* Put the text near the image, add padding to designate where */
  float:left;
  padding-top: 85px;
  padding-left: 10px;
}
body { 
    /*Make the background go from white to sky blue */
    background-image: linear-gradient(90deg, white, skyblue);
}

table{
    /*Add the border to the table */
    border: 1px solid black;
}
th, td{
    /*Add border to all columns and fill the table */
    width: 20%;
    border: 1px solid black;
    text-align: left;
}
#tble{
    /*Changes where table is */
    padding-top: 260px;
}
button{

    /*Make the buttons pill shaped and add the gradient color */
    background-color: white;
  border: linear-gradient(90deg, white, skyblue);
  padding: 7px 35px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  margin: 4px 2px;
  cursor: pointer;
  border-radius: 16px;
}
</style>

<head>
    <!-- Get the image for web page-->
<div id ="logo">
    <img src="https://github.com/mespinoza39/Assignment-Event-Driven-Programming---Buttons/blob/main/UATspaceLogo.jpg?raw=true">
</div>
<div id = "Title">
    <!-- Add Title -->
    <h1> UAT Space Program </h1>
</div>  
    <title>Table</title>
</head>
<!-- Change backgtound color and add space to allow for table to be on left-->
<body>
    <p2>
        <!-- Required to have borders for cells-->
    <div id="tble">
    <table>
        <tr>
            <th> <b>Data Type</b></th>
            <th> <b>Reading</b> </th>
        </tr>
        <tr> 
            <!-- Adding data for table-->
            <td> Time elapsed: </td>
            <td> 15 Seconds</td>
        </tr>
        <tr> 
            <td> Latitud: </td>
            <td> 0</td>
        </tr>
        <tr> 
            <td> Longitude: </td>
            <td> 0 </td>
        </tr>
        <tr> 
            <td> GPS Altitude: </td>
            <td> 0 </td>
        </tr>
        <tr> 
            <td> BMP Sensor Altitude: </td>
            <td> 30383.04</td>
        </tr>
        <tr> 
            <!-- Still adding data for table-->
            <td> BMP Sensor Pressure: </td>
            <td> 2.34</td>
        </tr>
        <tr> 
            <td> BMP Sensor Temperature: </td>
            <td> 0</td>
        </tr>
        <tr> 
            <!-- use some CSS to give more whitespace in between the cells-->
            <td> Digital Sensor Temperature: </td>
            <td> 24.12</td>
        </tr>
        <tr> 
            <td> CSS Sensor Temperature: </td>
            <td> 25/td>
        </tr>
        <tr> 
            <td> CSS Sensor eCO2: </td>
            <td> 400</td>
        </tr>
        <tr> 
            <td> CSS Sensor TVOC: </td>
            <td> 0</td>
        </tr>
        <tr> 
            <td> UV: </td>
            <td> 0 </td>
        </tr>
        <tr> 
            <td> Accel X: </td>
            <td> -0.87</td>
        </tr>
        <tr> 
            <td> Accel Y: </td>
            <td> -0.02</td>
        </tr>
        <tr> 
            <td> Accel Z: </td>
            <td> 9.61</td>
        </tr>
        <tr> 
            <!-- Adding data for table-->
            <td> Magnetix X: </td>
            <td> 0.13</td>
        </tr>
        <tr> 
            <td> Magnetic Y: </td>
            <td> 0.57</td>
        </tr>
        <tr> 
            <td> Magnetic Z: </td>
            <td> -0.24</td>
        </tr>
        <tr> 
            <td> Gyro X: </td>
            <td> 4.66</td>
        </tr>
        <tr> 
            <td> Gryo Y: </td>
            <td> 0.01</td>
        </tr>
        <tr> 
            <td> Gyro Z: </td>
            <td> -0.4</td>
        </tr>

    </table>
    </div>
    </p2>
    <!-- Create the buttons and have them call the function-->
    <p3><br></p3>
    <p4> <button id="startButton" type="buton" onclick="start()">Start</button> </p4>
    <!-- Same as above but for stop button-->
    <p5> <button id="stopButton" type="button" onclick="stop()" disabled>Stop</button> </p5>

</body>
</html>
