
![1](https://github.com/Rishiv1000/Dice-Game-using-Simple-Javascript/assets/114014651/3b4f32d3-56ed-4200-95a0-afe0422c97de)
![Screenshot 2023-10-27 130724](https://github.com/Rishiv1000/Dice-Game-using-Simple-Javascript/assets/114014651/f628d138-ac62-457a-9090-181b90f2e7ab)
![Screenshot 2023-10-27 130642](https://github.com/Rishiv1000/Dice-Game-using-Simple-Javascript/assets/114014651/c9dc1221-0946-40ef-9da7-ba5c39d21284)

Step 1 - We Create Html File

step 2 - In index.js file ,
       var random1 = Math.floor(Math.random()*6) + 1;

       var random2 = Math.floor(Math.random() *6) + 1; 

step 3 - Access Random Image From random number

        var src1 = "images/dice" + random1 + ".png";
        var src2 = "images/dice" + random2 + ".png"; 

step 4- Select Img Element From Document

     var image1 = document.querySelectorAll("img")[0];   

     var image2 = document.querySelectorAll("img")[1];
       

     ////** id or Class Se Bhi Ho Jata Hai Tabhi index [0] ,[1] use Kara hai **//

Step 5 - Change Image With Set Attribute

           
      var image1 = document.querySelectorAll("img")[0];
      image1.setAttribute( "src" , src1);

      var image2 = document.querySelectorAll("img")[1];
      image2.setAttribute("src", src2);


Step 6 - Make IF ELSE Condition For Winner and Change Background Colour

       
      if(random1>random2){
           document.querySelector('h1').innerText= "win 1"
           document.body.style.backgroundColor = "green";
      }
      else if (random2>random1){
           document.querySelector('h1').innerText= "win 2";
           document.body.style.backgroundColor = "blue";
      }
      else {
      document.querySelector('h1').innerText= "draw !";
      }


 
      
       

        
       





        
