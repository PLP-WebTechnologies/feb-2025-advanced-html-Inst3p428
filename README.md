# Advanced HTML5 Elements and Forms

## Objectives
Implement HTML5 images, lists, tables, forms and input types.
Use form validation attributes.
Apply multimedia elements such as audio and video.

## Instructions

- Create an index.html file.
- Add an ordered list with roman numerals
- Add an external image from pexels.com
- Add a table of 5 contacts with; name, address, mobile and emails
- Add a registration form

>[!NOTE]
>  The registration form should have:
>- Name, email, password, and date fields.
>- A dropdown, radio buttons, and checkboxes.
>- Proper labels and placeholders.
>- Required fields and validation attributes.
>- Ensure proper indentation and commenting.
 
# Tasks
- Create a well-structured HTML5 document.
- Ensure semantic correctness.

Happy Coding! 💻✨
<!DOCTYPE html>
<html>
    <head>
        <title> WEEK TWO WEB DEV ASSIGNMENT </title>
        <style>
        body {
            alt: "Audi s1 Quattro and Audi Hoonitron";
            background-image: url('audi.jpg');
            background-size: cover;
            background-position: center;
            background-repeat: no-repeat;
            height: 100vh; /* Ensures the body takes the full viewport height */
            margin: 0; /* Removes default margin */
        }
        li {
            color: white;
        }
        table,th,td{
            border: 2px solid black;
            color: white;
        }
        legend{
            color:  solid black;
        }
        audio{
            position: fixed;
            top: 10px;
            right: 10px;
            z-index: 1000;
            background-color: transparent;
        }
        video{
            position: fixed;
            bottom: 10px;
            right: 10px;
            z-index: 1000;
        }
    </style>
    </head>
    <body>
        <h2 style="color: white;"> AUDI S1 QUATTRO </h2>
        <h4 style="color: white;">Key Features & Specs</h4>
        <ol type="I">
            <li>  Engine: 2.0 TFSI turbocharged petrol engine .</li>
            <li> Power Output – 231 horsepower</li>
            <li> Torque –  370 Nm</li>
            <li> Transmission: 6-speed manual gearbox.</li>
            <li> Drivetrain: Quattro all-wheel drive system</li>
            <li> Weight – Around 1,315 kg</li>
            <li>  0-100 km/h – 5.8 seconds</li>
        </ol>
        <table style="width: 50%;">
            <tr>
                <th>name</th>
                <th>address</th>
                <th>mobile</th>
                <th>emails</th>
            </tr>
            <tr>
                <td>Michele Mouton</td>
                <td>12 Bonhomie Court</td>
                <td>08232435645</td>
                <td>Michmout@gmail.com</td>
            </tr>
            <tr>
                <td>Walter Röhrl</td>
                <td>13 Rohl St</td>
                <td>0812423432</td>
                <td>Waltro21@gmail.com</td>
            </tr>
            <tr>
                <td>Hannu Mikkola</td>
                <td>1st Mannu Drive</td>
                <td>0812324352</td>
                <td>Michmout@gmail.com</td>
            </tr>
            <tr>
                <td>Carlos Sainz</td>
                <td>2014 Forest Drive</td>
                <td>08102325343</td>
                <td>CarSainz88@gmail.com</td>
            </tr>
            <tr>
                <td>Mattias Ekström </td>
                <td>14 Hill Drive</td>
                <td>08096895463</td>
                <td>Michmout@gmail.com</td>
            </tr>
        </table>
        <br/>
        <form >
            <fieldset style="width: 25%;">
                <fieldset style="width: 40%;">
                    <legend>Personal Information</legend>
                    <input type="text" name="Name" required placeholder="Enter your name">
                    <input type="email" name="useremail" required placeholder="Enter email">
                    <input type="password" name="password" minlength="8" maxlength="12" required placeholder="Your password">
                    <br><input type="radio" id="male" name="Gender" value="MALE">
                    <label for="male">MALE</label>
                    <br><input type="radio" id="female" name="Gender" value="FEMALE">
                    <label for="female">FEMALE</label>
                </fieldset>
                <fieldset style="width: 40%;">
                    <legend>Other Information</legend>
                    <input type="text" name="Date" placeholder="Enter Date">
                    <select name="Occupation" aria-placeholder="Your Occupation">
                    <option value="Engineer">Engineer</option>
                    <option value="Data.A">Data Analyst</option>
                    <option value="Doc">Doctor</option>
                    <option value="R.D">Rally Driver</option>
                    </select>
                    <br/><input type="checkbox" id="vehicle1" name="vehicle1" value="Audi s1">
                    <label for="vehicle1"> I have an Audi s1</label><br>
                    <input type="checkbox" id="vehicle2" name="vehicle2" value="Audi s2">
                    <label for="vehicle2"> I have an Audi s2</label><br>
                    <input type="checkbox" id="vehicle3" name="vehicle3" value="Audi s3">
                    <label for="vehicle3"> I have a Audi s3</label><br>
               
                </fieldset>
                <input type="submit" value="Submit" style="padding: 1%;">
            </fieldset>
        </form>
        <audio controls>
            <source src="multimedia/audis1quattro.mp3" type="audio/mpeg">
            Your browser does not support the audio element.
        </audio>
        <video width="300" height="240" controls>
            <source src="multimedia/audi s1 quattro.mp4" type="video/mp4">
          Your browser does not support the video tag.
          </video>
    </body>
</html>
