# NationalUniversitySGPACalculator
National Unversity Bangladesh, SGPA Caclculator is one kind of Calculator Which is Specially Made for National University Computer Science and Engineering Students it. it Calculates Each Semester Subject Result and give the the overall SGPA. It has also a Feture, It give some Resourse Basis of your Result, Like as If your SGPA is less than 3.0 it give a Button, which contains some link of Learning/Study Site
and also give Comment.
and it has also a Special Feture, which is to print your result in Text Format 

##Code Description:
 
          
         if(Result>=3.80 && Result<=4.00){
          comtMark.setText("Briliant Result, The Result Say That You Are Very Serious In Your Study Go on");
          comtMark.setForeground(java.awt.Color.blue);
          reSrc.setVisible(false);
          //comtSug.setText("You are Very Serious In your Study Best Of Luck");
        }else if(Result>=3.40 && Result<=3.79){
          comtMark.setText("Very Good Result, You Try Your Best, Go On");
          comtMark.setForeground(java.awt.Color.DARK_GRAY);
           reSrc.setVisible(false);
          //comtSug.setText("You are Very Serious In your Study Best Of Luck");
        }
 like in this Result is the variable which store the SGPA, and give the comment and resourses of Matching with Logic
 and,
 The Formula of calculating SGPA : 
        add = put*cre1;
        add2= put*cre2;
        .....
        .....
        .....
        addn=put*cren;
        
        addCre = cre1 + cre2 + cre3 + cre4 + cre5 + cre6 + cre7 + cre8 + cre9 + cre10 + cre11;
        Result = (add + addTwo+ addThree + addFour + addFive + addSix + addSeven + addEight + addNine + addTen + addTwelve)/(addCre);
        
here "addcre" is Total credit hour & cre1.cre2,cre3.......are the credit value and add1, add2, add3......are give the value of multiply the value of Java ComboBox Value which is denoted by put nad creditValue
   if(name.getText().equals("")){
          JOptionPane.showMessageDialog(null,"Type your name Before Genarating & Printing Your Mark Sheet/Log!");
        }
        else if(resultDisp.getText().equals("")){
          JOptionPane.showMessageDialog(null,"I Think You do Not Calculate Your Result! Calculate Now Than Print");
        }
        else if(resultDisp.getText().equals("NaN")){
          JOptionPane.showMessageDialog(null,"I Think Your Result is [Nan]! Properly Calculate and Print");
        }
        else{
        
        String fileWrite = name.getText()+".txt";
        try {
            BufferedWriter writer ; 
             
            writer = new BufferedWriter (new FileWriter(fileWrite));
            
            writer.write("Mark Sheet Log Prepared By National University SGPA Calculator");
            writer.newLine();
            writer.newLine();
            //For Name Write
            writer.write("Your Name:"+" "+name.getText());
            writer.newLine();
            writer.newLine();
            //For Sub1
            writer.write("Subject 1 Grade: " +(String) subOne.getSelectedItem());
            writer.write("   ");
            writer.write("Subject 1 Credit Hour: " +(String) subOneCre.getSelectedItem());
            writer.newLine();
            //For Sub2
            writer.write("Subject 2 Grade: " +(String) subTwo.getSelectedItem());
            writer.write("   ");
            writer.write("Subject 2 Credit Hour: " +(String) subTwoCre.getSelectedItem());
            writer.newLine();
            //For Sub3
            writer.write("Subject 3 Grade: " +(String) subThree.getSelectedItem());
            writer.write("   ");
            writer.write("Subject 3 Credit Hour: " +(String) subThreeCre.getSelectedItem());
            writer.newLine();
            //For Sub4
            writer.write("Subject 4 Grade: " +(String) subFour.getSelectedItem());
            writer.write("   ");
            writer.write("Subject 4 Credit Hour: " +(String) subFourCre.getSelectedItem());
            writer.newLine();
            //For Sub5
            writer.write("Subject 5 Grade: " +(String) subFive.getSelectedItem());
            writer.write("   ");
            writer.write("Subject 5 Credit Hour: " +(String) subFiveCre.getSelectedItem());
            writer.newLine();
            //For Sub6
            writer.write("Subject 6 Grade: " +(String) subSix.getSelectedItem());
            writer.write("   ");
            writer.write("Subject 6 Credit Hour: " +(String) subSixCre.getSelectedItem());
            writer.newLine();
            //For Sub7
            writer.write("Subject 7 Grade: " +(String) subSeven.getSelectedItem());
            writer.write("   ");
            writer.write("Subject 7 Credit Hour: " +(String) subSevenCre.getSelectedItem());
            writer.newLine();
            //For Sub8
            writer.write("Subject 8 Grade: " +(String) subEight.getSelectedItem());
            writer.write("   ");
            writer.write("Subject 8 Credit Hour: " +(String) subEightCre.getSelectedItem());
            writer.newLine();
            //For Sub9
            writer.write("Subject 9 Grade: " +(String) subNine.getSelectedItem());
            writer.write("   ");
            writer.write("Subject 9 Credit Hour: " +(String) subNineCre.getSelectedItem());
            writer.newLine();
            //For Sub10
            writer.write("Subject 10 Grade: " +(String) subTen.getSelectedItem());
            writer.write("   ");
            writer.write("Subject 10 Credit Hour: " +(String) subTenCre.getSelectedItem());
            writer.newLine();
            //For Sub11
            writer.write("Subject 11 Grade: " +(String) subTwelve.getSelectedItem());
            writer.write("   ");
            writer.write("Subject 11 Credit Hour: " +(String) subTwelveCre.getSelectedItem());
            writer.newLine();
            writer.newLine();
           //For Result
            
            writer.write("Your Result: " +resultDisp.getText());
            writer.newLine();
            
           //For Comment
            writer.newLine();
            writer.write("Best Of Luck");
           
            
            writer.close();
            
            JOptionPane.showMessageDialog(null, "Your Result Printed Successfully! You can get Your File where Your Application is Situated");
        } catch (Exception e) {
        }
        
 this code is responsible for write students result in the text file. in this code i use java BufferWritter class and store the result in text file separately basis of each students name. if i type my name Avi in Type Name jtextfield it store the Avi.txt file 
