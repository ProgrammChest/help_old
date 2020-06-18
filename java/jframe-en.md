# JFrame Example

```java

import java.awt.FlowLayout;  
import javax.swing.JButton;  
import javax.swing.JFrame;  
import javax.swing.JLabel;  
import javax.swing.Jpanel;  

public class JFrameExample {  

    public static void main(String[] args) {
        //Basics
        JFrame frame = new JFrame("JFrameExample");  
        JPanel panel = new JPanel();  
        panel.setLayout(new FlowLayout());  

        //Components
        JLabel label = new JLabel("Simple JFrame Example");  
        JButton button = new JButton();  
        button.setText("MyButton");  
        panel.add(label);  
        panel.add(button);  
        frame.add(panel);

        //Window Settings
        frame.setSize(200, 300);  
        frame.setLocationRelativeTo(null);  
        frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);  
        frame.setVisible(true);  
    }  
}
```

## Source

Discord: $_Dominik#8860 | info@dominikdev.de
  