# Calculator
Build and design a graphical user interface calculator.

/**
 * Initializes the variables for Calculator
 */
double firstnum = 0.0;
double secondnum = 0.0;
double result = 0.0;
String operation;


public Calculator() {
    initComponents();
}

private void initComponents() {

    jtxtDisplay = new javax.swing.JTextField();
    jBtn1 = new javax.swing.JButton();
    jBtn2 = new javax.swing.JButton();
    jBtn3 = new javax.swing.JButton();
    jBtn5 = new javax.swing.JButton();
    jBtn4 = new javax.swing.JButton();
    jBtn6 = new javax.swing.JButton();
    jBtn8 = new javax.swing.JButton();
    jBtn7 = new javax.swing.JButton();
    jBtn9 = new javax.swing.JButton();
    jBtn0 = new javax.swing.JButton();
    jBtnDecimal = new javax.swing.JButton();
    jBtnPlusMinus = new javax.swing.JButton();
    jBtnClear = new javax.swing.JButton();
    jBtnAdd = new javax.swing.JButton();
    jBtnSubtract = new javax.swing.JButton();
    jBtnDivide = new javax.swing.JButton();
    jBtnMultiply = new javax.swing.JButton();
    jBtnEqual = new javax.swing.JButton();

    setDefaultCloseOperation(javax.swing.WindowConstants.EXIT_ON_CLOSE);

    jtxtDisplay.setFont(new java.awt.Font("Tahoma", 1, 24)); // NOI18N
    jtxtDisplay.setHorizontalAlignment(javax.swing.JTextField.RIGHT);

    jBtn1.setFont(new java.awt.Font("Tahoma", 1, 24)); // NOI18N
    jBtn1.setText("1");
    jBtn1.addActionListener(new java.awt.event.ActionListener() {
        public void actionPerformed(java.awt.event.ActionEvent evt) {
            jBtn1ActionPerformed(evt);
        }
    });

    jBtn2.setFont(new java.awt.Font("Tahoma", 1, 24)); // NOI18N
    jBtn2.setText("2");
    jBtn2.addActionListener(new java.awt.event.ActionListener() {
        public void actionPerformed(java.awt.event.ActionEvent evt) {
            jBtn2ActionPerformed(evt);
        }
    });

    jBtn3.setFont(new java.awt.Font("Tahoma", 1, 24)); // NOI18N
    jBtn3.setText("3");
    jBtn3.addActionListener(new java.awt.event.ActionListener() {
        public void actionPerformed(java.awt.event.ActionEvent evt) {
            jBtn3ActionPerformed(evt);
        }
    });

    jBtn5.setFont(new java.awt.Font("Tahoma", 1, 24)); // NOI18N
    jBtn5.setText("5");
    jBtn5.addActionListener(new java.awt.event.ActionListener() {
        public void actionPerformed(java.awt.event.ActionEvent evt) {
            jBtn5ActionPerformed(evt);
        }
    });

    jBtn4.setFont(new java.awt.Font("Tahoma", 1, 24)); // NOI18N
    jBtn4.setText("4");
    jBtn4.addActionListener(new java.awt.event.ActionListener() {
        public void actionPerformed(java.awt.event.ActionEvent evt) {
            jBtn4ActionPerformed(evt);
        }
    });

    jBtn6.setFont(new java.awt.Font("Tahoma", 1, 24)); // NOI18N
    jBtn6.setText("6");
    jBtn6.addActionListener(new java.awt.event.ActionListener() {
        public void actionPerformed(java.awt.event.ActionEvent evt) {
            jBtn6ActionPerformed(evt);
        }
    });

    jBtn8.setFont(new java.awt.Font("Tahoma", 1, 24)); // NOI18N
    jBtn8.setText("8");
    jBtn8.addActionListener(new java.awt.event.ActionListener() {
        public void actionPerformed(java.awt.event.ActionEvent evt) {
            jBtn8ActionPerformed(evt);
        }
    });

    jBtn7.setFont(new java.awt.Font("Tahoma", 1, 24)); // NOI18N
    jBtn7.setText("7");
    jBtn7.addActionListener(new java.awt.event.ActionListener() {
        public void actionPerformed(java.awt.event.ActionEvent evt) {
            jBtn7ActionPerformed(evt);
        }
    });

    jBtn9.setFont(new java.awt.Font("Tahoma", 1, 24)); // NOI18N
    jBtn9.setText("9");
    jBtn9.addActionListener(new java.awt.event.ActionListener() {
        public void actionPerformed(java.awt.event.ActionEvent evt) {
            jBtn9ActionPerformed(evt);
        }
    });

    jBtn0.setFont(new java.awt.Font("Tahoma", 1, 24)); // NOI18N
    jBtn0.setText("0");
    jBtn0.addActionListener(new java.awt.event.ActionListener() {
        public void actionPerformed(java.awt.event.ActionEvent evt) {
            jBtn0ActionPerformed(evt);
        }
    });

    jBtnDecimal.setFont(new java.awt.Font("Tahoma", 1, 24)); // NOI18N
    jBtnDecimal.setText(".");
    jBtnDecimal.addActionListener(new java.awt.event.ActionListener() {
        public void actionPerformed(java.awt.event.ActionEvent evt) {
            jBtnDecimalActionPerformed(evt);
        }
    });

    jBtnPlusMinus.setFont(new java.awt.Font("Tahoma", 1, 14)); // NOI18N
    jBtnPlusMinus.setText("-/+");
    jBtnPlusMinus.addActionListener(new java.awt.event.ActionListener() {
        public void actionPerformed(java.awt.event.ActionEvent evt) {
            jBtnPlusMinusActionPerformed(evt);
        }
    });

    jBtnClear.setFont(new java.awt.Font("Tahoma", 1, 24)); // NOI18N
    jBtnClear.setText("C");
    jBtnClear.addActionListener(new java.awt.event.ActionListener() {
        public void actionPerformed(java.awt.event.ActionEvent evt) {
            jBtnClearActionPerformed(evt);
        }
    });

    jBtnAdd.setFont(new java.awt.Font("Tahoma", 0, 24)); // NOI18N
    jBtnAdd.setText("+");
    jBtnAdd.addActionListener(new java.awt.event.ActionListener() {
        public void actionPerformed(java.awt.event.ActionEvent evt) {
            jBtnAddActionPerformed(evt);
        }
    });

    jBtnSubtract.setFont(new java.awt.Font("Tahoma", 0, 24)); // NOI18N
    jBtnSubtract.setText("-");
    jBtnSubtract.addActionListener(new java.awt.event.ActionListener() {
        public void actionPerformed(java.awt.event.ActionEvent evt) {
            jBtnSubtractActionPerformed(evt);
        }
    });

    jBtnDivide.setFont(new java.awt.Font("Tahoma", 0, 24)); // NOI18N
    jBtnDivide.setText("/");
    jBtnDivide.addActionListener(new java.awt.event.ActionListener() {
        public void actionPerformed(java.awt.event.ActionEvent evt) {
            jBtnDivideActionPerformed(evt);
        }
    });

    jBtnMultiply.setFont(new java.awt.Font("Tahoma", 0, 24)); // NOI18N
    jBtnMultiply.setText("*");
    jBtnMultiply.addActionListener(new java.awt.event.ActionListener() {
        public void actionPerformed(java.awt.event.ActionEvent evt) {
            jBtnMultiplyActionPerformed(evt);
        }
    });

    jBtnEqual.setFont(new java.awt.Font("Tahoma", 1, 24)); // NOI18N
    jBtnEqual.setText("=");
    jBtnEqual.addActionListener(new java.awt.event.ActionListener() {
        public void actionPerformed(java.awt.event.ActionEvent evt) {
            jBtnEqualActionPerformed(evt);
        }
    });

    javax.swing.GroupLayout layout = new javax.swing.GroupLayout(getContentPane());
    getContentPane().setLayout(layout);
    layout.setHorizontalGroup(
        layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
        .addGroup(layout.createSequentialGroup()
            .addGap(47, 47, 47)
            .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.TRAILING, false)
                .addComponent(jtxtDisplay, javax.swing.GroupLayout.Alignment.LEADING)
                .addGroup(javax.swing.GroupLayout.Alignment.LEADING, layout.createSequentialGroup()
                    .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING, false)
                        .addGroup(layout.createSequentialGroup()
                            .addComponent(jBtn1, javax.swing.GroupLayout.PREFERRED_SIZE, 59, javax.swing.GroupLayout.PREFERRED_SIZE)
                            .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.RELATED)
                            .addComponent(jBtn2, javax.swing.GroupLayout.PREFERRED_SIZE, 59, javax.swing.GroupLayout.PREFERRED_SIZE)
                            .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.RELATED)
                            .addComponent(jBtn3, javax.swing.GroupLayout.PREFERRED_SIZE, 59, javax.swing.GroupLayout.PREFERRED_SIZE))
                        .addGroup(layout.createSequentialGroup()
                            .addComponent(jBtn4, javax.swing.GroupLayout.PREFERRED_SIZE, 59, javax.swing.GroupLayout.PREFERRED_SIZE)
                            .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.RELATED)
                            .addComponent(jBtn5, javax.swing.GroupLayout.PREFERRED_SIZE, 59, javax.swing.GroupLayout.PREFERRED_SIZE)
                            .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.RELATED)
                            .addComponent(jBtn6, javax.swing.GroupLayout.PREFERRED_SIZE, 59, javax.swing.GroupLayout.PREFERRED_SIZE))
                        .addGroup(layout.createSequentialGroup()
                            .addComponent(jBtn7, javax.swing.GroupLayout.PREFERRED_SIZE, 59, javax.swing.GroupLayout.PREFERRED_SIZE)
                            .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.RELATED)
                            .addComponent(jBtn8, javax.swing.GroupLayout.PREFERRED_SIZE, 59, javax.swing.GroupLayout.PREFERRED_SIZE)
                            .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.RELATED)
                            .addComponent(jBtn9, javax.swing.GroupLayout.PREFERRED_SIZE, 59, javax.swing.GroupLayout.PREFERRED_SIZE)))
                    .addGap(18, 18, 18)
                    .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
                        .addComponent(jBtnAdd, javax.swing.GroupLayout.PREFERRED_SIZE, 62, javax.swing.GroupLayout.PREFERRED_SIZE)
                        .addComponent(jBtnSubtract, javax.swing.GroupLayout.PREFERRED_SIZE, 62, javax.swing.GroupLayout.PREFERRED_SIZE)
                        .addComponent(jBtnDivide, javax.swing.GroupLayout.PREFERRED_SIZE, 62, javax.swing.GroupLayout.PREFERRED_SIZE)
                        .addComponent(jBtnMultiply, javax.swing.GroupLayout.PREFERRED_SIZE, 62, javax.swing.GroupLayout.PREFERRED_SIZE)))
                .addGroup(layout.createSequentialGroup()
                    .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.TRAILING)
                        .addComponent(jBtnClear, javax.swing.GroupLayout.PREFERRED_SIZE, 124, javax.swing.GroupLayout.PREFERRED_SIZE)
                        .addGroup(layout.createSequentialGroup()
                            .addComponent(jBtnDecimal, javax.swing.GroupLayout.PREFERRED_SIZE, 59, javax.swing.GroupLayout.PREFERRED_SIZE)
                            .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.RELATED)
                            .addComponent(jBtn0, javax.swing.GroupLayout.PREFERRED_SIZE, 59, javax.swing.GroupLayout.PREFERRED_SIZE)))
                    .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.RELATED)
                    .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
                        .addComponent(jBtnPlusMinus, javax.swing.GroupLayout.PREFERRED_SIZE, 59, javax.swing.GroupLayout.PREFERRED_SIZE)
                        .addComponent(jBtnEqual, javax.swing.GroupLayout.PREFERRED_SIZE, 139, javax.swing.GroupLayout.PREFERRED_SIZE))))
            .addContainerGap(53, Short.MAX_VALUE))
    );
    layout.setVerticalGroup(
        layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
        .addGroup(layout.createSequentialGroup()
            .addGap(55, 55, 55)
            .addComponent(jtxtDisplay, javax.swing.GroupLayout.PREFERRED_SIZE, 67, javax.swing.GroupLayout.PREFERRED_SIZE)
            .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.UNRELATED)
            .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING, false)
                .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.BASELINE)
                    .addComponent(jBtn1, javax.swing.GroupLayout.PREFERRED_SIZE, 54, javax.swing.GroupLayout.PREFERRED_SIZE)
                    .addComponent(jBtn2, javax.swing.GroupLayout.PREFERRED_SIZE, 54, javax.swing.GroupLayout.PREFERRED_SIZE)
                    .addComponent(jBtn3, javax.swing.GroupLayout.PREFERRED_SIZE, 54, javax.swing.GroupLayout.PREFERRED_SIZE))
                .addComponent(jBtnAdd, javax.swing.GroupLayout.PREFERRED_SIZE, 54, javax.swing.GroupLayout.PREFERRED_SIZE))
            .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.UNRELATED)
            .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.BASELINE)
                .addComponent(jBtn4, javax.swing.GroupLayout.PREFERRED_SIZE, 54, javax.swing.GroupLayout.PREFERRED_SIZE)
                .addComponent(jBtn5, javax.swing.GroupLayout.PREFERRED_SIZE, 54, javax.swing.GroupLayout.PREFERRED_SIZE)
                .addComponent(jBtn6, javax.swing.GroupLayout.PREFERRED_SIZE, 54, javax.swing.GroupLayout.PREFERRED_SIZE)
                .addComponent(jBtnSubtract, javax.swing.GroupLayout.PREFERRED_SIZE, 54, javax.swing.GroupLayout.PREFERRED_SIZE))
            .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.UNRELATED)
            .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING, false)
                .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.BASELINE)
                    .addComponent(jBtn7, javax.swing.GroupLayout.PREFERRED_SIZE, 54, javax.swing.GroupLayout.PREFERRED_SIZE)
                    .addComponent(jBtn8, javax.swing.GroupLayout.PREFERRED_SIZE, 54, javax.swing.GroupLayout.PREFERRED_SIZE)
                    .addComponent(jBtn9, javax.swing.GroupLayout.PREFERRED_SIZE, 54, javax.swing.GroupLayout.PREFERRED_SIZE))
                .addComponent(jBtnDivide, javax.swing.GroupLayout.DEFAULT_SIZE, javax.swing.GroupLayout.DEFAULT_SIZE, Short.MAX_VALUE))
            .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.UNRELATED)
            .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING)
                .addComponent(jBtnMultiply, javax.swing.GroupLayout.PREFERRED_SIZE, 54, javax.swing.GroupLayout.PREFERRED_SIZE)
                .addComponent(jBtnPlusMinus, javax.swing.GroupLayout.PREFERRED_SIZE, 54, javax.swing.GroupLayout.PREFERRED_SIZE)
                .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.BASELINE)
                    .addComponent(jBtn0, javax.swing.GroupLayout.PREFERRED_SIZE, 54, javax.swing.GroupLayout.PREFERRED_SIZE)
                    .addComponent(jBtnDecimal, javax.swing.GroupLayout.PREFERRED_SIZE, 54, javax.swing.GroupLayout.PREFERRED_SIZE)))
            .addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.UNRELATED)
            .addGroup(layout.createParallelGroup(javax.swing.GroupLayout.Alignment.BASELINE)
                .addComponent(jBtnClear, javax.swing.GroupLayout.PREFERRED_SIZE, 55, javax.swing.GroupLayout.PREFERRED_SIZE)
                .addComponent(jBtnEqual, javax.swing.GroupLayout.PREFERRED_SIZE, 55, javax.swing.GroupLayout.PREFERRED_SIZE))
            .addContainerGap(24, Short.MAX_VALUE))
    );

    pack();
}//                         

private void jBtnClearActionPerformed(java.awt.event.ActionEvent evt) {                                          
    jtxtDisplay.setText("");
}                                         

private void jBtn1ActionPerformed(java.awt.event.ActionEvent evt) {                                      
    String enterNum = jtxtDisplay.getText() + jBtn1.getText();
    jtxtDisplay.setText(enterNum);
}                                     

private void jBtn2ActionPerformed(java.awt.event.ActionEvent evt) {                                      
    String enterNum = jtxtDisplay.getText() + jBtn2.getText();
    jtxtDisplay.setText(enterNum);
}                                     

private void jBtn3ActionPerformed(java.awt.event.ActionEvent evt) {                                      
    String enterNum = jtxtDisplay.getText() + jBtn3.getText();
    jtxtDisplay.setText(enterNum);
}                                     

private void jBtn4ActionPerformed(java.awt.event.ActionEvent evt) {                                      
    String enterNum = jtxtDisplay.getText() + jBtn4.getText();
    jtxtDisplay.setText(enterNum);
}                                     

private void jBtn5ActionPerformed(java.awt.event.ActionEvent evt) {                                      
    String enterNum = jtxtDisplay.getText() + jBtn5.getText();
    jtxtDisplay.setText(enterNum);
}                                     

private void jBtn6ActionPerformed(java.awt.event.ActionEvent evt) {                                      
    String enterNum = jtxtDisplay.getText() + jBtn6.getText();
    jtxtDisplay.setText(enterNum);
}                                     

private void jBtn7ActionPerformed(java.awt.event.ActionEvent evt) {                                      
    String enterNum = jtxtDisplay.getText() + jBtn7.getText();
    jtxtDisplay.setText(enterNum);
}                                     

private void jBtn8ActionPerformed(java.awt.event.ActionEvent evt) {                                      
    String enterNum = jtxtDisplay.getText() + jBtn8.getText();
    jtxtDisplay.setText(enterNum);
}                                     

private void jBtn9ActionPerformed(java.awt.event.ActionEvent evt) {                                      
    String enterNum = jtxtDisplay.getText() + jBtn9.getText();
    jtxtDisplay.setText(enterNum);
}                                     

private void jBtn0ActionPerformed(java.awt.event.ActionEvent evt) {                                      
    String enterNum = jtxtDisplay.getText() + jBtn0.getText();
    jtxtDisplay.setText(enterNum);
}                                     

private void jBtnAddActionPerformed(java.awt.event.ActionEvent evt) {                                        
    firstnum = Double.parseDouble(jtxtDisplay.getText());
    jtxtDisplay.setText("");
    operation = "+";
}                                       

private void jBtnEqualActionPerformed(java.awt.event.ActionEvent evt) {                                          
    secondnum = Double.parseDouble(jtxtDisplay.getText());
    String answer;
    switch(operation)
    {
        // Cases for mathematical operations
        case "+":
            result = firstnum + secondnum;
            break;
        case "-":
            result = firstnum - secondnum;
            break;
        case "/":
            result = firstnum / secondnum;
            break;
        case "*":
            result = firstnum * secondnum;
            break;
            
    }
    // Displats result in format
    answer = String.format("%.3f", result);
    jtxtDisplay.setText(answer);
    
}                                         

private void jBtnSubtractActionPerformed(java.awt.event.ActionEvent evt) {                                             
            firstnum = Double.parseDouble(jtxtDisplay.getText());
    jtxtDisplay.setText("");
    operation = "-";
}                                            

private void jBtnDivideActionPerformed(java.awt.event.ActionEvent evt) {                                           
            firstnum = Double.parseDouble(jtxtDisplay.getText());
    jtxtDisplay.setText("");
    operation = "/";
}                                          

private void jBtnMultiplyActionPerformed(java.awt.event.ActionEvent evt) {                                             
            firstnum = Double.parseDouble(jtxtDisplay.getText());
    jtxtDisplay.setText("");
    operation = "*";
}                                            

private void jBtnPlusMinusActionPerformed(java.awt.event.ActionEvent evt) {                                              
    if(!jtxtDisplay.getText().equals(""))
    {
        double value = Double.parseDouble(jtxtDisplay.getText());
        value *= -1;
        jtxtDisplay.setText(String.format("%.3f",value));
    }
    
    
}                                             

private void jBtnDecimalActionPerformed(java.awt.event.ActionEvent evt) {                                            
    if(jtxtDisplay.getText().indexOf(".") < 0)
    {
        String enterNum = jtxtDisplay.getText() + jBtnDecimal.getText();
        jtxtDisplay.setText(enterNum);
        
    }
}                                           

/**
 * @param args the command line arguments
 */
public static void main(String args[]) {
    /* Set the Nimbus look and feel */
    //
    /* If Nimbus (introduced in Java SE 6) is not available, stay with the default look and feel.
     * For details see http://download.oracle.com/javase/tutorial/uiswing/lookandfeel/plaf.html 
     */
    try {
        for (javax.swing.UIManager.LookAndFeelInfo info : javax.swing.UIManager.getInstalledLookAndFeels()) {
            if ("Nimbus".equals(info.getName())) {
                javax.swing.UIManager.setLookAndFeel(info.getClassName());
                break;
            }
        }
    } catch (ClassNotFoundException ex) {
        java.util.logging.Logger.getLogger(Calculator.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
    } catch (InstantiationException ex) {
        java.util.logging.Logger.getLogger(Calculator.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
    } catch (IllegalAccessException ex) {
        java.util.logging.Logger.getLogger(Calculator.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
    } catch (javax.swing.UnsupportedLookAndFeelException ex) {
        java.util.logging.Logger.getLogger(Calculator.class.getName()).log(java.util.logging.Level.SEVERE, null, ex);
    }
    //

    /* Create and display the form */
    java.awt.EventQueue.invokeLater(new Runnable() {
        public void run() {
            new Calculator().setVisible(true);
        }
    });
}

// Variables declaration - do not modify                     
private javax.swing.JButton jBtn0;
private javax.swing.JButton jBtn1;
private javax.swing.JButton jBtn2;
private javax.swing.JButton jBtn3;
private javax.swing.JButton jBtn4;
private javax.swing.JButton jBtn5;
private javax.swing.JButton jBtn6;
private javax.swing.JButton jBtn7;
private javax.swing.JButton jBtn8;
private javax.swing.JButton jBtn9;
private javax.swing.JButton jBtnAdd;
private javax.swing.JButton jBtnClear;
private javax.swing.JButton jBtnDecimal;
private javax.swing.JButton jBtnDivide;
private javax.swing.JButton jBtnEqual;
private javax.swing.JButton jBtnMultiply;
private javax.swing.JButton jBtnPlusMinus;
private javax.swing.JButton jBtnSubtract;
private javax.swing.JTextField jtxtDisplay;
// End of variables declaration              
