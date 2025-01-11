# Triple-Jump-In-Unity
this is a guide on triple jump

For this guide you will need unity. 2022.39f this is the version of unity that i will be useing.
you will aslo need  visual studio to write your code in.

The fist step is to make the player.there way to do this is by going to click on the hierarchy and you will go to 2d objects and spirte you can use triangle

The triangle will be the player.
you will aslo need to add a box colider and rigidbody 2D 
you will go to the hierarchy and add an game obeject to the player
create an empty game object. you put it at the button of your player 

![image](https://github.com/user-attachments/assets/c284faf7-4cae-419e-9e59-54d95a2f21f1)




to add this you will click on there player and go to add component 
i added an image to show yuu where it is.


![image](https://github.com/user-attachments/assets/2f64ef69-ebbf-4206-bb73-604d9acd15ab)







![image](https://github.com/user-attachments/assets/385a23d6-bad9-4366-a8c4-5358fe9ed270)



you will then need to make a scrpit for the player movement and call it player movement.
to  make a scrpit you right click. consal 



![image](https://github.com/user-attachments/assets/74129049-1c33-4408-a32d-bb0a2d4e0b4c)


once you make the scrpit make sure its is named player movement. this will help you find it much easier.

i then  made one platform and you will just copy it and paste it again change the name to platform 2, i made sure that the platforms have box colider so there player is able to walk and jump on it.

![image](https://github.com/user-attachments/assets/e1d8d5aa-a29b-41a5-b61d-2c8f7f4b089b)

to add a box colider you just need to go to add component 

![image](https://github.com/user-attachments/assets/b61f7840-45e8-41e9-8e7c-c57f8909ea06)


then click on box colider2D 

![image](https://github.com/user-attachments/assets/402db919-5227-4163-9954-cffcd471db26)

i added an image hope this will help you. find the box colider.
 after you done this then you go to your scirpt which you made ealier which is player movement you will need to open it.

 you will need to make four privte variables
 which are a Private float horizontal
 private float speed and jumping power and
 private bool is faceing right.

 i added a picture to help you.

 ![image](https://github.com/user-attachments/assets/9f4bddc7-b90d-445c-9532-dbe7474cd58f)


 after you need 3 serialized fields to refernce the rigid body and the ground check and groud layer.

 once you finshed  that you will need to go to update void on the code and write code i will provide an image.

 
 
 ![image](https://github.com/user-attachments/assets/9d7af01a-de4e-4f33-abf1-ac87bbfa83a3)

this is the code that will move the player 


 ![image](https://github.com/user-attachments/assets/ca2d8fd1-35fb-4c15-a72e-39555b7f59fa)

 after you finish  this part of the code you will then need tto go to the jumping part.
 to make the triple jump.

 you will need to haed to the area of the code which is responsble for jumping.

 ![image](https://github.com/user-attachments/assets/d3dfbef7-6369-49f3-b5c7-a14aff39210a)

 which can be seen in the image above.

 you need to decalre three private variables  which are 1 a Boolean that indicates whether our player is already jumping and an integer for the maximum number of jump 
 this will control how many times you can jump.
 you will also need to add and an intenger for the number of remaining jumps,


 ![image](https://github.com/user-attachments/assets/7b048323-1ce7-48ec-a305-30e6bee1aef7)





in the update method whenever our player  is grounded and  and we are not pressing the jumping button  we set is jumping to false and  reset the number of remaining jumps  to the maximum number of jumps

![image](https://github.com/user-attachments/assets/00baff54-37c0-482b-bf41-d4af3048de55)


now every  time we press the jump button  we check if our player is  grounded or  if jumping is true and the number of remaining jumps is grater  than zero  and as soon as our player jumps  we set is jumping to ture
and subtract 1 from the remaining  jumps using decrement operator







