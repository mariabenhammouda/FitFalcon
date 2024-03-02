# FitFalcon
Globally, there has been an increase in the attainment of gym memberships, and the emphasis on fitness routines and health coaching has far surpassed ever before. However, as more people utilize the gym for their daily exercises, proper form, correct and safe equipment usage has become significantly vital for an overall successful fitness experience.
According to the National Safety Council (NSC), in 2019 “personal exercise, with or without exercise equipment, accounted for about 468,000 injuries below the category of exercise and exercise equipment”
Fitness instructors cite the following reasons for gym-related injuries:
Inattention due to cell phones or other distractions.
Using equipment for the first time without proper instruction
Working out too hard, too soon after a period of inactivity.

While personal trainers are available, they remain an expensive option. Moreover, most people are already committed to gym membership payments and personal trainers may be economically overwhelming. In collaboration with the NYUAD athletics department, the FitFalcon app acts as a portable gym partner.

Purpose -
Decrease gym injuries by indicating the proper form and technique of gym equipment and machines
Ease overall gym-intimidation by providing a personal gym companion 
Provide information on the different types of equipment and their uses.

Target Users - 
This app is designed for members of the NYUAD community who prioritize their health and are interested in gym workouts, irrespective of their current fitness level or ability.

How to Use FitFalcon - 
Select your avatar, then point your phone camera onto the user guide image usually located on the side of the gym machine. Once the gym equipment is recognized by the application, you will be directed to a page with information on the machine and the application’s recommended workouts. Read the information provided about the equipment and select the type of exercise you are willing to do on that piece of equipment. Browse through the front, back, and side previews using the “next preview” button. Follow the avatar's movements for a safe exercise routine. Once you have completed the exercise you may choose between returning to the Camera and directing it to another equipment to perform the next exercise or you may exit through the exit button.

Features:
-Useful description of the equipment
- Information on proper workout posture
- Detailed animation guide
- Recommended workouts based on equipment detected

How does FitFalcon work-
According to your character selection, our algorithm will generate an avatar that performs  the exercise movements with proper form based on the user guide image you direct your camera toward. The user guide image is usually located on the side of the gym equipment. The user guide image usually provides a brief description of the muscles targeted by the equipment and has a picture of the equipment on it. Below is an example of the user guide image on one of the NYUAD gym equipment.

![Screen Shot 2024-03-02 at 8 06 25 AM](https://github.com/mariabenhammouda/FitFalcon/assets/102983688/59fd4823-6d7b-4253-b042-75e52a80ce4d)

The application aims to include the following functionalities: 
Play animations of the workout, 
interaction with the user. 
An interactive experience with the real-world environment and accurate image detection.
To achieve the animation functionality, we used the website, Mixamo.  Mixamo has a wide range of characters and animations to select from. Both male and female characters were implemented to provide the user with a personalized experience.
The following animations were downloaded from the site:
-Overhead squat 
-Kettlebell swing 
-Front raises 
-Running 
-Walking 
-Bicep curls
Animation controllers for each of the exercises were then created. 

The gym machines were imported from a Unity built-in asset named “BodyBuilder asset pack”. The asset pack includes dumbbells, kettlebells, a squat rack, barbells, a preacher curl bench, and a leg press. The equipment was attached to the animations by adding the equipment as a child to the hand prefab and then adjusting the dimensions, size, and angles to best suit.

To enable Interactions with the user buttons with various functionalities were implemented. Some scenes prompt the user to select a character, type of workout, and the camera preview. To create an interactive experience in the real-world environment, the application uses Ar foundation packet and Vuforia Engine, a platform for AR development and image detection. An image is uploaded to the Vuforia database. The Target Manager processes the images to generate both data and visual representations of the target’s features. The image target function detects the image by comparing extracted natural features from the camera image against a known target resource database. For this application, the code changes scenes once the image is detected successfully.
The application supports both portrait and landscape modes for devices. The application allows for a swift transition back and forth between the animation and the AR camera. In any of the scenes, once the user clicks on Quit the application terminates.
The algorithm is catered for the following user guide images:

Squat Rack:

![Screen Shot 2024-03-02 at 8 09 52 AM](https://github.com/mariabenhammouda/FitFalcon/assets/102983688/e165dadd-f197-48c6-bbfb-0a96e79684c4)

Treadmill:

![Screen Shot 2024-03-02 at 8 10 00 AM](https://github.com/mariabenhammouda/FitFalcon/assets/102983688/600ed289-9d02-4d58-b76e-00fa675ea081)

Dumbbell rack:

![Screen Shot 2024-03-02 at 8 10 07 AM](https://github.com/mariabenhammouda/FitFalcon/assets/102983688/aa3ad8e8-597b-49d6-b9d5-ddb28abd59f2)

Kettlebell Rack:

![Screen Shot 2024-03-02 at 8 10 15 AM](https://github.com/mariabenhammouda/FitFalcon/assets/102983688/307a31e6-9032-457e-98bf-e4938ff10d98)


The following are snapshots of the application functionalities:

      Main menu:                    AR camera:                  Workout Menu:     
![Screen Shot 2024-03-02 at 8 10 38 AM](https://github.com/mariabenhammouda/FitFalcon/assets/102983688/e58d4161-a954-432d-8131-bdeea9929c03)

Animation: 

![Screen Shot 2024-03-02 at 8 10 43 AM](https://github.com/mariabenhammouda/FitFalcon/assets/102983688/4158398c-168c-4c03-89dd-ed0bc7943c25)

The project can be accessed via the following link: https://drive.google.com/file/d/1n_kv8a5_mr6nwFeJAnC0515y3921kQgs/view?usp=sharing
